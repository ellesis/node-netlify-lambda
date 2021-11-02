Node Express web server

# node express - api server

npm init
npm install express --save
make app.js file

npm install nodemon -g

fix package.json

```json
"scripts": {
    "start": "node app.js",
    "dev": "nodemon --watch app.js"
  },
```

# deploy on the netlify

- npm i netlify-lambda serverless-http --save

- Add .gitignore
  /functions

- Create a netlify.toml file
