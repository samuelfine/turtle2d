# &lt;lt-sprite&gt;

The `<lt-sprite>` element, or Sprite, is custom element for dynamic game objects that can be solid, can move, or are animated. Sprite elements are often the base element for a player character, other NPCs, or objects that can be interacted with.

*[dynamic]: Game objects that will move and change

!!! info

    If you want to create a game object that is static, or will be rendered having a repeated tiling image—like walls, floors, or larger background images—consider using a [`<lt-tile>`](lt-tile.md) instead.

*[static]: Game objects that cannot move or be moved

## Example

## Attributes
### General
| Attribute   |  Description        | Default value |
| ----------- | -------------------|---------------- |
| `x`  | A positive or negative number representing the sprite's position on the horizontal `x` axis, in pixels, starting from `0`,`0` in the upper left corner | 0 |
| `y`  | A positive or negative number representing the sprite's position on the vertical `y` axis, in pixels, starting from `0`,`0` in the upper left corner      | 0 |
| `width` | A positive number representing the `width` of the sprite, in pixels | 0 |
| `height` | A positive number representing the `height` of the sprite, in pixels | 0 |
| `persists` | If this attribute is set, the sprite object will persist across Maps. Useful for player sprites, or other global sprites that need to be available in more than one Map  . | false/null |

### Rendering &amp; Animation
| Attribute   |  Description        | Default value |
| ----------- | -------------------|---------------- |
| `image-url` | The URL of an image file used to render the sprite. Can be a single image, or a sprite strip/sheet for animation. | null |
| `fps` | The speed that the sprite should animate at, in frames per second. | null |
| `frames` | The number of frames that should be cycled through, from left to right. | null |
| `frame-width` | The width of a single frame of animation. Usually the same width as the sprite itself, or larger if the frames have space around them. | null |