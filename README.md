# Full-Stack Aplication with SpringBoot and Angular

## Create Spring application template
* https://start.spring.io/

## Running application from command line
### Build Spring Boot Project with Maven: 
* mvn install or mvn clean install

### Run Spring Boot app using Maven:
* mvn spring-boot:run
* Spring-boot running on http://localhost:8080/

## Endpoints can be tested with Postman using GET
* http://localhost:8080/api/v1/bikes
* http://localhost:8080/api/v1/bikes/{id}

## Creating Database with sqlite3 (https://github.com/dlbunker/ps-spring-boot-and-angular/tree/master/sql)
* sqlite3 bike.db
* sqlite> .help
* sqlite> .tables

## Angular packageManager
* ng config -g cli.packageManager yarn

## Angular create new project in bike folder and add routing switch to project
* ng new bike-ui --routing=true
* Stylesheet use CSS
* cd bike-ui
* ng v
* npm start runs on http://localhost:4200/

## add proxy URL in SpringBoot server Angular endpoint
* http://localhost:4200/server/api/v1/bikes

## Create bike service in bike-ui
* ng g service services/bike

## Create admin component in bike-ui 
* ng g component components/admin

## show bikes on browser after creating components
* Network bikes service show http://localhost:4200/server/api/v1/bikes
* Preview shows JSON payload
* http://localhost:4200/admin

## Create components home component in bike-ui 
* ng g component components/home

## Create view-registration component in bike-ui 
* ng g component components/view-registration

## Angular dependencies
* npm install bootstrap@4.0.0-beta.2 --save
* npm install @angular-devkit/core --save
* npm install express-http-proxy --save
* npm install cors --save
* npm install port --save

## Make production buil with Angular CLI and run DEV server
* ng build --prod
* node server.js