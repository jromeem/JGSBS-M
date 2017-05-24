---
layout: post
title: "p5js Community Video"
description: ""
category: projects
tile_bg: 'p5asters.gif'
---
<style type="text/css">
    #p5canvas { margin: 0; }
</style>

Spinning asterisks!

So I made this specific sketch for p5.js’s community statement video project.

This video project was created as a result of the first p5.js Contributors Conference. From what I understand, each participant of the conference was filmed reciting a short section of the community statement in front of a green screen. The idea was to compile each section tied with a different p5js sketch in the background, hence the green screen.

I was assigned the last section of the community statement in which Lauren McCarthy and Liu Chang (?) are reciting the last bullet in the community statement: “in the future: the future is now.”
My sketch incorporates p5.js’s mascot/logo, the pink asterisk, which can be seen throughout the p5.js website. When you click or press any key on the sketch, the asterisks randomly regenerates into different colors and different positions within the p5's thematic color palette.

On an interesting note, finding the LCM for all the different speeds of spins in order to achieve a perfectly looping gif was pretty difficult at first. But after reducing the speeds to four possible integers and realizing that a perfectly looped asterisk only has to spin 72 degrees to repeat again, really helped me out. Yuck factorization! Yay math!

Anyway, I hope you like it!

<div id="p5canvas"></div>

&nbsp;

<script type="text/javascript" src="/assets/js/comm.js"></script>
