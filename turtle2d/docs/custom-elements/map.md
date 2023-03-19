# &lt;map&gt;

Turtle2D uses the HTML `<map>` element to represent sections of a game, similar scenes or levels in other game engine. One Map might contain the interior of a building, another Map might contain the overworld and all its elements, while a third Map could contain the game's main menu.

Only one Map can be active at a time. The contents of the active Map will be rendered and updated by the game's engine, while other inactive Maps will not. 

```
<map class="building-a" active>
    <lt-tile class="wall wall-top ...></lt-tile>
    <lt-tile class="wall wall-right ...></lt-tile>
    <lt-tile class="wall wall-bottom ...></lt-tile>
    <lt-tile class="wall wall-left ...></lt-tile>
    ...
</map>

<map class="overworld">
    <lt-sprite class="tree" ...></lt-sprite>
    <lt-sprite class="tree" ...></lt-sprite>
    ...
</map>
```

*[dynamic]: Game objects that will move and change