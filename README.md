Basic React/Express web app that stores info on all US congress members in a mongo db and uses an extremely simple microservices structure with Docker.

Each service needs a .env file with the following in it:

DB_URL=mongodb://database:27017/YOUR_DB_NAME \
VOTESMART_API_KEY=YOUR_VOTE_SMART_API_KEY \
REACT_APP_BASE_API_URL=http://0.0.0.0:3000 \
REACT_APP_STATES_ENDPOINT=states \
REACT_APP_OFFICIALS_ENDPOINT=officials

### Steps to Run

1) Install latest version of Docker 
2) make sure you are in project root folder
3)```docker-compose build --no-cache```
4) ```docker-compose up```
5) Open new terminal window that is also in project root folder
6) ```docker-compose exec congressional-members-search-api npm run seed```
7) Watch data fetching progress!
8) Go to http://localhost