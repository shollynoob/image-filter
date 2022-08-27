# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into three parts:
1. [The Simple Frontend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-frontend)
A basic Ionic client web application which consumes the RestAPI Backend. [Covered in the course]
2. [The RestAPI Backend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-restapi), a Node-Express server which can be deployed to a cloud service. [Covered in the course]
3. [The Image Filtering Microservice](https://github.com/udacity/cloud-developer/tree/master/course-02/project/image-filter-starter-code), the final project for the course. It is a Node-Express application which runs a simple script to process images. [Your assignment]

## Tasks

### Setup Node Environment

You'll need to create a new node server. Open a new terminal within the project directory and run:

1. Initialize a new project: `npm i`
2. run the development server with `npm run dev`

### Create a new endpoint in the server.ts file

The starter code has a task for you to complete an endpoint in `./src/server.ts` which uses query parameter to download an image from a public URL, filter the image, and return the result.

We've included a few helper functions to handle some of these concepts and we're importing it for you at the top of the `./src/server.ts`  file.

```typescript
import {filterImageFromURL, deleteLocalFiles} from './util/util';
```

### Deploying your system

Follow the process described in the course to `eb init` a new application and `eb create` a new environment to deploy your image-filter service! Don't forget you can use `eb deploy` to push changes.

## Stand Out (Optional)

### Refactor the course RESTapi

If you're feeling up to it, refactor the course RESTapi to make a request to your newly provisioned image server.

### Authentication

Prevent requests without valid authentication headers.
> !!NOTE if you choose to submit this, make sure to add the token to the postman collection and export the postman collection file to your submission so we can review!

### Custom Domain Name

Add your own domain name and have it point to the running services (try adding a subdomain name to point to the processing server)
> !NOTE: Domain names are not included in AWS’ free tier and will incur a cost.



## My Note


# donwload and install UnxUtils
Register the Path `C:\Program Files (x86)\UnxUtils\usr\local\wbin` in the envirometal variable

# updating environmetal variable
![image](https://user-images.githubusercontent.com/5302985/186998664-d49895ee-1358-4f34-855b-9d130dd69322.png)

![image](https://user-images.githubusercontent.com/5302985/186998864-e785ffd6-29c5-4de1-a2e8-98209269937c.png)

# install PIP using cmdlet 
`pip install awsebcli --upgrade --user`

Register eb cli to enviromental varible using `%USERPROFILE%\AppData\roaming\Python\Python37\scripts`

Runnung `eb create`
![image](https://user-images.githubusercontent.com/5302985/187049071-52534f75-a1ca-47f5-b2a5-242b28b9f266.png)

Elastic Beanstalk Deployed
![image](https://user-images.githubusercontent.com/5302985/187049214-1a6c23c5-2b89-40c1-b22a-51d87b6292af.png)


Test on Postman
![image](https://user-images.githubusercontent.com/5302985/187050303-fa0be19f-bef4-428c-bdb6-3a0c3f1951c8.png)

Github Repo : https://github.com/shollynoob/image-filter

Elastic Beanstack Endpoint :  http://udagram-sola-dev-dev.us-east-1.elasticbeanstalk.com/


Test Image Url : https://cdn.vanguardngr.com/wp-content/uploads/2021/09/Naira-appreciates-1200x720-1-1024x614.jpg

Test url: http://udagram-sola-dev-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://cdn.vanguardngr.com/wp-content/uploads/2021/09/Naira-appreciates-1200x720-1-1024x614.jpg

