# website
PiE's public-facing website, built on Jekyll.

# Docker Container for Jekyll
Docker Hub: <https://hub.docker.com/r/numascott/docker-whale/>

Docker Pull Command

    docker pull numascott/docker-whale

###Usage:

Navigate to within the jekyll webiste folder then run

    docker run -d -v "$(pwd):/src" -p 4000:4000 numascott/jekyll serve

The jekyll site should be available at The jekyll site should be available at <http://192.168.99.100:4000>
