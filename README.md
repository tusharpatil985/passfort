Two python projects have been provided to you.

1.) Dice-service
2.) Gateway

To run the above projects you need to perform the below steps:

1.) We are assuming that you are already using Ubuntu OS.
2.) Install Docker for that run Docker.sh script on your machine.
3.) Once docker is installed, run the below commans:
  a.) docker container run -d --name dice-service tusharpatil985/dice
  b.) docker container run -d -p 127.0.0.1:5000:5000 --name gateway --link dice-service -d tusharpatil985/gateway
4.) Run the http://127.0.0.1:5000 in your browser to get the random number.

OR

1.) We are assuming that you are already using Ubuntu OS.
2.) Install Docker for that run Docker.sh script on your machine.
3.) COPY app.py, run.sh and requirements.txt files of dice-service folder at /opt/dice location.
4.) COPY app.py, run.sh and requirements.txt files of gateway folder at /opt/gateway location
4.) Install docker-compose: "sudo apt -y install docker-compose"
5.) Run "docker-compose up"
6.) Run the http://127.0.0.1:5000 in your browser to get the random number.
