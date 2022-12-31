<h1 align="center">SASS PRE-PROCESSOR</h1>

### COMPILER IMPLEMENTATION:

* Open Command Prompt
* Navigate to the root project folder
* Enter commands in the following:
* ```npm init --yes```
* ```npm i -g node-sass```
* In {} package.json file under the ```"scripts"``` type the following:
```
"scripts": {
    "watch": "node-sass -o assets/css assets/scss/index.scss -w"
},
```

* To start SASS Compiler enter the following command: ```npm run watch```
* If no errors the compilation process NPM SERVER will start with the following console log message:
```
> new@1.0.0 watch C:\Users\Tomislav\Desktop\new
> node-sass -o assets/css assets/scss/index.scss -w
```

More info [HERE](https://sass-lang.com/)