# ASP.NET Cheatsheet

## Unique Features

- Web framework for building web applications on the .NET platform
- Model-View-Controller (MVC) architecture
- Razor view engine
- Entity Framework
- ASP.NET Identity

## Controllers

```csharp
// Define a controller
public class ControllerName : Controller
{
    public IActionResult FunctionName()
    {
        // Controller body
        return View();
    }
}

// Route to a controller action
app.UseEndpoints(endpoints =>
{
    endpoints.MapControllerRoute(
        name: "default",
        pattern: "{controller=Home}/{action=Index}/{id?}");
});
```

## Views

```html
<!-- Razor syntax -->
@foreach (var item in Model.Items)
{
    <span>@item.Attribute</span>
}
```

## Forms

```html
<!-- HTML syntax for form -->
<form method="POST" action="/url">
    <input type="text" name="field_name">
    <button type="submit">Submit</button>
</form>

<!-- Handle form submission in controller -->
[HttpPost("/url")]
public IActionResult FunctionName(ModelName model)
{
    // Form handling code
    return RedirectToAction("Success");
}
```

## Database

```csharp
// Connect to a database
services.AddDbContext<ApplicationDbContext>(options =>
    options.UseSqlServer(Configuration.GetConnectionString("DefaultConnection")));

// Define a model
public class ModelName
{
    public int Id { get; set; }
    public string FieldName { get; set; }
}

// Create a migration
dotnet ef migrations add MigrationName

// Apply migrations
dotnet ef database update
```

## Authentication

```csharp
// User registration
[HttpPost("/register")]
public async Task<IActionResult> Register(RegisterViewModel model)
{
    if (ModelState.IsValid)
    {
        var user = new ApplicationUser { UserName = model.Email, Email = model.Email };
        var result = await _userManager.CreateAsync(user, model.Password);
        if (result.Succeeded)
        {
            await _signInManager.SignInAsync(user, isPersistent: false);
            return RedirectToAction("Index", "Home");
        }
        foreach (var error in result.Errors)
        {
            ModelState.AddModelError(string.Empty, error.Description);
        }
    }
    return View(model);
}

// User login
[HttpPost("/login")]
public async Task<IActionResult> Login(LoginViewModel model, string returnUrl = null)
{
    returnUrl ??= Url.Content("~/");
    var result = await _signInManager.PasswordSignInAsync(model.Email, model.Password, model.RememberMe, lockoutOnFailure: false);
    if (result.Succeeded)
    {
        return LocalRedirect(returnUrl);
    }
    ModelState.AddModelError(string.Empty, "Invalid login attempt.");
    return View(model);
}

// User logout
[HttpPost("/logout")]
public async Task<IActionResult> Logout()
{
    await _signInManager.SignOutAsync();
    return RedirectToAction("Index", "Home");
}
```

## Resources

- [ASP.NET Documentation](https://dotnet.microsoft.com/learn/aspnet/what-is-aspnet)
- [ASP.NET Core Tutorial](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/start-mvc?view=aspnetcore-5.0&tabs=visual-studio)
- [Entity Framework Core Tutorial](https://docs.microsoft.com/en-us/ef/core/get-started/?tabs=netcore-cli)