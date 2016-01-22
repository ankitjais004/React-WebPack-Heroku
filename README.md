# React-WebPack-Heroku
Motive of this repository:- This is just a simple app to be deployed on heroku.

###Basic environment required: 
1. node 4.x
2. npm 2.14.x
3. ReactJs
4. Webpack
5. Heroku Account 
6. Express

#####ReactJs:
It is a *javascript* library. For more learning pls visit <https://facebook.github.io/react/docs/tutorial.html>
#####Webpack: 
It is a module bundler. It creates a single *bundle.js* file which contains all the stuffs needed. It is then added to intex.html file inside script tag.

Important points to be kept in mind while writing wepback config file for production:-

* We can make two separate config files for development and production. Here we'l only consider the production configuration.
* In *package.json* we have to include
"scripts": {
    "deploy": "webpack --config ./webpack-production.config.js --progress --colors",
    "start": "node server.js"
  } & "engines": {
    "node": "4.x",
    "npm": "2.14.x"
  }

* Dont forget to add webpack inside dependency.

For more learning pls visit <https://survivejs.com/webpack_react/webpack_and_react> & <https://webpack.github.io/docs> 

#####Express:
We are using node js' express framework to run our application.

##### Heroku:
* To deploy our app in heroku we first have to make an account on heroku and login.
* npm run deploy
* git push heroku master

I have deployed this simple App on heroku--> <https://peaceful-wildwood-12514.herokuapp.com>

