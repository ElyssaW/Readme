# GITHUB MARK DOWN FOR NODE.JS

Here is how you get started with Node.js

## Install Node

Open command line

1. brew update

2. brew install node

3. node -v

## Github Repo Init

1. Install Node.js

I did this once and promptly forgot how to do it. Good luck.

2. Create Directory Folder

Create a directory folder using the mkdir command in terminal, and cd into it

3. Initialize node

Initialize Node.js in the file by writing npm init, or nopm init -y if you'd like to speedrun the settings process

4. Create modules

Fill in the file with modules you'd like to run

5. Run modules

You can run a module using Node by writing node [filename].js

## Calling New Modules

But wait! Do you want to call in new modules to whatever you're running with . How do we do that?

1. Add code to exports

In the Javscript file you'd like to export, create a module.exports object, and using
dot notation, add any code you'd like to export to it. For example:

* module.exports.beBasic = () => console.log("That's so fetch!")

This, when exported, will allow you to import an object containing the BeBasic function, and thereby allowing you to run that function whenever you'd like, similar to Math.floor() and Math.random()

2. Import the module

You have to bring the module into the Javascript file that you wish to use it in by using import. Include this code in your destination file:

* `const myModule = require('./myModule.js')`

This will search for the Javascript by the file name, and import it into the Javascript file, assigning it to myModule variable. The code can then be called by writing `myModule.beBasic` (Or myModule.[Whatever the function name is.])

## Install Modules

You can use NPM to download new modules from the internet and beyond (Or just the internet.) YOu can do this by opening the target directory in command line and writing

* `npm i [module name]`

You can use -g to install packages globally, by generally that's not

# Express.js

Initialize node with npm, initialize nodemon with nodemon, install express with node i express.

In your Javascript, import express with `const express = require('express.js')`

Instantiate your server with `let app = express()`

Listen to your choosen port with `app.listen([port name])`

Send responses with `app.get('[url], (req, res) => {
    res.Send([response])
}')`

OR

`app.get('[url], (req, res) => {
    res.SendFile(__dirname+'[relative file path to html]')
}')`