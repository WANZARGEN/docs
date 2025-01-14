# SpaceONE Document  

## How to use this repository 

### Prerequisities 


You need following installed locally 

- npm 
- Go 
- Hugo(Extended version)
- Docker & Docker Compose 

Before we start, install the dependencies, Clone the repository and navigate to the directory. 

```bash
git clone --recurse-submodules --depth 1 https://github.com/spaceone-dev/docs

cd docs

```

SpaceONE blog uses Docsy Hugo theme. So, we strongly recommend pulling in the submodule and other developmment dependencies by running the following. 

```bash
# pull in the Docsy submodule
git submodule update --init --recursive --depth 1

```

### Install PostCSS 

To build SpaceONE blog, you also need  `PostCSS` to create the final asset. If you need install it, you must have recent version of NodeJS installed on your machine so you can use npm. 

```bash
npm install --no-optional -D --save
```

## Running Blog locally 

Once you've made your own working copy of this repo, from the root folder, run: 

```bash
hugo server -D
```

## Running Docker container locally
You can run SpaceONE blog by inside a Docker container. 


```bash 
docker-compose up --build
```

Open you web browser type `http://localhost:1313` in your navigation bar.


To stop Docker Compose, on your terminal window, press Ctrl + C.

To remove the produced images run:

```bash 
docker-compose rm
```