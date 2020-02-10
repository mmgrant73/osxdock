[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/owner/my-element)
# OSX Dock:

### What is it?
OSX Dock - is a custom web component which is like the docking bar on the MacOS operation system that can be used on a website.  It is easy to 
use and set up.

![Alt text](https://github.com/mmgrant73/osxdock/blob/master/osxdock.png?raw=true "Image-osxdock")

[Click here for Demo](https://mmgrant73.github.io/osxdock/osxdock.html) 

### How to use it?
It is quite easy to use it on your webpage. Just follow the below steps:

1. Include the link to the script file that holds the this custom web component (osxdock.js) near the bottom of 
   the body section of your webpage.  See below
   
```
    <script src="./osxdock.js"></script>
```

2.  Then use the custom element tags on your webpage.

```
    <osx-dock>
        <item href="www.facebook.com" src="./osxdock/facebook-icon.png">Facebook</item>
        <item href="www.google.com" src="./osxdock/google-icon.png">Google</item>
        <item href="www.github.com" src="./osxdock/github.png">Github</item>
    </osx-dock>
```

Note: That is all you have to do to use this custom element.  There is an example HTML page (osxdock.html) that shows how to use it.

```
    <!DOCTYPE html>
    <html>
      <head>
        <title>OSX Dock Web Component</title>
        <style>
            body {
                background-color: rgb(90,90,90);
            }
            h1 {
                color: white;
                text-align: center;
            }
        </style>
      </head>
      
      <body>
      
        <h1>This is a demostration of the OSX Dock Web Component</h1>

        <div>
            <osx-dock>
                <item href="www.facebook.com" src="./osxdock/facebook-icon.png">Facebook</item>
                <item href="www.google.com" src="./osxdock/google-icon.png">Google</item>
                <item href="www.github.com" src="./osxdock/github.png">Github</item>
            </osx-dock>
        </div> 

        <script src="./osxdock.js"></script>

      </body>
      
    </html>
```

### There are only three properties that you can use to customize this element.

There are three attributes that you need to set:
1. href - is the hyperlink that will become active when a user click on the icon in the dock bar
2. src - is the image that will be used in the dock bar
3. innerText - the innerText between the item tag will be display when the mouse is hovered over the icon

### To Do:
1. Add a way so one can style the dock bar

Note: You have to set the two attributes(href and src) and the innerText. 

Note: This was inspired by something I saw on https://zurb.com/lab.  Some of the CSS was dervied from this site.  
I expanded on it and converted it to a web component
