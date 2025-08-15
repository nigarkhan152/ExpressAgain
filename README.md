# ExpressAgain

Let start with the basic understanding of how to setup for node project 
In this , you will get to know all the basic setup information, and environment, because basic is important, let start will the backend tutorial , using node, express & mongodb
let start with installing some packages 
1) npm init -y (for node packages)
2) npm i express (installing express.js)
3) npm i ejs

After installing  these packages you will get a directory named node_modulus(you dont have to worry about that)
and also two file package.json and package_lock.json 
once you get these files on your code editor, create a file name it as index.js to your main root
and write the boiler plate of to setup server

const express = require('express')
const app = express()
const path = require('path')

app.use(express.json())
app.set('view engine','ejs');

app.get("/",function(req,res){
  res.render("index.ejs");
})
app.listen(3000,function(){
  console.log("Its running")
})
