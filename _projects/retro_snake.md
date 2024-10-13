---
layout: page
title: Retro Snake
description: Retro Snake is a hardware implementation of the game Snake
img: assets/img/snake.jpeg
importance: 6
category: work
visible: true
---


It is one of the first games available on mobile phones. For this project, we used ATMega32 as the Microcontroller.

The game is displayed on a grid(16×16) built with 4 8×8 bi-color LED matrices. There are 2 digital IR sensors to control the snake. In the game, we can move the snake head right or left by using these sensors. Whenever the snake eats a food, one point is added to the score and the length of the snake increases.

There are two modes in the game:
 - Classic Mode
 - Obstacle Mode

In classic mode, the game continues until the head of the snake collides with its own body.
In obstacle mode, there are 4 levels. When the snake eats two foods, the level increases except for the last level. The game ends when the snake’s head collides with its body or a obstacle.
The score and the high score is displayed on a 16×2 I2C LCD display.
We have used a buzzer to indicate that the snake has eaten a food.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/circuit_diagram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0"><iframe width="470" height="264" src="https://www.youtube.com/embed/ReesaAqyTmY?si=FKR8TocIadGuU7NA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    On the left, It is circuit diagram of the project. On the right, you can find the video demonstration of the project.
</div>


Github: [Retro Snake](https://github.com/RedwanulKarim612/Retro-Snake)