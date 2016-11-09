Overview
========

In this project you will choose three things from a list of improvements for your web site.
Chose from the following list of topics:

1. Hosting on DigitalOcean
    
      Email me for an invite if you you'd like to do this.
    
2. Caching with Redis
    
      Install the Python Redis client https://pypi.python.org/pypi/redis with pip and
      start a Redis docker image such as https://hub.docker.com/_/redis/ .
      
      You can't use Django's caching interfaces to configure whole page caching with Redis without using additonal packages. Instead just directly call the Redis python client to store pages and later look them up. Think about how and when
      to invalidate the cache'd content (after a certain amount of time? when the DB changes? something else?).
    
3. Continuous Integration
    
      
    
4. Integration tests
    
      Write integration tests using Selenium http://www.seleniumhq.org to test your web front end.
    
5. Performance testing
    
      Measure how fast your app will scale. This is a good project to do in combination with #1 above
      to measure how fast it runs on your laptop vs a DigitalOcean VM (it may not be as much different
      as you expect!). I recommend using JMeter http://jmeter.apache.org which is also available via
      a Docker image at https://hub.docker.com/r/hauptmedia/jmeter/ .
    
6. Load balancing
    
      Run multiple instances of your app tiers with a load balancer in front to distribute the load across
      all the instances. For example, if you have two copies of your web front end the load balance will
      sit in front of it, receive connections from browsers, and forward them on to one or the other
      of the web front end instances. 'pen' is a common and relatively simple one and is available 
      as a Docker image at https://hub.docker.com/r/galexrt/pen/ .

Deliverable
===========

Please turn in via email a write up including:

1. describing what you did

2. updated docker-compose.yml if you are running any new or changed containers
 
2. link to any code in github you wrote for this (especially for caching)

3. include any sample output (especially for the load balancer, continuous integration, performance test examples)

4. include any command lines (such as for running load tests, unit tests or load balancers)

5. for hosting on digital island, include a link to your app or service working there

6. Don't forget to provide user stories and unit tests accordingly.
