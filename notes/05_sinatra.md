# Sinatra

* State
  * State is data that persists over time
  * HTTP being stateless, can be thought of as every HTTP request being handled separately
  * Servers can remember things between requests by using techniques that are built on top of HTTP
  * `enable :sessions` allows for sessions in Sinatra
  * `set :session_secret, 'secret'` is necessary because otherwise, Sinatra will set a random `:session_secret` every time the application starts
* Make sure to include a `/` before the URL of any public assets. If you don't, the file will be searched from the current location `.`
* Resource-based URLs
  * The name of the thing being modified is included in the URL
  * Most useful for helping developers guess the URL that accomplishes a certain task
  * Examples:
    * `GET /lists` -> view all lists
    * `GET /lists/new` -> new list form
    * `POST /lists` -> create a new list
    * `GET /lists/1` -> view a single list
