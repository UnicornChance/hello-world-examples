# GO Hello World Example Project


### Unit Test Command

If you're in the `goapp` project directory you can run this command to do a basic go unit test.

`go test ./...`

This will recursively check for test fiels to run.

#### Unit Test Coverage Parameters

From the `goapp` project directory we can run this command:

`go test ./... -coverprofile=../../../Downloads/output.out`

This will keep track of the coverage of our unit tests and output to a defined output file.

## Docker

#### Build

From within the `goapp` project directory run:

`docker build -t go-hello-world .`

#### Run

`docker run -it -p 8080:8080 go-hello-world`

#### Stop

`docker ps`   - to find the docker container ID

`docker stop <container_id>`