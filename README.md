# meteor
Meteor docker container

to build:
`docker build -t bberto/meteor .`

to run:
`docker run --name myapp -v /host/myapp/code:/code bberto/meteor`
  
to rsync:
`docker exec calipso rsync -av --exclude-from /code/.dockerignore /code /app`
