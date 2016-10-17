# README

Do a bundle install

```bash
gem install bourbon
gem install neat
gem install bitters
gem "refills", group: :development
```
# Rename your application.css to application.scss

# Watch for changes in app directory:
``sass --watch application.scss:app.css``

# Make sure you're in app/assets/stylesheets/css/0-plugins:
``bourbon install``
``bitters install``
``neat install``
``rails generate refills:list``
``rails generate refills:import SNIPPET``
# refills install in views

##### Go to application scss and import them! ######

```bash
@import 'bourbon/bourbon'
@import "neat/neat";
@import 'base/base'
```
