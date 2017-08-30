# pzc-node-red
My node-red installation with various included packages.

I used yarn on my system to set this up.

    [~/pzc-node-red]$ yarn install
    
This will install a myriad of packages, and plugins into this instance of node-red.

node-red currently uses the ~/.node-red directory for data, so multiple instances won't work properly *(I think)

I'll figure out how to make it more instance oriented later.

I've been sharing this with my friends who aren't software professionals, so the path to getting this to work on most linux setups is:

* NVM (Node Version Manager)
* Install Node
* Install Yarn
* Clone this repository with git
* Install the dependancies
* Run the server

https://github.com/creationix/nvm

Installation:

    # this will download the NVM install file and run it.
    wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash

    # this will bring in your node nvm settings so you can use nvm in this shell
    # you only have to do this during the install, when you open a new terminal node/nvm will work fine.
    . ~/.nvm/nvm.sh
    
    # this will install node.js (version 6 is the LTS)
    nvm install v6
    
    # this will install the yarn package management tool
    npm install -g yarn
    
    # this will clone over the pzc-node-red setup
    git clone https://github.com/prozacgod/pzc-node-red.git
    
    # change into it's directory
    cd pzc-node-red
    
    # install the dependancies with yarn
    yarn install
    
    # and run the node-red server
    yarn run node-red
    
Good luck!!
