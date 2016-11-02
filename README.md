#Description
Here's a Rails app with the Bourbon family installed, featuring:
* [Bourbon](https://github.com/thoughtbot/bourbon): A simple and lightweight mixin library for Sass
* [Neat](https://github.com/thoughtbot/neat): A lightweight semantic grid framework for Sass and Bourbon
* [Bitters](https://github.com/thoughtbot/bitters): Scaffold styles, variables and structure for Bourbon projects
* [Refills](https://github.com/thoughtbot/refills): Prepackaged patterns and components built with Bourbon, Neat and Bitters

> If you want to start building and customizing on a fresh Rails app right away, clone/fork the repo. Otherwise, if you'd like to install it on your own Rails app, read on for more details.

#Installation
Run bundle install on the command line.
```bash
bundle install
```

Install bourbon, neat, bitters, and refills.
```bash
gem install bourbon
gem install neat
gem install bitters
gem "refills", group: :development
```

Rename your application.css to application.scss

Watch for changes in app directory:
``sass --watch application.scss:app.css``

Import bourbon, bitters, neat, refills for use in your rails app. Make sure you're in app/assets/stylesheets/css/0-plugins:
```bash
bourbon install
bitters install
neat install
rails generate refills:list
rails generate refills:import SNIPPET
```

*Go to application.scss and import them!*
```bash
@import 'bourbon/bourbon';
@import 'neat/neat';
@import 'base/base';
```
> Note: Refills installs in the views folder, so there's no need to import them into application.scss
