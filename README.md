# JCMS-Easy-Docker

The JCMSWeb has been an indispensable tool for managing transgenic mice in our
lab. Since Jax Laboratory has stopped supporting JCMS, JCMS-Easy-Docker attempts
to simplify the installation by using Docker, and simplify the daily use by
develop a new web interface.


## Usage

    git clone https://github.com/venklab/JCMS-Easy-Docker.git

Then go to the JCMS-Easy-Docker directory

    docker-compose up

The start up of first run is slow, depends on the network bandwidth,
because docker needs to pull the containers. The container behind new web
interface will install LaTeX from Internet and there are a lots of packages to
download.

After start up, open web browser and go to http://localhost:8080/jcms for
JCMSWeb, the initial account is 'mtsadmin' password 'changeMe'.

Go to http://localhost:8001 for the new web interface.



## Future plan

Port JCMSWeb from Java to other languages that is easier to rebuild, or lighter,
or easier to learn for biologist.
