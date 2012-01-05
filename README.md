# node-boilerplate
      
  Structure for your non-trivial [node.js](http://nodejs.org) project.

  required: linux/osx, node 0.6.x

  on by default: mongodb, redis

## 1. Develop

  ```shell
  git clone git://github.com/skookum/node-boilerplate.git
  cd node-boilerplate
  sudo npm install
  sudo node server
  ```

## 2. Provision

  - fill out `scripts/deploy.conf`
  - add developers' public keys to `scripts/provisioning/keys`
  - add deploy user's private key outside the repository
  
  ```
  cd scripts
  ./provision staging root
  ```

## 3. Deploy

  ```
  cd scripts
  ./deploy staging setup
  ./deploy staging
  ```

## Adding libraries

  Add to 'dependencies' in /package.json, then:
  
  ```shell
  sudo npm install
  ```