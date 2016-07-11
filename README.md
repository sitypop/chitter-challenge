[![Build Status](https://travis-ci.org/makersacademy/chitter-challenge.svg?branch=master)](https://travis-ci.org/makersacademy/chitter-challenge)

Chitter Challenge
=================


Introduction
------------
Chitter is a little Twitter clone that provides a platform for users to post messages to a public stream.


Features
-------
* User can sign up, log in and log out
* Once logged in, post a message (peep) on Chitter
* Peeps displayed showing poster's name and the time at which the post is created

Instructions
------------------
To experience Chitter locally, clone this repo:
```
$ git clone git@github.com:sitypop/chitter-challenge.git
```
You will need to create a local database to save the data:
```
$ psql
yourusername=# CREATE DATABASE chitter_development;
```
Once your database has been created, type in `\q` to quit Postgres.

In order to create the relevant columns for your database,in the root directory of Chitter, type in Terminal:

```
$ rake db:auto_migrate
```

Next, to start up the server:

```
$ rackup
```

Visit `localhost:9292` in your browser to use the app. You should see the index page.

To post a peep, please sign up:


You should then be able to create a peep:


Testing
-------
To run the tests, you will need to create a `chitter_test` database in Postgres. Then under the root directory of the project, run:

```
$ rake db:auto_migrate
$ bundle install
$ rspec
```

Tools used
-----------
* Ruby
* RSpec
* Sinatra
* Capybara
* DataMapper
* PostgreSQL
* BCrypt

Author
----------------------
Sity Shah
