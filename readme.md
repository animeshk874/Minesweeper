# Minesweeper


## Overview

A simple API to include the classic **minesweeper** game in your web apps. With customization options, you can set the grid size, number of mines etc. - all that within a file of size ~ 6KB.

Demo links : 

* [View it on surge.sh](https://boring-minesweeper.surge.sh/)
* [View it on Codepen](https://codepen.io/animeshk874/pen/wXQGrZ)


## Usage

#### Dependencies

The API uses [jQuery](https://github.com/jquery/jquery) for DOM manipulations and [Ben Alman's Tiny Pub Sub](https://github.com/cowboy/jquery-tiny-pubsub) to publish and subscribe to events/topics.
Include these ```script``` tags within the ```head``` tags.

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-tiny-pubsub/0.7.0/ba-tiny-pubsub.min.js"></script>
```


#### Markup

Create a ```div``` that will act as a container for the Minesweeper grid.

```html
<div id="mine-container"></div>
```


#### CSS

Optionally, you can set the width of the container div uisng CSS.

```CSS
#mine-container{
    width: 500px;
    max-width: 95%;
}
```


#### JavaScript

First, clone/download this repo in your project's folder and then include the ```mines.min.js``` file in your web app.

```html
<script src="./Minesweeper/mines.min.js"></script>
```

Then, initialize the game by making a call to the *Minesweeper()* function and passing the customizations that you want as a parameter.

```html
<script>
    Minesweeper({
        size: 8,
        minesCount: 10,
        elementId: "mine-container",
        flagIcon: "https://boring-minesweeper.surge.sh/Minesweeper/images/flag.png",
        mineIcon: "https://boring-minesweeper.surge.sh/Minesweeper/images/mine.png"
    });
</script>
```

The parameter being passed is an object with the following properties -:
* **size** (optional) - Specifies the size of the grid (8x8 in this case). Default value - 8.
* **minesCount** (optional) - Specifies the number of mines in the grid (10 in this case). Default value - 10.
* **elementId** (mandatory) - Specifies the **id** of the DOM element that contains the game (```mine-container``` in this case).
* **flagIcon** (optional) - Specifies the image that is to be used as flag icon.
* **mineIcon** (optional) - Specifies the image that is to be used as mine icon.


## Demo

* [View it on surge.sh](https://boring-minesweeper.surge.sh/)
* [View it on Codepen](https://codepen.io/animeshk874/pen/wXQGrZ)