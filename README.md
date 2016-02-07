# Docker Container for Jekyll
Docker Hub: <https://hub.docker.com/r/numascott/docker-whale/>

Docker Pull Command

    docker pull numascott/docker-whale

###Usage:

Navigate to within the jekyll webiste folder then run

    docker run -d -v "$(pwd):/src" -p 4000:4000 numascott/jekyll serve