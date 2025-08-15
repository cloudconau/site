# site
To deploy locally for development purposes:
```sh
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```

To deploy for to Github Pages:
```sh
docker run --rm -it -p 8008:8000 -v $(pwd):/docs -v $SSH_AUTH_SOCK:/ssh-agent -e SSH_AUTH_SOCK=/ssh-agent squidfunk/mkdocs-material gh-deploy 
```