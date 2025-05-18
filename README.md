# Ruby on Rails Tutorial sample application
 This is the sample application for
 [*Ruby on Rails Tutorial:
 Learn Web Development with Rails*](https://www.railstutorial.org/)
 (6th Edition)
 by [Michael Hartl](https://www.michaelhartl.com/).
 ## License
 All source code in the [Ruby on Rails Tutorial](https://www.railstutorial.org/)
 is available jointly under the MIT License and the Beerware License. See
 [LICENSE.md](LICENSE.md) for details.
 ## Getting started
 To get started with the app, clone the repo and then install the needed gems:
 ```
 $ bundle install--without production
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
 For more information, see the
 [*Ruby on Rails Tutorial* book](https://www.railstutorial.org/book).

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


Cambios en application

<!DOCTYPE html>
<html>
  <head>
    <title><%= full_title(yield(:title)) %></title>
    <meta charset="utf-8">
    <%= csrf_meta_tags %>
    <%= csp_meta_tag %>
    <%= stylesheet_link_tag 'application', media: 'all',
    'data-turbolinks-track': 'reload' %>
    <%= javascript_include_tag "application", "data-turbo-track": "reload", defer: true %>
  </head>
  <body>
    <%= yield %>
  </body>
</html>