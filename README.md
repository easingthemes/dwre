##dwre
=========


-------------------------------------------
##Prepare
___________________________________________

- Check dependencies, and update to latest
- Ruby, Sass, Compass, NodeJs, Git

### NODEJS update
```sh
sudo apt-get install python-software-properties
sudo add-apt-repository ppa:chris-lea/node.js
sudo apt-get update
sudo apt-get install nodejs
```

### node modules - globall
```sh
sudo npm install -g yo
sudo npm install -g grunt-cli
sudo npm install -g bower
sudo npm install -g karma
sudo npm install -g karma-cli
```

-------------------------------------------
Project 'dwre'
___________________________________________

mkdir dwre && cd $_

sudo npm install -g generator-webapp

yo webapp dwre
***lot of errors for bower and npm, not yo.

--add description, name, repo etc. in package.json
--change deprecated modules

// Run npm and bower again if you got errors

sudo npm install
bower install //no sudo here

export NODE_PATH=/usr/bin/node/lib/node_modules/
-------------------------------------------
Testing
___________________________________________

grunt serve //ok
grunt test //karma error

npm install grunt-karma --save-dev
npm install karma-phantomjs-launcher --save-dev
npm install karma-jasmine --save-dev
sudo npm install -g phantomjs
sudo npm install phantomjs

grunt test //ok

// DEVELOPE ...... FINISH, BUILD
grunt build
//resolve errors
sudo npm install grunt-ngmin --save-dev

grunt build
//Now we got dist folder for our app

-------------------------------------------
Git
___________________________________________

git init
git remote add ugithub https://github.com/easingthemes/repo.git
git remote add bitbucket git@bitbucket.org:easingthemes/repo.git
git remote -v

* git add .
* git commit -m "commit message"
** git commit -a
git push -u bitbucket --all
* git push upstream master
* git pull upstream master

git remote set-url github git@github.com:easingthemes/newrepo.git



