# About

This is a Spring Boot "Hello-World" application which is deployed on OpenShift(minishift) for demo purposes only.

OKD is the Community Distribution of Kubernetes that powers Red Hat OpenShift - https://www.okd.io/
Minishift is a tool that helps you run OpenShift locally by running a single-node OpenShift cluster inside a VM.

https://ashishtechmill.com/running-simple-spring-boot-application-on-openshift

https://github.com/yrashish/springboot-openshift

oc delete all -l app=springboot-kubernetes (remove old application)
oc new-app registry.access.redhat.com/openjdk/openjdk-11-rhel7~https://github.com/bmgitit777/springboot-kubernetes.git
oc logs -f bc/springboot-kubernetes
oc status or oc status --suggest
oc expose svc/springboot-kubernetes
