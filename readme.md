# StoryZoo Website

Hugo site built using: [Klakegg\hugo](https://hub.docker.com/r/klakegg/hugo/)
Down side of running via a container is you don't get live reload.
If you want live reload then you need to install Hugo locally

## Serve

### Powershell

docker run --rm -it -p 1313:1313 -v ${pwd}:/src klakegg/hugo:ext-alpine serve

### Bash

docker run --rm -it -p 1313:1313 -v $(pwd):/src klakegg/hugo:ext-alpine serve

## Build

### Powershell

docker run --rm -it -v ${pwd}:/src klakegg/hugo:latest

### Bash

docker run --rm -it -v $(pwd):/src klakegg/hugo:latest

## Deploy

Cloudflare is configured to build and deploy ALL changes to the Main branch to production, any changes to other branches deploy to a Preview branch

## Dependencies

Bootstrap added as per: [https://www.noorix.com.au/blog/how-to/static-website-hugo-bootstrap-serverless-2](https://www.noorix.com.au/blog/how-to/static-website-hugo-bootstrap-serverless-2)


## TODO:

1. [] - Ensure FavIcon is correct
1. [] - Story Card needs to be link. Not just the read more 