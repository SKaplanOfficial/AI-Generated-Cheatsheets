# Flask Cheatsheet

## Unique Features

- Lightweight web framework
- Jinja2 template engine
- Werkzeug WSGI toolkit
- URL routing
- Flask extensions

## Routing

```python
# Define a route
@app.route('/url')
def function_name():
    # Route body
    return render_template('template.html')
```

## Templates

```html
<!-- Jinja2 syntax -->
{% for item in items %}
    {{ item.attribute }}
{% endfor %}
```

## Forms

```html
<!-- HTML syntax for form -->
<form method="POST" action="/url">
    <input type="text" name="field_name">
    <button type="submit">Submit</button>
</form>

<!-- Handle form submission in view function -->
@app.route('/url', methods=['GET', 'POST'])
def function_name():
    if request.method == 'POST':
        field_name = request.form['field_name']
        # Form handling code
        return redirect('/success')
    return render_template('template.html')
```

## Database

```python
# Connect to a database
app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///database.db'
db = SQLAlchemy(app)

# Define a model
class ModelName(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    field_name = db.Column(db.String(255), nullable=False)

# Create a migration
flask db init
flask db migrate
flask db upgrade
```

## Authentication

```python
# User registration
@app.route('/register', methods=['GET', 'POST'])
def register():
    form = RegistrationForm()
    if form.validate_on_submit():
        user = User(username=form.username.data, email=form.email.data)
        user.set_password(form.password.data)
        db.session.add(user)
        db.session.commit()
        flash('Congratulations, you are now a registered user!')
        return redirect(url_for('login'))
    return render_template('register.html', title='Register', form=form)

# User login
@app.route('/login', methods=['GET', 'POST'])
def login():
    form = LoginForm()
    if form.validate_on_submit():
        user = User.query.filter_by(username=form.username.data).first()
        if user is None or not user.check_password(form.password.data):
            flash('Invalid username or password')
            return redirect(url_for('login'))
        login_user(user, remember=form.remember_me.data)
        return redirect(url_for('index'))
    return render_template('login.html', title='Sign In', form=form)

# User logout
@app.route('/logout')
def logout():
    logout_user()
    return redirect(url_for('index'))
```

## Resources

- [Flask Documentation](https://flask.palletsprojects.com/)
- [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
- [Flask Extensions](https://flask.palletsprojects.com/en/2.0.x/extensions/)