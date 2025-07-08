# Start from the official Go image
FROM golang:1.24-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the Go files into the container
COPY . .

# Download the dependencies
RUN go mod download

# Build the Go application
RUN go build -o app .

# Expose the port the app runs on
EXPOSE 8080

# Command to run the application
CMD ["./app"]
