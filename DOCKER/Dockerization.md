## Dockerization of reactnative project

#### Dockerfile Code:
```
FROM node:latest


WORKDIR /app
RUN npm install -g expo-cli
RUN npm install -g nodemon


COPY ./myapp/src/App.js /app
COPY ./myapp/src/App.test.js /app
COPY ./myapp/src/index.css /app
COPY ./myapp/src/index.js /app
COPY ./myapp/src/App.css /app
COPY ./myapp/src/reportWebVitals.js /app
COPY ./myapp/src/setupTests.js /app
COPY ./myapp/package.json /app
COPY ./myapp/package-lock.json /app
COPY ./myapp/public/index.html /app
COPY ./myapp/public/manifest.json /app
COPY ./screens/Login.js /app
COPY ./screens/Signup.js /app

RUN npm install 

COPY . /app

CMD [ "expo", "start" ]
```
#### command for creating docker image:
```
docker build -t name_of_image .
```
![image](https://github.com/HimanshuGound/geniehub-assignment/assets/92567932/a304682e-c76a-4c2b-9913-473fba45325a)

#### Creating container with image:
- click the run button:
![image](https://github.com/HimanshuGound/geniehub-assignment/assets/92567932/ea5e82e6-6090-4724-bea8-b82d0c9d7ab6)

- Now the container is ready:
  ![image](https://github.com/HimanshuGound/geniehub-assignment/assets/92567932/6621c814-8aa1-4435-a6f3-a41476f292c5)


