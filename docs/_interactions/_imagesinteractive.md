# Imagenes con hover

<iframe height="470" style="width: 100%;" scrolling="no" title="Hover image" src="//codepen.io/IgnacioRodrigues/embed/ymvrxj/?height=470&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/ymvrxj/'>Hover image</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

Esto va en la cabecera del email:

```html
.rollover:hover > img,
* [summary=rollover]:hover > img{
  max-height: 0px !important;
}  
.rollover:hover > div img,
* [summary=rollover]:hover > div img{
  max-height: none !important;
}

@media screen and (max-device-width:1024px) {
  .rollover:hover > img,
  * [summary=rollover]:hover > img{
    max-height: none !important;
  }
  .rollover:hover > div img,
  * [summary=rollover]:hover > div img{
    max-height: 0px !important;
  }  
}
```

Esto va en el cuerpo del email:

```html
   <a class="rollover" summary="rollover" href="http://store.nike.com/us/en_us/pd/flyknit-lunar-3-running-shoe/pid-10252949/pgid-1561757">
     <img src="http://freshinbox.com/examples/image-swap/images/shoe-main2.jpg" width="500" style="display:block;width:500px;"  alt="Nike FlyKnit 3" border=0>
     <div style="mso-hide:all;">
       <img src="http://freshinbox.com/examples/image-swap/images/shoe-alt2.jpg" style="max-height:0px;display:block;width:500px;" width="500" alt="" border=0>
     </div>
   </a>
```
