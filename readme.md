# Minesweeper

##Overview

A simple API to include the classic **minesweeper** game in your web apps. With customization options, you can set the grid size, number of mines etc. - all that within a file of size ~ 6KB.

Demo links : 
[View it on surge.sh](https://boring-minesweeper.surge.sh/)

## Usage

#### Dependencies

The API uses [jQuery](https://github.com/jquery/jquery) for DOM manipulations and [Ben Alman's Tiny Pub Sub](https://github.com/cowboy/jquery-tiny-pubsub) to publish and subscribe to events/topics.
Include these ```script``` tags within the ```head``` tags.

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-tiny-pubsub/0.7.0/ba-tiny-pubsub.min.js"></script>
```

