# MyApp

- A simple Web application named `MyApp` with three different components based on `go`, `nodejs with typescript` and `wordpress with php`
- In this Repository, we are going  setup Continuous Integration (CI) and Continuous Delivery/Deployment (CD) for these components individually

**Tools Used**

- Version Control system : Git
- Source Code Repository Managment tool : Github
- Containerization: Docker
- Container Orchestration: Docker Compose
- Continuous Integration and Continuous Delivery (CI/CD) : Jenkins / GitHub Actions

- Implemented Linting, unit testing in the CI workflows as part of code standards.


## local setup

### pre-requisites

The following applications should be installed in your system to work on this project. You can verify installation using below commands

`go --version`  if you don't have installed then use this [Go official installation documentation](https://go.dev/doc/install)

`node --version` if you don't have installed then use this [Node official documentation](https://nodejs.org/en/download/package-manager)

`php -v` if you don't have installed then use this [PHP official Documentation](https://www.php.net/downloads)

`docker --version` if you don't have installed then use [docker installation](https://docs.docker.com/engine/install/)

Clone the source repository 👇

```
git clone https://github.com/charan-happy/MyApp.git
cd MyApp
```
Start the services using below command 👇
`docker-compose up`

### Access Services

go at `http://localhost:8080`
![image](https://github.com/charan-happy/MyApp/assets/89054489/dd74bfa1-bd37-418b-ac02-3262e8478cfe)

nextjs at `http://localhost:3000`
![image](https://github.com/charan-happy/MyApp/assets/89054489/5c12040c-2adf-4acb-b7b0-5e9ff92694a2)


wordpress at `http://localhost:80`
![image](https://github.com/charan-happy/MyApp/assets/89054489/b557d690-5a13-435e-8f40-77b4238b9223)


Thanks for following along till now.

Please reachout to me at `nagacharan4286@gmail.com` in case of any queries.

