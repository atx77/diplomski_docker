Docker setup for:
- Frontend (Angular + Nginx)
- Backend (Spring Boot)
- MySQL with data dump
- Apache Solr with already indexed data dump

In order to run it (Docker is required):
1 - Clone this repo
2 - Build and start services with:
   docker-compose build
   docker-compose up -d
   
Applications will be available at:
1 - Frontend: http://localhost
2 - Backend: http://localhost:8080
3 - Solr: http://localhost:8983

Various properties can be changed in application.properties file. 
After making changes to application.properties, restart of backend service is required using command:
	docker-compose restart backend

Other useful commands:
- Shut down all services: docker-compose down
- Check status of services: docker ps
- Check logs of service: docker-compose logs -f [service name]

