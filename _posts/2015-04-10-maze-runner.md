---
layout: post
title: "Maze Runner"
description: ""
category: projects
tile_bg: 'maze.gif'
---
<style type="text/css">
    #ui {
        width: 400px;
        height: 100%;
        float: right;
    }
    #theme-table td {
        font-size: 14px;
        height: 30px;
        border: 1px solid #ccc;
        padding: 5px;
        opacity: 0.9
    }
    #theme-table td:hover {
        opacity: 0.2;
    }
    #size-slider {
        float: left;
        margin-top: 50px;
    }
</style>

Hello. I wrote a little visualization of a [maze generation algorithm](http://en.wikipedia.org/wiki/Maze_generation_algorithm). It's pretty maze-merizing!

<div id="p5canvas">

    <div id="ui">
        <table id="theme-table">
            <th>Theme</th>
            <tr>
                <td id="minuet">Minuet</td>
                <td id="bolero">Bolero</td>
                <td id="serenade">Serenade</td>
            </tr>
            <tr>
                <td id="nocturne">Nocturne</td>
                <td id="requiem">Requiem</td>
                <td id="prelude">Prelude</td>
            </tr>
        </table>

        <div id="size-slider">
        <h4 style="width:100%; padding-left:15px; margin:5px; text-align:left;">Size</h4>

        </div>
    </div>

</div>

I originally wrote this in [Processing](https://processing.org/) (which I used to make the background of this website actually), but I thought it was too cool to keep to myself, so I decided to transcoded into [p5.js](http://p5js.org/) so that I can showcase it here. If you are into visuals and have some programming background I recommend looking into the Processing family. You can make some really [cool shit](http://beesandbombs.com/roulette) with it.

There are some plans for more interactive features... maybe later...

P.S. some weird development notes:  

- p5 is pretty neat-o
- delicious copy pasta
- dog doodles + squares
- p5 + coffeescript??? yes? ...!!!
- why do I stay up to do anything anymore.
- \*a really fast dog\* [yes.](https://scottblanton.files.wordpress.com/2012/04/lab_running.jpg)
- pls don't look at the source

<script type="text/javascript" src="/assets/js/maz.js"></script>