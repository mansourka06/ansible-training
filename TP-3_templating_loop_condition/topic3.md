# TP3 templating loop & conditions

## What is done in this topic :

- Create a cluster (1 ansible and 1 client) and retrieve the webapp code stored on github

- Create a templates folder containing an index.html.j2 file that will display the following on the site


- **Create the deploy.yml playbook**:
    * use loops to install git and wget using the yum module
    * Use a condition to install wget and git only if we're on a CentOS system.

- Modify the default website, by copying an index.html.j2 template which should display "welcome to -hostname-" -hostname.html.j2
hostname-" -hostname- being retrieved from variables provided by ansible

- Modify the deployment of the apache container so that it mounts the index.html file in the directory in which it

- read the website by default (see the apache Doc on Dockerhub), you'll be using the notion of mounting a
volume

- **Check that your site conforms to expectations**
