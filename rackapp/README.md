# Rack

Ruby Webserver Interface

* Minimal interface between webservers
* A Rack application is a Ruby object that responds to method ```call```. It takes exactly one argument, the environment and returns an ```Array``` of exactly three values: ```status```, ```headers```, and ```body```.

## Input - just one hash

### Environment
* REQUEST_METHOD
* SCRIPT_NAME
* PATH_INFO
* QUERY_STRING
* HTTP_xxx
* rack.version etc.

## Output - array of 3 elements

### Status

* integer >= 100

### Headers

* Content-Type
* Content-Length

### Body

* Array of strings (actually object that responds to each and yields string values)

# Sinatra, Padrino, Rails
# Reverse proxy - nginx
# Ruby webservers - unicorn, passenger, puma