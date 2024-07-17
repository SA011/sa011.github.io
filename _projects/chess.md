---
layout: page
title: Chess Engine
description: A chess project with home-made engine
img: assets/img/chess.png
importance: 1
category: fun
visible: true
---

A very simple chess engine implementing Alpha-Beta Prunning. It can beat stockfish level 2 with only depth 3. It does not yet use any book moves. I hope it will improve if I incorporate book move with it.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/open.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/chess.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A simple chess board in middle game
</div>

The chess engine can find checkmates and positional placement of pieces.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/checkmate.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/menu.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A checkmate and main-menu with different options.
</div>
