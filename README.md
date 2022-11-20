# MongoDB Express React Node - (MERN) Typescript Template

## Backend

<!-- Create a directory for the backend -->

mkdir backend  
cd backend

<!-- Initialize the project -->

npm init -y

<!-- Create a directory for the source files -->

mkdir src

<!-- Create a file for the App -->

touch src/app.ts

<!-- Install the dependencies -->

npm i express dotenv cors mongoose http-errors

<!-- Install the devDependancies -->

npm i -D typescript ts-node nodemon @types/express @types/cors @types/mongoose @types/node @types/http-errors

<!-- Initialize the Typescript config file -->

npx tsc --init

<!-- Add dev and start script -->
In package.json  
"scripts": {  
    "test": "echo \"Error: no test specified\" && exit 1",  
    "dev": "nodemon ./src/app.ts",  
    "start": "npx tsc && node ./dist/app.js"  
  },  
  
<!-- Edit the tscofig -->
In tsconfig.json. 
"module": "commonjs"  
"rootDir": "./src"  
"moduleResolution": "node"  
"outDir": "./dist"  
"include": ["./src"]  

<!-- Create directory for the Model, Controller and Routes Folder -->

mkdir src/models
mkdir src/controllers
mkdir src/routes

## Frontend

<!-- Install Create React App using npx with Typescript template -->

npx create-react-app frontend --template typescript
