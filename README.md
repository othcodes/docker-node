## To start the application

Step 1: build node image from Dockerfile

    docker build -t my-app:1.0 .

Step 2: start mongodb and mongo-express

    docker-compose -f docker-compose.yaml up -d

(Then access the mongo-express under localhost:8080 from your browser)

Step 3: in mongo-express UI - create a new database "my-db"

Step 4: in mongo-express UI - create a new collection "users" in the database "my-db"

Step 5: inside the "app" folder start node server

    npm install
    node server.js

Step 6: access the nodejs application from browser

    http://localhost:3000
