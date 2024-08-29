# NGINX-CONF
some nginx configuration files
## some benefits of nginx web server
# 1. load balancing
# 2. reverse proxy
# 3. cashing
# 4. host multi sites
# nginx conf blocks 
## main --> 1. events, 2.stream, 3.http

# http block --> 1. server 2. upstream

#   REVERSE PROXY USE CASES BELOW HERE -->
1. Load Balancing
Distribute Traffic: A reverse proxy can distribute incoming client requests across multiple backend servers. This helps balance the load, prevent server overload, and improve overall application availability.
Scalability: By distributing requests, a reverse proxy allows you to scale your infrastructure horizontally by adding more backend servers as needed.
2. Security
Hide Backend Servers: A reverse proxy can obscure the identity and internal structure of backend servers, adding a layer of security by preventing direct access to them.
DDoS Mitigation: It can help absorb and mitigate distributed denial-of-service (DDoS) attacks by spreading the traffic load or blocking malicious requests before they reach the backend servers.
SSL Termination: A reverse proxy can handle SSL encryption and decryption, relieving backend servers of this processing task, thereby improving performance.
3. Caching
Content Caching: Reverse proxies can cache static content (like images, scripts, and stylesheets) to serve subsequent requests more quickly, reducing load on the backend servers and improving response times.
Reduce Latency: By caching responses from backend servers, a reverse proxy can reduce the time it takes to serve client requests, especially for frequently accessed content.
4. Traffic Routing
URL Rewriting: Reverse proxies can route requests to different backend servers or services based on the URL or other request attributes, enabling complex routing rules.
API Gateway: It can act as a central point for routing API requests to different microservices in a microservices architecture.
5. Failover and Redundancy
High Availability: In case of a server failure, a reverse proxy can redirect traffic to healthy servers, ensuring high availability and uninterrupted service.
