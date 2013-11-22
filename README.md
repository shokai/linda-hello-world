# Linda Hello World

very simple Sinatra [RocketIO Linda application](https://github.com/shokai/sinatra-rocketio-linda).

- https://github.com/shokai/linda-hello-world
- [demo](http://hello-linda.shokai.org)


## Install Dependencies

    % gem install bundler
    % bundle install


## Run

    % bundle exec rackup config.ru -p 5000

=> http://localhost:5000


### set websocket port

    % WS_PORT=5001 bundle exec rackup config.ru -p 5000
