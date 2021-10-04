# TP Continous Integration

This application is produced in NodeJS and Express.

First, we had to containerize the application using docker.
Then, we had to set up continuous integration. For that, the tp required to use CircleCI.

The behavior of the project was that at each push on the main branch, the CircleCI script was executed.
It installs the application, launches it and tests it. 
If these steps are validated, it pushes directly the docker image of the application on my Docker Hub account. 

You can see it in ```/.circleci/config.yml```.
