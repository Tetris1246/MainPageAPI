# MainPageAPI
## What is it?
MainPageAPI is a sort of tool for creating your own mainpage with own icons...
## Why it exists
MainPageAPI exists, because some time ago i made [this](https://tetris1246.github.io/) page and after i shared it to my classmates. Everyone wanted just this one link replaced with another and so on. That's the reason i developed this API.
After a quick research i did not find a API like this one. Thats the reason why i published this. 
## How to use it
### The structure
- first you create a folder with a `.html` file. You can call it how you want
- After that, you open the `.html` file and ass these lines:
```
<!DOCTYPE html>
<html>
    <body>
    </body>
    <script src="https://tetris1246.github.io/MainPageAPI/MainPageAPI.js"></script>
    <script>
        let bodyElement = document.getElementsByTagName("body")[0];


    </script>
</html>
```
the `<!DOCTYPE html>` and `<html></html>` tags are only there, because otherwise there would be a error in the console or it would not work at all in some browsers.

the `<body></body>` tag is the container into which the content will later be inserted

`<script src="https://tetris1246.github.io/MainPageAPI/MainPageAPI.js"></script>` implements the api. If you implement it like that, the page only works with internet. If you want to use the page also offline you have to put in the same folder as in wich the `.html` file is, a `.js` file in wich you put [that](../blob/main/MainPageAPI.js) code. Then you put instead of the codepiece above (`<script> src="...`) you write `<script src="theJustCreatedDotJSFile.js"</script>`.

into the other script tag (`<script> </script>`) you put the main code. `let body = document.getElementsByTagName("body")[0];` defines the element, in wich the page goes. in the sample above it's the `body` element.

# Commands
## space();
### syntax:
`space(<space in px>, <body element>);`
### description:
Inserts a space


## customIcon();
### syntax:
`customIcon(<page link>, <image link>)`
### description:
If you want, to change the icon for a page in these commands: `addBigFields()` & `addIcons()`, you can put instead of the link, the `customIcon()` command. The `<image link>` can be the path to a image or `.gif` file or a URL.


##  changeApi();
### syntax:
`changeApi(<api link>);`
### description:
You can use the `changeApi()` command, for chaneging the api, that takes the icons automaticly. As default, the google favicon api is used. But you can add your own api. In the URL, you replace the size of the icon with `{size}` and the URL with `{url}`.


## changeIconResolution();
### syntax:
`changeIconResolution(<size>);`
### description:
If you want to change the resolution of the icons, you can use the `changeIconResolution()` command. Instead of the `<size>` spacer, put the resolution in px. The default is 64.


## addBigFields();
### syntax:
`addBigFields([<link1>, <link2>, <link3>, ...], <body element>);`
### description:
Adds big fields centered to the page. You can add as many icons, as you want. In the syntax above, the URL of the page is specified instead of the `<link...>` spacer. The icon will be taken automatically if you do not use the `customIcon()` function. Instead of the `<body element>` spacer, put the name of the variable defined earlier.


## addIcons();
### syntax:
`addIcons([<link1>, <link2>, <link3>, ...], <body element>);`
### description:
Adds icons centered to the page. You can add as many icons, as you want. In the syntax above, the URL of the page is specified instead of the `<link...>` spacer. The icon will be taken automatically if you do not use the `customIcon()` function. Instead of the `<body element>` spacer, put the name of the variable defined earlier.


## addSearchbar();
### syntax:
`addSearchbar(<specific search engine>, <body element>);`
### description:
Adds a searchbar to the page. Instead of the `<specific search engine>` spacer, you put one of these URLs:
-  www.google.com
-  www.bing.com
-  www.duckduckgo.com
-  de.wikipedia.or
-  www.ecosia.org 

Instead of the `<body element>` spacer, put the name of the variable defined earlier.


## backgroundColor();
### syntax:
`backgroundColor(<color>, <body element>);`
### description:
Replaces the background color of the page. Instead of the `<color>` spacer, put a hex colorcode ([colorPicker](https://tetris1246.github.io/colorPicker/)), that you want. Instead of the `<body element>` spacer, put the name of the variable defined earlier.

## backgroundImage();
### syntax:
`backgroundImage(<image link>, <body element>)`
### description:
Replaces the background image of the page. The `<image link>` can be the path to a image or `.gif` file or a URL. Instead of the `<body element>` spacer, put the name of the variable defined earlier.


If you have questsions, you can send me a message on discord: [Tetris12#5223](https://discordapp.com/users/487130226158075915/)
    