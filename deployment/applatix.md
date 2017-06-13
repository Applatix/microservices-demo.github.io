---
layout: default
---

## Sock Shop on Applatix

The following instructions will help you deploy and run the Sock Shop application on Applatix. 




### Pre-requisites


1. Have an [AWS Account](https://console.aws.amazon.com)
2. Sign up for [Applatix](https://pages.applatix.com/acton/media/25513/contact-us-for-a-free-trial-of-applatix)
3. Deploy one or more Applatix Kubernetes clusters in your AWS account

### Deployment

Applatix is driven by YAML DSL. You'll find the YAML deployment specs of all the Sock Shop microservices under **deploy/applatix** folder.
2. Once Applatix cluster is installed, integrate it with the github repo and under **Catalog** menu item you will see a **sock shop** app.
3. In Applatix, for the stateful microservices create EBS volumes with the names **sock-shop-order-db**, **sock-shop-user-db**, **sock-shop-cart-db**, **sock-shop-cart**,  **sock-shop-shipping**,  **sock-shop-order**.
4. Deploy sock shop from the Applatix **Catalog**.

It will take 1-2 minutes to deploy and you can see all the services in the web console.


### Using

* You can access the Sock Shop front-end service in a browser 

### Tracing

[Zipkin](http://zipkin.io/) has been used in some of the services. While the services are running you can view the trace.

### Starting, Stopping, Terminating

You can start, stop, terminate sock shop from the Applatix web console.

### Uninstalling Applatix

You can uninstall the Applatix cluster from the Applatix SaaS portal in one click or you can manually delete it from your AWS account.
