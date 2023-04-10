# Laravel Cheatsheet

## Unique Features

- Model-View-Controller (MVC) architecture
- Artisan command-line interface
- Object-Relational Mapping (ORM)
- Blade template engine
- Routing
- Eloquent ORM

## Models

```php
// Define a model
class ModelName extends Model
{
    protected $fillable = ['field_name'];
}

// Create a migration
php artisan make:migration create_model_names_table

// Apply migrations
php artisan migrate
```

## Controllers

```php
// Define a controller
class ControllerName extends Controller
{
    public function functionName(Request $request)
    {
        // Controller body
        return view('view_name');
    }
}

// Route to a controller method
Route::get('/url', [ControllerName::class, 'functionName']);
```

## Views

```html
<!-- Blade syntax -->
@foreach ($items as $item)
    {{ $item->attribute }}
@endforeach
```

## Forms

```html
<!-- Blade syntax for form -->
<form method="POST" action="/url">
    @csrf
    <input type="text" name="field_name">
    <button type="submit">Submit</button>
</form>

<!-- Handle form submission in controller -->
public function functionName(Request $request)
{
    $model = new ModelName;
    $model->field_name = $request->input('field_name');
    $model->save();
    return redirect('/success');
}
```

## Authentication

```php
// User registration
public function register(Request $request)
{
    $validatedData = $request->validate([
        'name' => 'required|max:255',
        'email' => 'required|email|unique:users|max:255',
        'password' => 'required|confirmed|min:8',
    ]);

    $user = User::create([
        'name' => $validatedData['name'],
        'email' => $validatedData['email'],
        'password' => Hash::make($validatedData['password']),
    ]);

    Auth::login($user);

    return redirect(RouteServiceProvider::HOME);
}

// User login
public function login(Request $request)
{
    $credentials = $request->validate([
        'email' => 'required|email',
        'password' => 'required',
    ]);

    if (Auth::attempt($credentials)) {
        $request->session()->regenerate();

        return redirect()->intended(RouteServiceProvider::HOME);
    }

    throw ValidationException::withMessages([
        'email' => __('auth.failed'),
    ]);
}

// User logout
public function logout(Request $request)
{
    Auth::logout();

    $request->session()->invalidate();

    $request->session()->regenerateToken();

    return redirect('/');
}
```

## Resources

- [Laravel Documentation](https://laravel.com/docs)
- [Laravel From Scratch](https://laracasts.com/series/laravel-6-from-scratch)
- [Laravel News](https://laravel-news.com/)