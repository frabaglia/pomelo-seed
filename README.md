#Pomelo Seed

##Install Node and NPM: Ubuntu 14.04

- curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
- sudo apt-get install -y nodejs npm

##Install global dependencies
- npm install -g pomelo pomelo-cli pm2

##Run web server

- cd express-server
- pm2 start ./bin/www

##Run game server

- cd game-server
- pomelo start --daemon
