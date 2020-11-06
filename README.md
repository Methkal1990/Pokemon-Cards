### To run the app

`npm install`

`npm start`

### To run with docker

`docker build -t react-docker .`

`docker run -p 8080:8080 react-docker`

check in your browser with **localhost:8080**

### An issue

You may face an issue when trying to build your Docker image with context:

`ERESOLVE unable to resolve dependency tree`

That's due to some new changes in npm and node. You can resolve it by changing in Dockerfile:

`Run npm install` to `Run npm install --legacy-peer-deps`

### The same project with Webpack

https://github.com/Methkal1990/Pokemon-Cards-webpack

