FROM golang:1.21-bookworm 

# Create and change to the app directory.
WORKDIR /app

COPY src/go.* ./
RUN go mod download

# Copy local code to the container image.
COPY ./src ./

# Build the binary.
RUN go build -o server

# Run the web service on container startup.
CMD ["/app/server"]
