# Udacity Image Processing API

This is an API that serves two different purposes. As a simple placeholder API, It allows the user to place images into the frontend with the sizes set via URL parameters for rapid prototyping. It can also be used as a library to serve properly scaled versions of user images to the frontend to reduce page load time. Rather than needing to resize and upload multiple copies of the same image to be used throughout the site, this API will handle resizing and serving stored images for the user.


## Project setup
```
Scripts

    npm run build - build the project
    npm start - start the build
    npm run dev - start the server in development mode
    npm test - run the tests

Now you need to install the dependencies for the server code.

### Install all dependencies using the package.json file

```bash
npm install
```

### Lint the code using Eslint

```bash
npm run lint
```

### Format the code using Prettier

```bash
npm run format
```

### Build and Test the app using Jasmine

```bash
npm run test
```

### Now that everything is set up, you can test the app by starting the server using nodemon

```bash
npm run dev
```
 
##### Usage:
To use the Image Processor API, send a request to the endpoint with the following query parameters:

**filename** : The filename of the image file to process as stored under assets

**width** : The intended width of the image file to be returned

**height** : The intended height of the image file to be returned

###### Example - http://localhost:5000/api/images?filename=palmtunnel&width=500&height=500


Once the application is running, a sample front-end page can be viewed - http://localhost:5000/ - which displays image thumbnails with varying sizes.



#####Dependencies

Jasmine: npm i jasmine Jasmine spec reporter: npm i jasmine-spec-reporter Express: npm i express Sharp: npm i sharp Supertest: npm i supertest

    Jasmine: npm i jasmine
    Jasmine spec reporter: npm i jasmine-spec-reporter
    Express: npm i express
    Sharp: npm i sharp
    Supertest: npm i supertest

##############devDependencies

    Prettier: npm i --save-dev prettier
    ESlint: npm i --save-dev eslint
    ESlint config prettier: npm i --save-dev eslint-config-prettier
    ESlint plugin prettier: npm i --save-dev eslint-plugin-prettier
    Typescript: npm i --save-dev typescript
    TS Node: npm i --save-dev ts-node
    Node types: npm i --save-dev @types/node
    Jasmine types: npm i --save-dev @types/jasmine
    Supertest types: npm i --save-dev @types/supertest
    Express types: npm i --save-dev @types/express
    Nodemon: npm i --save-dev nodemon
    Sharp types: npm i --save-dev @types/sharp



##### Error messages:

___401 Bad Request___:  query parameters are missing, invalid or cannot be determined

___404 Not Found___:  image file could not be found or does not exist under assets
