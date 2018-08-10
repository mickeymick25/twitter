# My Twitter
The idea aim to partially reproduce the twitter website main functionnalities
This is based on this tutorial:
https://web-crunch.com/lets-build-with-ruby-on-rails-a-twitter-clone/

## Getting Started
Not being a developer but UX you could see some code breaks or bad practices...
I tried to use docker in dev environnement, so i followed this tutorial :
https://blog.blindside.io/developing-a-ruby-on-rails-app-with-docker-compose-d75b20334634


So to build docker image :
```
docker-compose build --force-rm web
```
Then create the database:
```
docker-compose run --rm web rails db:create
```
Then migrate the database:
```
docker-compose run --rm web rails db:migrate
```
Then launch the container:
```
docker-compose up web
```
