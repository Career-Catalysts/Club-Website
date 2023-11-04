@media (min-width: 300px) | @media (100px <= width <= 300px)

max-width

vw, vh 
<!-- viewoport width and height -->

use rem
<!-- relative to font size -->

@media (orientation: portrait)
<!-- check when width < height; landscape also available -->

@media (min-aspect-ratio: 1 / 1)


@container
<!-- another useful trick for responsive layout -->

@keyframes
<!-- for animations -->

parallax effect can be made by making use of depth via z-axis
- `perspective: 20px;`
- `transform-style: preserve-3d;`
- `transform: translateZ(10px) scale(0.5);`

can make items snap in place when scrolling