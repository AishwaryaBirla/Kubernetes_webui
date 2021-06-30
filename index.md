## Kubernetes Integration with python CGI

Task- Portal to run kubernetes commands

## Kubernetes- 
Kubernetes, also known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications.

### Advantages of kubernetes- 
1. Automated rollouts and rollbacks
2. Service discovery and load balancing
3. Storage orchestration
4. Secret and configuration management
5. Automatic bin packing
6. Batch execution
7. IPv4/IPv6 dual-stack
8. Horizontal scaling
9. Self-healing
10. Designed for extensibility

## HTTPD-
The Apache HTTP Server Project is an effort to develop and maintain an open-source HTTP server for modern operating systems including UNIX and Windows. The goal of this project is to provide a secure, efficient and extensible server that provides HTTP services in sync with the current HTTP standards.

The Common Gateway Interface, or CGI, is a set of standards that define how information is exchanged between the web server and a custom script.
CGI can be easily created using cgi-bin of httpd. The files which has permission in server to be executed are made executable and put in folder- /var/www/cgi-bin 

After seting up the webserver, Test the working using the url(http://<instance_ip>/kub.html) in any browser- Here are sample inputs and the output obtained from the server over kubernetes cluster. 

1. First screen that appears-
   ![Sample Output](1.png)
2. Executing a command to run pod with podname "pod1" and "httpd" image
   ![creating pod](2.png)
3. Creating a deployment with name "pod1" and using "httpd" image
   ![creating deployment](3.png)
4. Exposing the deployment "pod1" on port 80 using NodePort type
   ![exposing deployment](4.png) 
5. Scaling the depolyment "pod1" with 3 replicas
   ![scaling deployment](5.png)
6. Deleting everything
   ![Deleting](6.png)
