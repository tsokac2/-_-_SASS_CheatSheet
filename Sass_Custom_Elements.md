  
## 
### HTML H1 - ::after{} effect
  ```<h1 className="card-heading" as="h3" size="1xl">Title of your component</h1>```
### SASS
```
.card-heading{
    white-space: nowrap;
    overflow: hidden;
    background-color: plum;
}
.card-heading::after {
    margin-left: 25px;
    content: '';
    display: inline-block;
    vertical-align: middle;
    width: 100%;
    height: 1px;
    background: black
}
```
### Browser output
![card-heading](https://github.com/tsokac2/-_-_SASS_CheatSheet/blob/main/wireframes/Responsive_h1_after_element.JPG)
#
