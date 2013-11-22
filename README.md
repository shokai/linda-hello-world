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


Install as Service
------------------

for launchd (Mac OSX)

    % sudo foreman export launchd /Library/LaunchDaemons/ --app linda-hello -u `whoami`
    % sudo launchctl load -w /Library/LaunchDaemons/linda-hello-web-1.plist

for upstart (Ubuntu)

    % sudo foreman export upstart /etc/init/ --app linda-hello -d `pwd` -u `whoami`
    % sudo service linda-hello start
