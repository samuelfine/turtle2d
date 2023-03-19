# Why Turtle2D?

!!! info
    This section is not required to learn how to create games with Turtle2D, but may help you better understand some of the decision-making that went into designing and building the engine.

Turtle2D is objectively worse than most, if not all, other game engines. It's probably the slowest and have fewer features than all other engines.

Turtle2D was created for, and is built upon, a set of core principles. In no particular order:

## Making games is for everyone, everywhere.
Neither expensive hardware nor dedicated space should be a prerequisite for building games. Turtle2D aims to work on any device that can run a modern web browser. Desktop PCs, laptops, tablets, even smartphones. (The engine itself was developed with a 10-year-old laptop.) The Editor can be used with a keyboard and mouse, trackpad, or touch/stylus controls. Make a game at your desk, on the couch, on the bus, in a park.

## How I learned to stop worrying and love the DOM
Most HTML5-based game engines go to extreme lengths to avoid the DOM. They encapsulate the engine logic in Javascript, and the game's rendering in a `<canvas>` element. I get it. It does offer far better frame-to-frame performance and access to a lot of magic like WebGL. But even state of the art game engines pale in comparison to the flexibility and ease-of-use that modern web stack provides. A few examples:

- **GUI** - HTML and CSS are the best user interface tools mankind has ever created. CSS `flex` and `grid` offer fluid, responsive, and interactive layouts with very little code. Elements and their content can be bordered, shadowed, animated, or transformed with ease. No other game engine comes close.
- **Vector graphics** - Most game engines require plugins for vector graphic support. HTML and CSS generates scalable lines, rectangles, and circles with a couple lines of CSS. Not to mention, the browser has full native support for SVG rendering *and* animation.
- **A mature DOM** - thanks to decades of effort from some of the largest companies in human history, the Document Object Model is a polished system that inherently provides a tree-like structure for organizing elements, similar to most game engines, along with robust tooling for querying child/parent elements, creation and removal of elements, and event handling. Creating "prefab"-style reusable components by encapsulating markup, styles, and behavior together in a single HTML file allows for dynamic yet maintainable assets. The browser offers a _lot_, and Turtle2D leans into that.

## The best that 1983 has to offer
Turtle2D aims to allow people to create games of a similar fidelity to the 8-bit era. Of course, there are no hard restrictions—you aren't bound to 240p resolution or 256 colors—but Turtle2D offers no physics, no lighting, no shaders, basic box-driven collision detection. Games will be straightforward and limited in pizazz. 

## Make the Engine assistive, not prescriptive. 
Turtle2D's engine and custom elements offer a fast, easy way to make "typical" 2D games. But these are not a _requirement_ for making a Turtle2D game. For example, the `Input` manager has helpers for simple Sprite movement using WASD or a D-pad. But that can be ignored, modified, or removed easily.

All Turtle2D games are, basically, websites with some helpful code and guidance to make it fun. Anything you can do with HTML, CSS, and Javascript can be used in making Turtle2D games.



## Make making games stupidly easy.
## 2. Fast is more important than good.