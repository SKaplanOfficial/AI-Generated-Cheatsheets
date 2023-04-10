# Ruby on Rails Cheatsheet

## Overview
- Ruby on Rails (Rails) is a web application framework written in the Ruby programming language.
- It follows the Model-View-Controller (MVC) architecture pattern and emphasizes convention over configuration.
- Rails is known for its productivity, ease of use, and strong community.

## Installation
- Install Ruby on your system.
- Install Rails using the command: `gem install rails`.
- Verify the installation using the command: `rails --version`.

## Creating a New Rails Application
- To create a new Rails application, use the command: `rails new <app_name>`.
- This will create a new directory with the specified name and generate a basic Rails application structure.

## Routing
- Rails uses a `routes.rb` file to define the application's routes.
- Routes are defined using the `get`, `post`, `put`, `patch`, and `delete` methods.
- Routes can include dynamic segments using the `:id` syntax.

## Controllers
- Controllers are responsible for handling requests and producing responses.
- Controllers are defined in the `app/controllers` directory.
- Controllers should inherit from the `ApplicationController` class.

## Models
- Models represent the data and behavior of the application.
- Models are defined in the `app/models` directory.
- Models should inherit from the `ActiveRecord::Base` class.

## Views
- Views are responsible for displaying the application's data to the user.
- Views are defined in the `app/views` directory.
- Views use Embedded Ruby (ERB) syntax to embed Ruby code in HTML.

## Migrations
- Migrations are used to modify the database schema.
- Migrations are defined in the `db/migrate` directory.
- Migrations can be created using the command: `rails generate migration <migration_name>`.

## Example
```ruby
# Example Rails controller
class UsersController < ApplicationController
  def index
    @users = User.all
  end

  def show
    @user = User.find(params[:id])
  end

  def new
    @user = User.new
  end

  def create
    @user = User.new(user_params)
    if @user.save
      redirect_to @user
    else
      render 'new'
    end
  end

  private

  def user_params
    params.require(:user).permit(:name, :email, :password)
  end
end
```
This Rails controller defines four actions: `index`, `show`, `new`, and `create`. The `index` action retrieves all users from the database and assigns them to the `@users` instance variable. The `show` action retrieves a single user based on the `id` parameter. The `new` action creates a new `User` object. The `create` action creates a new `User` object based on the parameters submitted in a form and saves it to the database. If the user is saved successfully, the user is redirected to their show page. If there are validation errors, the user is shown the new user form again with error messages.

## Resources
- [Ruby on Rails Website](https://rubyonrails.org/)
- [Ruby on Rails Guides](https://guides.rubyonrails.org/)
- [Ruby on Rails API Documentation](https://api.rubyonrails.org/)