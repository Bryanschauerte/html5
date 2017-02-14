# HTML5

### Semantic elements

- `<nav/>`
- `<title/>`
- `<header/>`
- `<article/>`
- `<section/>`
- `<aside/>`
- `<figure/>`
- `<dialog/>`
- `<footer/>`

Makes reading html much cleaner and easier to scan to appropriate sections.


### Added Attributes
*Ones I found useful so far (biased)*

####Custom 'data-' attributes.

Great way to store data on an element.
Recently used this bad boy to resort an array of removed elements and re-attach them to the dom

`<div id ='html5Container' data-coolness='very' ><h1>yatta yatta</h1></div>`

Accessible with css like so...

`[data-coolness]='very' {
  color: '#ff69b4'
  }`

   or javascript magic
```javascript
var targetElem = document.getElementById("html5Container");
var isHowCool = targetElem.getAttribute('coolness');
```

Yes, you can have multiple.

#### contenteditable(boolean value)

`<p contenteditable="true">I can be edited!<p>`

Pretty much the most useless thing ever. I tired to find just one good use case. So far, just the creating of WYSIWYGs. Other than that, poor api and browsers dont seem to like it either.

#### background
Add an image directly to the background of an element, splash in some style, botta-bing you got a pretty/well sized background.
**Lots of other styling attributes as well**

#### draggable
Make your UI more interactive. Buttons are cool, but dragging a element to a container for input could be really neat. (Build your own pizza, quiz/matching games, editing a shopping cart...)

#### spellcheck
Yeah... That might be handy..

### WebWorkers
#### Helllllo Threading

Run script asynchronously after the file loads. If it fails to load, it dies silently. Goodbye unresponsive script message... Want a thing to be awesome? -> Make your thing a progressive web app... (https://developers.google.com/web/progressive-web-apps/)

## Some other changes that might be helpful to know...
  - Tags can be uppercase now.
  - Attributes values dont have to be surrounded with quotes.
  - Don't need to close empty tags (but.. you totally still should)
  - 'type' on your script/style tag is no longer needed.
