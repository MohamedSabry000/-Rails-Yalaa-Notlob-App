# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## Steps:
* run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java` for giving the availability to run the command `bundle install`.

* Following => (How to add bootstrap 5 to an existing Rails 7 app)[https://www.uday.net/add-bootstrap-5-to-an-existing-Rails-7-app]
 * add those 2 lines into _**Gemfile**_
 ```
 gem 'jsbundling-rails'  # needed for bootstrap javascript
 gem 'cssbundling-rails' # Install bootstrap 5
 ```
* run `bundle install`
* run `rails javascript:install:esbuild`
* run `rails css:install:bootstrap`
 * found **bootstrap** is already installed