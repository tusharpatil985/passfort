Two python projects have been provided to you.

1.) Dice-service
2.) Gateway

To run the above projects you need to perform the below steps:

1.) We are assuming that you are already using Ubuntu OS.
2.) Install Docker for that run install-docker.sh script on your machine.
3.) Once docker is installed, run the below commans:
  a.) docker container run -d --name dice-service tusharpatil985/dice
  b.) docker container run -d -p 127.0.0.1:5000:5000 --name gateway --link dice -d tusharpatil985/gateway
4.) Run the http://127.0.0.1:5000 in your browser to get the random number.

OR

1.) We are assuming that you are already using Ubuntu OS.
2.) Install Docker for that run install-docker.sh script on your machine.
3.) Run "docker-compose up"
4.) Run the http://127.0.0.1:5000 in your browser to get the random number.
