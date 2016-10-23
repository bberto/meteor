# meteor
Meteor docker container

to build:
`docker build -t bberto/meteor .`

to run:
`docker run --name myapp -v /host/myapp/code:/code -p 4000:3000 bberto/meteor`
  
to initially copy app files:
`docker cp . myapp:/app`

to rsync:
`docker exec calipso rsync -av --exclude-from /code/.dockerignore /code /app`
