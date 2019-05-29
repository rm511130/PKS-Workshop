# PKS-Workshop v05-30-2019
PKS (Pivotal Container Service) - K8s - Kubernetes Workshop on vSphere 6.5

## (1) The History of Containers

[Containers & Orchestration](https://drive.google.com/open?id=1Ly5SAmlZLFyoXC8btFIqfLnvvkRwq4ET)

## (2) Quick Test for Comparison Purposes

Assuming that 
1. you have access to a PAS environment (e.g. https://run.pivotal.io or [cf dev](https://pivotal.io/platform/pcf-tutorials/getting-started-with-pivotal-cloud-foundry-dev/introduction))  
2. you have the [CF CLI](https://github.com/cloudfoundry/cli#installers-and-compressed-binaries) installed on your machine and 
3. you know how to `cf push` App 
4. you have already performed the `cf api` and `cf login` comamnds to target an Org and a Space

Workshop Steps:

1. `$ mkdir -p /work/pas; cd /work/pas; curl -k http://chess.cfapps.io > index.php; cf push chess`
2. Using the route provided in the output of the `cf push` command, please verify that your App is running

What have we learned:

1. A single `index.php` file was enough for PAS, using its buildpack process, to run your App in a container
2. The curated container image creation, instantiation, orchestration, routing, logging, health-monitoring & management were all performed by PAS
