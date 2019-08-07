# Me gusta

Este componente interactivo, logra una similitud al "Me gusta" que se utiliza en las redes sociales. Si lo utilizamos en un email, acompañamos a usabilidad del usuario a que lo vea como algo familiar, como resultado una experiencia positiva dentro del email.

<iframe height="427" style="width: 100%;" scrolling="no" title="Like" src="//codepen.io/IgnacioRodrigues/embed/ymvZPr/?height=427&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/ymvZPr/'>Like</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

```html
<style>
  .pf {
    display: block;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    background-position: -56px 56px;
  }

  @media screen and (max-width:9999px) {

    .hov-l:hover .pf,
    *[summary="hov-l"]:hover *[summary="pf"] {
      background-position: 2px 1px !important;
    }

    .display-block:hover .display-none * {
      display: block !important;
    }
  }
</style>
```

```html
<table width="500" border="0" cellspacing="0" cellpadding="0" style="border:0">
  <tr>
    <td class="m-bgg tag-cw" valign="top" colspan="1" rowspan="3">
      <a href="#" class="hov-l" summary="hov-l" data-hs-link-id="0" target="_blank">
        <table width="100%" border="0" cellspacing="0" cellpadding="0" style="border:0">
          <tbody>
            <tr>
              <td align="center" valign="top" style="background-image:url(https://imgur.com/4ufxoN1.png);background-size:auto 100%;background-position:center center;background-repeat: no-repeat">
                <span class="pf" summary="pf" style="background-image:url(https://imgur.com/0BINXiw.png);">
                  <!--[if !((gte mso 9)|(IE))]><!--><img src="https://i.imgur.com/koZkyNL.png" width="312" style="width:100%;max-width:100%;display:block;" alt="DopplerGram">
                  <!--<![endif]-->
                  <!--[if mso]><a href="https://www.instagram.com/p/Bynj3wHF_bn/"><img src="https://imgur.com/4ufxoN1.png" width="312" style="display:block;" alt="DopplerGram"></a><!--<![endif]-->
                </span>
              </td>
            </tr>
          </tbody>
        </table>
      </a>
    </td>
    <td class="m-bgg m-tag-sw tag-sh" valign="top">&nbsp;</td>
  </tr>
</table>
```
