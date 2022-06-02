Node Express and netlify-lambda web server

# node express - netlify-lambda, serverless-http

npm init
npm install express --save

make src/api.js file

## install nodemon and setting

npm install nodemon -g

- fix package.json

```json
  "scripts": {
    "start": "./node_modules/.bin/netlify-lambda serve src",
    "build": "./node_modules/.bin/netlify-lambda build src"
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

- deploy url (netlify)
  https://ellesis-api.netlify.app/.netlify/functions/api/
