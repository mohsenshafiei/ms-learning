### Microservices Learning

#### What are Microservices?
- An approach to developing a single application as a suite of small services.
- Each runs on its own process and communicates using lightweight mechanisms, usually using an HTTP based API
- Microservices are built around business capabilities
- Independently deployable, using automated deployment tools
- They are decentralized in nature
- Enables apps to be written by multiple teams using multiple tech stacks

#### Why Microservices?
- Microservices help decrease the cost of change
- Allow for easier integration
- Works very well within a DevOps context

#### Key Difference of Monolithic Apps And Microservices Apps

- Monolithic application:
  * Less modular
  * Scalability is done by scaling entire app
  * Entire language is written in the same language or tech stack

- Microservices application:
  * Each service is its own module
  * Each service is independently scalable
  * Apps can be made up of services in multiple languages or stack

#### Key design principles
- Component as services
- Organization as services
- Product as opposed to projects
- Smart endpoints and dumb pipes
- Decentralized governance


#### Component as services

- components can be made into services in Nodejs very easily using common framework called express
- Using the routing capabilities that express provides, we can create web-based APIs very quickly


#### Products, not projects
- Microservices lend themselves to a product-based approach to software development and maintenance
- This works well for business capability development because developers have an on-going relationship with the software as they continue to develop and improve the application
- Microservices sometimes create new business opportunities using the product-based approach

#### Smart endpoints and dumb pipes

- Microservices own their own domain logic
- They use simple protocols like http and employ a RESTful approach to API management
- Key to creating a Microservice from Monolithic is to change the communication pattern

#### We can use the express framework to easily accomplish this in our code
- Model: Data structures and interfaces for operation on data
- View: The place to manage the way output is rendered
- Controller: The router that controls request and responses

#### Controllers in express
- Controls the routing of the API calls
- Interfaces with the model to work with data (CRUD, and so on)
- Passes responses output to the view
- This is accomplished with express routing

#### Single service per host
- isolates services from others
- Service has exclusive resources
- Easy to monitor and deploy
- Less efficient in some cases than multiple services per host

#### Service instance per container
- Package the service in a docker container
- Scaling is easy by changing the number of container instances
- Encapsulates the tech stack
- Isolate each service

#### Serverless deployment
- Eliminate the need to maintain servers
- Scales according to usage
- These need to be quick and lightweight
- Latency risk
- Pay per request

#### Why Containerization?
- Solves the problem of how reliably move software between environments
- Encapsulates the entire runtime environment
- Includes the application and its dependencies, libraries and other binaries
