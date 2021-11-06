# Rack and Sinatra

* Rack
  * Web servers listen to requests and return responses (e.g., `puma`, `WEBrick`)
  * Rack is a generic interface to help application developers connect to web servers
  * The application is referred to as a 'Rack application'
  * Framework aids programmers in building an application
  * Specifications
    * Needs a `rackup` file (`.ru`)
    * Pass an object to the `run` method in the file
    * Object must respond to the `call(env)` method and return 3 elements: status code, headers, and response body
    * `env` gives important information like path or user-agent
    * `erb` is a templating library that allows us to embed Ruby in HTML. Its name comes from embedded Ruby, which is a good description of how it works — by embedding bits of Ruby code into another file.
* Sinatra
  * Sinatra provides conventions for where to place your application code. It has built-in capabilities for routing, view templates, and many other convenient features that you'd otherwise have to code up yourself.
  * But at the core, it's nothing more than some Ruby code connecting to a TCP server, handling requests and sending back responses all in an HTTP-compliant string format. Keep that in mind.
