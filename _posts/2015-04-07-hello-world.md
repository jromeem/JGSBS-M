---
layout: post
title: "Hello (p5) World"
description: ""
category: projects
tile_bg: 'welcome.png'
---
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean auctor arcu ut ipsum placerat auctor. Integer nec auctor diam. Vivamus convallis risus vel rhoncus porttitor. Etiam consequat ante eu lorem finibus, ac interdum quam posuere. Etiam vel ultricies felis. Donec sodales risus iaculis turpis ultricies fringilla. Proin risus urna, suscipit eu purus ultrices, convallis pulvinar eros. Pellentesque sed felis cursus, feugiat tellus quis, efficitur est.

Vestibulum pellentesque vestibulum hendrerit. Integer tincidunt fermentum lacinia. Fusce at dapibus dui. Donec eget justo felis. Quisque quam justo, tincidunt non porta ac, porttitor in est. Curabitur eu quam quis mi blandit faucibus et ac nunc.

Duis magna tellus, viverra non mauris id, elementum hendrerit odio.

Nullam dapibus metus nunc, sollicitudin convallis libero commodo rutrum. Proin ullamcorper tellus nec nisl porta consectetur. Praesent sollicitudin elit eros, eleifend elementum felis eleifend et. Integer fringilla, velit a mattis lobortis, justo est imperdiet odio, vel tempor purus nisl non eros. Nunc semper viverra dolor at dictum. Mauris porta nec augue gravida consectetur. Vivamus elit velit, aliquet in ante eleifend, sodales consequat felis.

You can find the Processing Reference <a href="/processing/ref.html">here</a>.

<div id="p5canvas"></div>
<small style="color:#ccc;">dont forget to right~</small>

<script type="text/javascript">

    var alphanum = 'abcdefghijklmnopqrstuvwxyz1234567890';
    var randChar = alphanum.charAt(_.random(alphanum.length-1));

    function setup() {
        var canvas = createCanvas(500, 500);

        canvas.parent("p5canvas");
        noLoop();
        noStroke();
    }

    function draw() {
        background(255, 200, 200);
        ellipse(134, 256, 100, 100);
        fill(200);
        textSize(20);
        text('press '+randChar, 100, 256);
        noStroke();
    }

    function keyPressed() {
        if (key.toLowerCase() == randChar) {
            
            var rand = _.random(2);
            background(rand == 0 ? 255 : 200,
                       rand == 1 ? 255 : 200,
                       rand == 2 ? 255 : 200);

            var size = _.random(20, 140);
            var randx = _.random(20, 450);
            var randy = _.random(50, 450);
            fill(255);
            ellipse(randx, randy, size, size);

            randChar = alphanum.charAt(_.random(alphanum.length-1));
            fill(200);
            textSize(20);
            text(randChar, randx-5, randy+5);
        }
    }

    var canvas = document.getElementById('p5canvas');
    canvas.onselectstart = function () { return false; }

</script>
