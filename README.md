# Customized deployable architecture

Based on https://github.com/IBM/customized-deployable-architecture

## Tutorials
This repository contains tutorials that step through the concept of a deployable architecture, how to develop one, how to customize an existing one found in the IBM catalog, and more.  The tutorials are 
a work in progress and are continually being improved upon.  Tutorials so far include:
-  [deployable architecture overview](./da%20customization%20tutorials/0%20-%20da%20overview/)
-  [basic depployable architecture customization](./da%20customization%20tutorials/2%20-%20basic%20da%20customization/)

## Example customized deployable architectures
This repository contains deployable architectures.

The first is an [example of a customization](./solutions/custom-slz) of the IBM deployable architecture [VSI on VPC landing zone](https://cloud.ibm.com/catalog/architecture/deploy-arch-ibm-slz-vsi-ef663980-4c71-4fac-af4f-4a510a9bcf68-global).  This customization is a minor customization but illustrates how easy it is accomoplish making a change that is suited to a particular need.  The customized deployable architecture still deploys a base networking layer with a Virtual Private Cloud but is now limited to the 'us-east' IBM Cloud region.   

![Custom topology](/images/baby-slz.svg)

## This example shows how:  


1. Create a custom deployable architecture and deploy it as a custom tile to the IBM cloud catalog.
1. Create a custom extension that extends the custom deployable architecture (based on the IBM VSI module) to deploy an Apache server.
1. create a pipeline that will publish the custom architecture and apache server as private solutions on the IBM public catalog.

![CustomTile](/images/custom-tile.png)


Catalog tiles:

* custom-deployable-arch is a generic deployable architecture for the network landscape.
