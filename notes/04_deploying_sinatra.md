# Deploying Sinatra

* Puma is more production-ready, as it can handle more than one request at a time using a single process. WEBrick is more appropriate for development
* Files
  * The `config.ru` file tells the web server how to start the application
  * The `Procfile` tells Heroku which processes should be started when the application boots up
* Environment variables
  * Appropriate for storing configuration information that is specific to a production environment.
  * Used to store sensitive information that you may not want to store in the application repository
