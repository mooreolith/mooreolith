Hi. Thanks for stopping by. This is Josh Moore's github.

This is my most recent github, mooreolith. Past ones included: 
* thwee-alchemist
* stauffenbits
* social-cartography
* box-lang
* lowrekey
* lowerkey
Sorry for littering on the information highway. I'm tidier at work, promise.

The common thread in this list is an attempt to properly implement 
[Dr. Todd Veldhuizen's Dynamic Multilevel Graph Visualization](https://arxiv.org/abs/0712.1549) as an 
easy to use HTML5 web component. At first as a threejs/jquery plugin. Eventually as a C++ library 
compiled to webassembly (requiring many steps for building and including the blob of program data). 

My hope for this technology is to help humans enlighten each other with regards to complex topics, 
and more specifically visualize data flows through programs' variables and function structures, as 
well as engineering assemblies, connections drawn as a half physical, half abstract representation. 
Greater understanding of parts' connections might lead to increased safety, and faster engineering 
cycles. 

So in this version (layout), I am trying to limit dependencies to threejs, which is reasonable. To that
end, I wrote the vector operations as functions on (pairs of) arrays. 

There's not much to it this time around. I began by writing the bare bones layout calculation, in the 
paper referred to "single level layout". Next steps are to salvage the Barnes Hut Tree from an earlier
version, itself a perfectly fine implementation.

The difficulty (for me, now) lies in tweaking the variables to arrive at stable layouts. It's a four or 
five variable balancing act. My hope is that I can 1) define metrics for the resulting layouts that 
machine learning can predict the necessary constants for. Vertex instantiation uses Math.random(). 

Maybe I should just define a sequence of values to keep the calculations and metrics consistent. 
Here's the current version: (early stages). [layout](https://github.com/mooreolith/layout)

other projects:
* [eight queens](https://mooreolith.github.io/eight-queens) an eight queens riddle with some solutions.
* [es.ipynb](https://mooreolith.github.io/es.ipynb) a crude localStorage notebook for browser javascript.

