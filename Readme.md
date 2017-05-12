## Semi-circle navbar

This is a sass mix-in to create a 90 degree arc of circular buttons and can connect the circles to a central point with spokes. It is slight modification on the on-circle mix-in by Hugo Giraudel and Ana Tudor in this article [https://css-tricks.com/snippets/sass/placing-items-circle/](https://css-tricks.com/snippets/sass/placing-items-circle/) 

Mixin
``` scss
  @import "semicircle-navbar";
  .rot-nav{
    @include arc-nav($item-count: 3, $circle-radius: 11em, $item-size: 5em, $corner: "bottom-right");
  }
```
HTML
``` html
     <nav class="rot-nav">
        <hr class="spoke"><hr class="spoke">
        <div class="circle"><a href="#">Blog</a></div>
        <div class="circle"><a href="#">Projects</a></div>
        <div class="circle"><a href="#">Photos</a></div>
     </nav>
```
