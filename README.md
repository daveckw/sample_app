# Ruby on Rails Tutorial sample application

This is the sample application for
[*Ruby on Rails Tutorial:
Learn Web Development with Rails*](http://www.railstutorial.org/)
by [Michael Hartl](http://www.michaelhartl.com/).

## License

All source code in the [Ruby on Rails Tutorial](http://railstutorial.org/)
is available jointly under the MIT License and the Beerware License. See
[LICENSE.md](LICENSE.md) for details.

## Getting started

To get started with the app, clone the repo and then install the needed gems:

```
$ bundle install --without production
```

Next, migrate the database:

```
$ rails db:migrate
```

Finally, run the test suite to verify that everything is working correctly:

```
$ rails test
```

If the test suite passes, you'll be ready to run the app in a local server:

```
$ rails server
```
## Git Initialization

git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/daveckw/sample_app.git
git push -u origin master

## Heroku Initialization
$ git commit -am "Add hello"
$ git push
$ heroku create
$ git push heroku master

## Generate Static Pages Home and Help
$ rails generate controller StaticPages home help

##  good idea to add the files for the Static Pages controller to the remote repository:
$ git add -A
$ git commit -m "Add a Static Pages controller"
$ git push -u origin static-pages

## Bcrypt 3.1.11 - Cannot load file on Windows
I solve it with uninstall all bcrypt gem versions with gem uninstall bcrypt and select option 3 (if exist) and uninstall all bcrypt-ruby gem versions with gem uninstall bcrypt-ruby and select option 3 (if exist) then install bcrypt using gem install bcrypt --platform=ruby then add this line gem 'bcrypt', platforms: :ruby to Gemfile, that is it :D.


##---------------------------------------------##

For more information, see the
[*Ruby on Rails Tutorial* book](http://www.railstutorial.org/book).
