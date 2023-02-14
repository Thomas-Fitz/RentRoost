## Project setup
​
The first thing you'll need to do is to download any dependencies by running this command:
​
```
npm install
```
​
Next take a moment to review the `.env` file that's located in the root of the project. You can store environment variables that you want to use throughout your application in this file. When you open it, it'll look like this:
​
```
# Java
VUE_APP_REMOTE_API=http://localhost:9000
```
​
*Note:* The Java Spring Boot application is configured to run on port 9000 instead of 8080.
​
Start your Vue application with the following command:
​
```
npm run serve
```
