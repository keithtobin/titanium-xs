# Create Openstack Titanium Base Container
#
# Version: 0.0.1
# Desctiption: This DockerFile (http://docs.docker.io/en/latest/use/builder) script is used by docker 
#	       to create the Openstack Titanium Base Container.  	
#

FROM      titanium-base-13
MAINTAINER Keith Tobin <keith.tobin@gmail.com>

ADD ./events/build/build-base /titanium/events/build/build-base
ADD ./events/build/build-mysql /titanium/events/build/build-mysql
ADD ./events/build/build-keystone /titanium/events/build/build-keystone
ADD ./events/build/build-glance /titanium/events/build/build-glance
ADD ./events/register/register-mysql /titanium/events/register/register-mysql
ADD ./events/register/register-keystone /titanium/events/register/register-keystone
ADD ./events/register/register-glance /titanium/events/register/register-glance
RUN chmod 777 /titanium/events/build/*
RUN chmod 777 /titanium/events/register/*
RUN /titanium/events/build/build-base
#RUN /titanium/events/build/build-mysql
#RUN /titanium/events/build/build-keystone 
#RUN /titanium/events/build/build-glance
#RUN /titanium/events/build/build-mysql

