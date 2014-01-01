# Create Openstack Titanium Base Container
#
# Version: 0.0.1
# Desctiption: This DockerFile (http://docs.docker.io/en/latest/use/builder) script is used by docker 
#	       to create the Openstack Titanium Base Container.  	
#

FROM      ubuntu
MAINTAINER Keith Tobin <keith.tobin@gmail.com>

ADD ./events/build/create-base-container-01 /titanium/events/build/create-base-container-01
RUN chmod 777 /titanium/events/build/*
RUN /titanium/events/build/create-base-container-01
 


