### Comments on this repository ###
As you read the code you will find that the comments address each of the requirements requested on the task. For example:

	# All HTTP requests should permanently redirect to their HTTPS equivalent
        return 301 https://$host$request_uri;


### About Part 2 missing requirements ###

The following requirement was addressed as follows:

	# " The app service should not reachable directly from the host and can only be accessed through the Nginx service."

By using `firewall-cmd`, the testing host was running CentOS8

  `firewall-cmd --remove-port=8000/tcp --permanent`
  
  `firewall-cmd reload`

Since Docker uses its own zone, dropping TCP traffic on port 8000 from the public zone should address the requirement.

### About this app ###

The task can be tested by running:
`docker-compose up`

and visiting localhost on a web browser, or alternatively `curl -k https://localhost`
