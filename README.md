# public

docker build -t cognitrandocker/hello .

docker run cognitrandocker/hello

// refers to the base image provided
FROM cognitrandocker/hello

// in order to populate the env var the script is trying to output
ENV ABC=hello

// in order to make the script executable
RUN chmod +x /opt/hello.sh
