## RabbitMQ test

- Run rabbitmq (using docker)
```
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management
```

- Run the service one
```
cd service-one
```
```
npm i
```
```
node index.js
```


- Run the service two
```
cd service-one
```
```
npm i
```
```
node index.js
```

- GET request to http://localhost:4001/send-msg 

A message is sent from service-one to Queue(names 'test-queue').
The message is read by service-two and logged.