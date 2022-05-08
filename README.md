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

