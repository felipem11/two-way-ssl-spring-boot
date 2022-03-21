# 2 way SSL with spring boot

Example client (nt-gateway) and service (nt-ms) code to show how to get 2 way SSL setup with self signed certificate.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

* Java 1.8
* Spring boot 2.1.2
* Java keytool utility


### Installing

Download nt-gateway and nt-ms projects in to your STS or Eclipse workspace.
https://medium.com/@niral22/2-way-ssl-with-spring-boot-microservices-2c97c974e83
keytool -importkeystore -srckeystore nt-ms.jks -destkeystore nt-ms.p12 -srcstoretype JKS -deststoretype PKCS12 -srcstorepass nt-service -deststorepass nt-service -srcalias nt-ms -destalias nt-ms -srckeypass nt-service -destkeypass nt-service -noprompt


keytool -importkeystore -srckeystore nt-gateway.jks -destkeystore nt-gateway.p12 -srcstoretype JKS -deststoretype PKCS12 -srcstorepass nt-gateway -deststorepass nt-gateway -srcalias nt-gateway -destalias nt-gateway -srckeypass nt-gateway -destkeypass nt-gateway -noprompt