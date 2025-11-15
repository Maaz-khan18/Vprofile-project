# Vprofile-project
# *Overview*
Vprofile is a multi-tier web application designed to simulate a production-grade deployment environment. It integrates several open-source services to demonstrate real-world DevOps practices, including service orchestration, configuration management, and infrastructure automation.

# *Architecture*
The application follows a layered architecture with the following components:
| *Service*     | *Role*                                              |
-----------------------------------------------------------------------
| MySQL         | Relational database for persistent storage          | 
| Memcache      | In-memory caching to reduce DB load                 | 
| RabbitMQ      | Message broker for asynchronous communication       | 
| Tomcat        | Java-based application server hosting backend logic | 
| Nginx         | Web server and reverse proxy for frontend access    | 
| ElasticSearch | Search and indexing engine for fast queries         | 

# *Setup Order*
To ensure proper dependency resolution, services should be provisioned in the following order:
- MySQL – Database Service
- Memcache – DB Caching Service
- RabbitMQ – Broker/Queue Service
- Tomcat – Application Service
- Nginx – Web Service
- ElasticSearch – Optional Search Service

# *Tech Stack*
- Backend: Java (Spring), Tomcat
- Frontend: JSP, HTML/CSS
- Database: MySQL
- Caching: Memcache
- Messaging: RabbitMQ
- Search: ElasticSearch
- Web Server: Nginx

# *Learning Objectives*
- Understand multi-tier application architecture
- Practice service orchestration and dependency management
- Deploy services using tools like Vagrant
- Simulate CI/CD pipelines and infrastructure automation
- Explore monitoring and logging integrations
