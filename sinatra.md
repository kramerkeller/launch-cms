Sinatra

Create a filename for your application

`mkdir application`

Create main application file

`atom application.rb`

initialize git

`git init`

setup remote repo and push

Create a Gemfile:

`atom Gemfile`

Add the following code to `Gemfile`

```ruby
source "https://rubygems.org"

ruby "2.5"

gem "sinatra"
gem "sinatra-contrib"
gem "erubis"
```

Run bundle install

`bundle install`

*You should now see a Gemfile.lock file*

Add the following code to `application.rb`:

```ruby
require "sinatra"
require "sinatra/reloader" if development?
require "sinatra/content_for"
require "tilt/erubis"

get "/" do
  "Hello World"
end
```

Starup the app

`ruby application.rb`

Test the route above at **localhost://4567**

DON'T FORGET GIT

`git commit -m "install sinatra"`
