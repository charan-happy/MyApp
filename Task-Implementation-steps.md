
## 1. Create a GitHub Repository
- Go to GitHub and create a new public repository named MyApp.
- Clone the repository to your local machine:
  [I used githu codespaces instead of local machine]
  `git clone https://github.com/charan-happy/MyApp.git`

- Inside the MyApp repository, create directories for each component
```
   cd MyApp 
   mkdir go-app nextjs-app wordpress-app
```

## 2. Initialize Repositories for Each Component
**Go Application**
```
cd go-app
go mod init go-app
touch main.go
git add .
git commit -m "Initialize Go application"
git push origin main

```
**nextjs application**
```
cd ../nextjs-app
npx create-next-app@latest --typescript .
git add .
git commit -m "Initialize Next.js application"
git push origin main

```
**wordpress application**
```
cd ../wordpress-app
touch index.php
git add .
git commit -m "Initialize WordPress application"
git push origin main

```
## 3. Implement Continuous Integration (CI) Workflows
- Created CI workflows .you can find same in `.github/workflows` directory
- for go application `go-app.yml` for nextjs application `nextjs-app.yml` and for wordpress application `wordpress.yml`

- we can achieve same in jenkins too. But , in jenkins we have setup pipelines in the UI. click on `new-item` and job name has to give then select job type as pipeline and follow the instructions thereafter as per our convenience.

## 4. Enforce Coding Standards
- Adding linters and unit testing as part of coding standard enforcement

## 5. Dockerize Each Application
- we wrote dockerfile for each component individually to dockerize the applications

## 6. Push Docker Images to a Container Registry
- To access the images we are pushing them to docker hub each component individually
Below are the commands to build and push images to docker hub registry

 ```
docker build -t your-username/go-app ./go-app
docker push <your-dockerhubusername>/go-app
docker build -t <dockerhub-username> /nextjs-app ./nextjs-app
docker push <your-dockerhub-username>/nextjs-app
docker build -t <your-dockerhub-username>/wordpress-app ./wordpress-app
docker push <your-dockerhub-username>/wordpress-app
  ```

## 7. Docker Compose Configuration
- As part of orchestration of all the services, we are using docker compose

## 8. Continuous Deployment (CD) Pipeline

- we have Extended CI workflows to include deployment stages.


### Problems Faces
- Installating dependencies and Ci workflows implementation part i faced difficulties and later by making use of internet i can able to fix them .

  
