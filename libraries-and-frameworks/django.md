# Django Cheatsheet

## Unique Features

- Model-View-Controller (MVC) architecture
- Object-Relational Mapping (ORM)
- Automatic admin interface
- URL routing
- Template system
- Django Rest Framework

## Models

```python
# Define a model
class ModelName(models.Model):
    field_name = models.FieldType()

# Create a migration
python manage.py makemigrations

# Apply migrations
python manage.py migrate
```

## Views

```python
# Define a view
def view_name(request):
    # View body
    return HttpResponse("Response")

# URL routing
path('url/', views.view_name, name='view_name'),
```

## Templates

```html
<!-- Template syntax -->
{% for item in items %}
    {{ item.attribute }}
{% endfor %}
```

## Forms

```python
# Define a form
class FormName(forms.Form):
    field_name = forms.FieldType()

# Render a form
def view_name(request):
    form = FormName()
    return render(request, 'template.html', {'form': form})

# Handle form submission
def view_name(request):
    form = FormName(request.POST)
    if form.is_valid():
        # Form handling code
```

## Authentication

```python
# User registration
def register(request):
    if request.method == 'POST':
        form = UserCreationForm(request.POST)
        if form.is_valid():
            form.save()
            return redirect('login')
    else:
        form = UserCreationForm()
    return render(request, 'registration/register.html', {'form': form})

# User login
def login(request):
    if request.method == 'POST':
        username = request.POST['username']
        password = request.POST['password']
        user = authenticate(request, username=username, password=password)
        if user is not None:
            auth_login(request, user)
            return redirect('home')
        else:
            messages.error(request, 'Invalid username or password')
    return render(request, 'registration/login.html')

# User logout
def logout(request):
    auth_logout(request)
    return redirect('login')
```

## Resources

- [Django Documentation](https://docs.djangoproject.com/)
- [Django Girls Tutorial](https://tutorial.djangogirls.org/)
- [Django for Beginners](https://djangoforbeginners.com/)