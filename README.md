## Whatis it?

http://guides.rubyonrails.org/getting_started.html.

## Vocabulary

Exotic terms found along the road:

 - Action: A method that processes a URL.
 - Controller: A collection of actions.
 - Migration: A class for table creation and updates.
 - Rake: `make` for Ruby (Ruby Make). [More](http://guides.rubyonrails.org/command_line.html#rake).
 - Resource: A collection of similar objects. [More](http://guides.rubyonrails.org/routing.html).

> **Resource.** This term is not well defined in this tutorial. It could be confused with a model, however, it's a bit more than a model. As far as I understand, a resource acts as a middleman between a model and the corresponding routes, while a model is only meant to deal with the data. Furtermore, the resource routing system is shipped with a REST API generator, and provides a convenient set of methods to interact with routes.

## For Linux users

### Required

    $ sudo apt-get install ruby-dev
    $ sudo gem install rails -V --no-ri --no-rdoc
    $ sudo apt-get install libsqlite3-dev

### Tips

Mute rails server:

    $ bin/rails server &> /dev/null &
    [1] 16854

Stop rails server:

    $ fg 1
    bin/rails server &> /dev/null
    ^C

Or:

    $ kill -9 16854
