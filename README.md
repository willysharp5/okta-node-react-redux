# User authentication application with Node OKTA react redux
 
User aAuthentication application to perform registration, login, logout and change password functionality using node, react with redux and [OKTA](https://www.okta.com/)

# Deploy
Deploy server and client separately and follow these steps for heruko git deploy 

#### Update Proxy in client package.json for heroku
"proxy": "https://secret-garden-64853.herokuapp.com",

### For local
"proxy": "http://localhost:3001",

#### Client 
* create static.json file and add 

```js
{
    "root": "docs/",
    "routes": {
      "/**": "index.html"
    }
}
```

* git init
* git add .
* git commit -m "Inititalize Code"
* heroku create okta-react-redux --buildpack https://github.com/mars/create-react-app-buildpack.git
* git push heroku master

#### Server 
* git init
* git add .
* git commit -m "Inititalize Code"
* heroku create node-server-react
* git push heroku master


#### Push to Github
git remote add github  https://github.com/willysharp5/node-okta-react-redux.git
git push -u github  master



