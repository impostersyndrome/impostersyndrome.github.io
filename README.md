# Usage Instructions

- Get [docker](https://docs.docker.com/engine/installation/)
- Get [jekyll](https://hub.docker.com/r/jekyll/jekyll/) image: `docker pull jekyll/jekyll`
- Run ``docker run --rm --label=jekyll --volume=$(pwd):/srv/jekyll -it -p $(docker-machine ip `docker-machine active`):4000:4000 jekyll/jekyll jekyll serve --force_polling``
- Then navigate to ``$(`docker-machine ip `docker-machine active`) ``:4000 to view the site

# Deployment Instructions

- Push the master branch to github.

### Thanks

Built using [poole](https://github.com/poole/poole)