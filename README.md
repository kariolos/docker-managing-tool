## Prerequisites
Make sure you have installed all of the following prerequisites on your development machine:
* Git - [Download & Install Git](https://git-scm.com/downloads). OSX and Linux machines typically have this already installed.
* Node.js - [Download & Install Node.js](https://nodejs.org/en/download/) and the npm package manager. If you encounter any problems, you can also use this [GitHub Gist](https://gist.github.com/isaacs/579814) to install Node.js.
* Docker - [Download & Install Node.js](https://docs.docker.com/install/)

## Downloading tradeline

### Cloning The GitHub Repository
The recommended way to get MEAN.js is to use git to directly clone the MEAN.JS repository:

```bash
$ git clone https://github.com/kariolos/tradeline.git
```

This will clone the latest version of the tradeline repository 

## Quick Install
Once you've downloaded the repository and installed all the prerequisites, you have to install the dependencies

To install the dependencies, run this in the application folder from the command-line:

```bash
$ npm install
```

* It will install the dependencies needed for the application to run.

## Running Your Application

#Run your application using npm:

```bash
$ npm start
```

Your application should run on port 3000 with the *development* environment configuration, so in your browser just go to [http://localhost:3000](http://localhost:3000)

## Development and deployment With Docker

* Install [Docker](https://docs.docker.com/installation/#installation)
* Install [Compose](https://docs.docker.com/compose/install/)

* Local development and testing with compose:
```bash
$ docker-compose up
```

* Local development and testing with just Docker:
```bash
$ docker build -t 'tag-name' .
$ docker run -d -v /var/run/docker.sock:/var/run/docker.sock -p ip:port:3000 'tag-name'
```