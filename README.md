# multi-docker

local run

docker-compose up --build

endpoint - http://localhost:3050/

Docker Images
=============
razatg/multi-client

razatg/multi-nginx

razatg/multi-server

razatg/multi-worker

Every Push to git4razat/multi-docker will trigger a build CI build on Travis CI, which runs the test cases and generates the above docker images and pushes the same to docker hub. Amazon Elastic Beanstalk will run the containers after Travis initiate the trigger.
