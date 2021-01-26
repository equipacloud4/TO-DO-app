NODE, ANGULAR AND MONGODB APP, YOU CAN APPLY TO DOCKER CONTAINERS.

This APP allows you to create and temporarily store new inputs.

<img src="https://user-images.githubusercontent.com/76655210/105786423-f9662c80-5f74-11eb-9d93-5a04e7542aba.png" width="600">

What you will nedd:
 - git clone this repository
 - docker 
 - node v14.15.4
 - angular cli v11.0.5

Test your APP locally:

MONGODB:
 - Dockerhub already has an image for mongo, so you can use that one, run this in your comand line:
   - docker run -p 27017:27017 -d --name mongo-todolist -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=admin mongo
   
        You can see it on http://localhost:27017/
        
BACKEND:
 - In your comand line go to the Backtend directory and enter these:
   - npm install
   - npm start
   
       You can see it on http://localhost:3000/
       
FRONTEND:
 - In your comand line go to the Frontend directory and enter these:
   - npm install -g @angular/cli@11.0.5
   - npm install 
   - ng serve
   
       The APP will be available on http://localhost:4200/
       
To run your APP on docker containers:
 - Through the docker-compose file, all 3 containers will be created and inicialized. All you have to do is run this comand in your project directory:
   - docker-compose up -d --build
   
       Access the APP through http://localhost:4200/, wait a few seconds and it should work fine.

Have FUN!!!
