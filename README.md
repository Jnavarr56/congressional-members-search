Basic React/Express web app that stores info on all US congress members in a mongo db and uses an extremely simple microservices structure with Docker.

1) Install latest version of Docker
2) ```docker-compose build --no-cache```
3) ```docker-compose up```
4) Open new terminal window
5) docker-compose exec  congressional-members-search-api npm run seed
4) Go to http://localhost:8080