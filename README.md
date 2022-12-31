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

More info **[CSS with superpowers](https://sass-lang.com/)**

### SASS IMPLEMENTATION AND FOLDER STRUCTURE

#### Create the following folder structure:
* ```assets/scss/abstracts``` - global SASS variables and mixins function
* ```assets/scss/base``` - global styles for html, body and special helper classes
* ```assets/scss/components``` - carousel image slideshow, small screen navigation menu
* ```assets/scss/layout``` - styling for HOME, TRIP, WORK, LIFE, TIPS, SIGN UP, LOGIN
* ```assets/scss/_index.scss``` - referencing all ```*.scss``` files in folder structure:
```
@import "abstracts/variables";
@import "abstracts/mixins";
@import "base/base";
```
* SASS RESPONSIVE Mixins function:
```
@mixin response($breakpoint) {
    @if($breakpoint == md) {
        @media(min-width: 768px) {
            @content;
        }
    }
}
```
* All files in the above folders MUST be named with the following naming conventions: ```_filename.scss```