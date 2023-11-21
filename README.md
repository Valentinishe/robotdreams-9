# robotdreams-9
Lesson #9


### Running
- install docker and docker-compose in your OS;
- clone the project by run ```git clone git@github.com:Valentinishe/robotdreams-9.git```;
- go to root folder in the project;
- go to /app folder and create `nodejs` image by run ```docker build . -t nodejs```;
- go to /db folder and create `mongodb` image by run ```docker build . -t mongodb```;
- run ```docker-compose up -d```.

### Stopping
- run ```docker-compose down```;
- go to /app folder and delete `nodejs` image by run ```docker rm nodejs --force```;
- go to /app folder and delete `mongodb` image by run ```docker rm mongodb --force```;
- if need (checking ```docker ps -a```), delete containers by run ```docker rm {name of container} --force```

### Restart 
- run ```docker-compose up --force-recreate```.

