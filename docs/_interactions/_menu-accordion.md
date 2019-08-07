# Menu acordion

<iframe height="397" style="width: 100%;" scrolling="no" title="Menu acordion" src="//codepen.io/IgnacioRodrigues/embed/KOQENp/?height=397&theme-id=0&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/KOQENp/'>Menu acordion</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>


> CSS

Esta parte va en la cabecera del email:

```html
<!-->
    <style type="text/css">
        @media only screen and (max-width:480px) {
            @-ms-viewport {
                width: 320px;
            }
            @viewport {
                width: 320px;
            }
        }
    </style>
    <!--<![endif]-->
    <!--[if mso]>
        <xml>
        <o:OfficeDocumentSettings>
          <o:AllowPNG/>
          <o:PixelsPerInch>96</o:PixelsPerInch>
        </o:OfficeDocumentSettings>
        </xml>
        <![endif]-->
    <!--[if lte mso 11]>
        <style type="text/css">
          .outlook-group-fix { width:100% !important; }
        </style>
        <![endif]-->
    <!--[if !mso]><!-->
    <link href="https://fonts.googleapis.com/css?family=Ubuntu:300,400,500,700" rel="stylesheet" type="text/css">
    <style type="text/css">
        @import url(https://fonts.googleapis.com/css?family=Ubuntu:300,400,500,700);
    </style>
    <!--<![endif]-->
    <style type="text/css">
        @media only screen and (min-width:480px) {
            .dp-column-per-100 {
                width: 100% !important;
                max-width: 100%;
            }
        }
    </style>
    <style type="text/css">
        noinput.dp-menu-checkbox {
            display: block!important;
            max-height: none!important;
            visibility: visible!important;
        }

        @media only screen and (max-width:480px) {
            .dp-menu-checkbox[type="checkbox"] ~ .dp-inline-links {
                display: none!important;
            }
            .dp-menu-checkbox[type="checkbox"]:checked ~ .dp-inline-links,
            .dp-menu-checkbox[type="checkbox"] ~ .dp-menu-trigger {
                display: block!important;
                max-width: none!important;
                max-height: none!important;
                font-size: inherit!important;
            }
            .dp-menu-checkbox[type="checkbox"] ~ .dp-inline-links > a {
                display: block!important;
            }
            .dp-menu-checkbox[type="checkbox"]:checked ~ .dp-menu-trigger .dp-menu-icon-close {
                display: block!important;
            }
            .dp-menu-checkbox[type="checkbox"]:checked ~ .dp-menu-trigger .dp-menu-icon-open {
                display: none!important;
            }
        }
    </style>
```

> HTML

Este snippet va en el cuerpo del email:

```html
<table border="0" cellpadding="0" cellspacing="0" width="100%" bgcolor="#ffb017">
  <tr>
    <td align="center" valign="top">
      <div>
        <!--[if mso | IE]><table align="center" border="0" cellpadding="0" cellspacing="0" class="" style="width:600px;" width="600" ><tr><td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;"><![endif]-->
        <div style="background:#ffb017;background-color:#ffb017;Margin:0px auto;max-width:600px;">
            <table align="center" border="0" cellpadding="0" cellspacing="0" role="presentation" style="background:#ffb017;background-color:#ffb017;width:100%;">
                <tbody>
                    <tr>
                        <td style="direction:ltr;font-size:0px;padding:20px 0;text-align:center;vertical-align:top;">
                            <!--[if mso | IE]><table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td class="" style="vertical-align:top;width:600px;" ><![endif]-->
                            <div class="dp-column-per-100 outlook-group-fix" style="font-size:13px;text-align:left;direction:ltr;display:inline-block;vertical-align:top;width:100%;">
                                <table border="0" cellpadding="0" cellspacing="0" role="presentation" style="vertical-align:top;" width="100%">
                                    <tr>
                                        <td align="center" style="font-size:0px;word-break:break-word;">
                                            <!--[if !mso><!-->
                                            <input type="checkbox" id="3d9259acdec3aebe" class="dp-menu-checkbox" style="display:none !important; max-height:0; visibility:hidden;">
                                            <!--<![endif]-->
                                            <div class="dp-menu-trigger" style="display:none;max-height:0px;max-width:0px;font-size:0px;overflow:hidden;">
                                                <label for="3d9259acdec3aebe" class="dp-menu-label" style="display:block;cursor:pointer;mso-hide:all;-moz-user-select:none;user-select:none;align:center;color:#ffffff;font-size:30px;font-family:Ubuntu, Helvetica, Arial, sans-serif;text-transform:uppercase;text-decoration:none;line-height:30px;padding:10px;"><span class="dp-menu-icon-open" style="mso-hide:all;">&#9776; </span><span class="dp-menu-icon-close" style="display:none;mso-hide:all;">&#8855;</span></label>
                                            </div>
                                            <div class="dp-inline-links">
                                                <!--[if mso | IE]><table role="presentation" border="0" cellpadding="0" cellspacing="0" align="center"><tr><td style="padding:15px 10px;" class="" ><![endif]--><a class="dp-link" href="#" target="_blank" style="display:inline-block;color:#ffffff;font-family:Ubuntu, Helvetica, Arial, sans-serif;font-size:13px;font-weight:normal;line-height:22px;text-decoration:none;text-transform:uppercase;padding:15px 10px;">Novedades</a>
                                                <!--[if mso | IE]></td><td style="padding:15px 10px;" class="" ><![endif]--><a class="dp-link" href="#" target="_blank" style="display:inline-block;color:#ffffff;font-family:Ubuntu, Helvetica, Arial, sans-serif;font-size:13px;font-weight:normal;line-height:22px;text-decoration:none;text-transform:uppercase;padding:15px 10px;">Catalogo</a>
                                                <!--[if mso | IE]></td><td style="padding:15px 10px;" class="" ><![endif]--><a class="dp-link" href="#" target="_blank" style="display:inline-block;color:#ffffff;font-family:Ubuntu, Helvetica, Arial, sans-serif;font-size:13px;font-weight:normal;line-height:22px;text-decoration:none;text-transform:uppercase;padding:15px 10px;">Productos</a>
                                                <!--[if mso | IE]></td><td style="padding:15px 10px;" class="" ><![endif]--><a class="dp-link" href="#" target="_blank" style="display:inline-block;color:#ffffff;font-family:Ubuntu, Helvetica, Arial, sans-serif;font-size:13px;font-weight:normal;line-height:22px;text-decoration:none;text-transform:uppercase;padding:15px 10px;">Iniciar Sesión</a>
                                                <!--[if mso | IE]></td></tr></table><![endif]-->
                                            </div>
                                        </td>
                                    </tr>
                                </table>
                            </div>
                            <!--[if mso | IE]></td></tr></table><![endif]-->
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
        <!--[if mso | IE]></td></tr></table><![endif]-->
      </div>

    </td>
  </tr>
</table>
```
