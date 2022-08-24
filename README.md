# scandeepfake_backend
 
## How to deploy a Tensorflow model on Heroku with Tensorflow serving

The serving is done from within a docker container (namely from the tensorflow/serving image). Using any container-orchestration system like docker-compose or Kubernetes will allow you to clearly separate the ml models served with tensorflow from the app or any other services. 

!! Remember Tensorflow serving serves the Rest API over the port 8501 but Heroku assigns a random port when it runs the dyno. !!
