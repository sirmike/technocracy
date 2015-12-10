# Rack

Ruby Webserver Interface
http://rack.github.io/

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
* http://www.sinatrarb.com/
* http://padrinorb.com/
* http://rubyonrails.org/

# Reverse proxy - nginx
* https://www.nginx.com/resources/admin-guide/reverse-proxy/

# Ruby webservers - unicorn, passenger, puma
* http://unicorn.bogomips.org/
* http://www.phusionpassenger.com/
* http://puma.io/
