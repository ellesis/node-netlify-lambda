Node Express web server

# node express - api server

npm init
npm install express --save
make app.js file

## install nodemon and setting

npm install nodemon -g

fix package.json

```json
"scripts": {
    "start": "node app.js",
    "dev": "nodemon --watch app.js"
  },
```

# deploy on the netlify with netlify-lambda, serverless-http

- npm i netlify-lambda serverless-http --save

- Add .gitignore
  /functions

- Create a netlify.toml file

- make folders and files
  /dist/index.html : blank file
  /src/api.js

- npm start
  http://localhost:9000/.netlify/functions/api/
  http://localhost:9000/.netlify/functions/api/test
