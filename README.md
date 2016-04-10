# Installation Instructions

- Get [docker](https://docs.docker.com/engine/installation/)
- Get [jekyll](https://hub.docker.com/r/jekyll/jekyll/) image: `docker pull jekyll/jekyll`
- Run ``POLLING=true docker run --rm --label=jekyll --volume=$(pwd):/srv/jekyll -it -p $(docker-machine ip `docker-machine active`):4000:4000 jekyll/jekyll``
- Then navigate to [docker-machine ip]:4000 to view the site