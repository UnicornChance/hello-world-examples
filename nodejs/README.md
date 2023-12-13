# Node Hello World Example Project


### GETTING STARTED

### `npm install`

setup the node project with all the correct dependencies and things.

### `npm test:ci`

To be able to run in ci we want to be able to define the coverage output directory and file type. To be able to do this dynamically we need to utilize shell variables. The following is an example command:

`coverageDirectory=../../../Downloads/ coverageReporters=lcov npm run test`

### `npm test`

The default test command that will run a local unit test of the nodejs project.

## Docker

#### Build

From within the `react-app` project directory run:

`docker build -t node-hello-world .`

#### Run

`docker run -it -p 80:8080 node-hello-world`

#### Stop

`docker ps`   - to find the docker container ID

`docker stop <container_id>`