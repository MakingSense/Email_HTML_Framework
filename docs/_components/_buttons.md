# Botones

## Tamaños

> Botón grande

<button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: #33AD73; color: #FFFFFF; border: 0px;">REGÍSTRATE GRATIS</button>

```css
.button-big {
  font-size: 15px;
  line-height: 15px;
  font-weight: 600;
  text-align: center;
  border-radius: 30px;
  padding: 20px 42px;
}
```

> Botón mediano

<button style="font-size: 13px; line-height: 13px; font-weight: 600; text-align: center; border-radius: 30px; padding: 15px 27px; background-color: #33AD73; color: #FFFFFF; border: 0px;">REGÍSTRATE GRATIS</button>

```css
.button-medium {
  font-size: 13px;
  line-height: 13px;
  font-weight: 600;
  text-align: center;
  border-radius: 30px;
  padding: 15px 27px;
}
```

> Botón chico

<button style="font-size: 11px; line-height: 11px; font-weight: 600; text-align: center; border-radius: 30px; padding: 11px 23px; background-color: #33AD73; color: #FFFFFF; border: 0px;">REGÍSTRATE GRATIS</button>

```css
.button-medium {
  font-size: 11px;
  line-height: 11px;
  font-weight: 600;
  text-align: center;
  border-radius: 30px;
  padding: 11px 23px;
}
```
## Colores

Dentro de cada tamaño una jerarquía primaria y otra secundaria:

> Primario verde

<table border="0" cellpadding="0" cellspacing="0" width="100%" style="border: 0px;">
  <tr style="border: 0px;">
    <td align="center" valign="middle" style="border: 0px;">
      <button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: #33AD73; color: #FFFFFF; border: 0px;">REGÍSTRATE GRATIS</button>
    </td>
    <td align="center" valign="middle" style="border: 0px;">
      <button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: #4CCA8E; color: #FFFFFF; border: 0px;">REGÍSTRATE GRATIS</button>
    </td>
  </tr>
</table>

```css
.primary-green {
  background-color: #33AD73;
  color: #FFFFFF;
}

.primary-green:hover {
  background-color: #4CCA8E;
}
```

Esto va en la cabecera del email:
```html
<style type="text/css">

.button-green--td:hover,
.button-green--a:hover {
  background: #008046 !important;
  border-color: #008046 !important;
}/* Button primary-green */

</style>
```

Esto va en el cuerpo del email:
```html
<tr>
  <td align="center" style="padding-top: 30px;">
    <table border="0" cellspacing="0" cellpadding="0" class="responsive-button">
      <tr>
        <td align="center">
          <div style="display:inline-block;">
            <!--[if mso]> <v:roundrect xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w="urn:schemas-microsoft-com:office:word" arcsize="99%" stroke="f" fillcolor="#33AD73" style="height:55px;v-text-anchor:middle;width:255.39px;" > <w:anchorlock/> <center style="width:100%;" > <![endif]-->
            <a href="#" target="_blank" class="button-green--a" style="box-sizing:content-box;background-color:#33AD73;border-radius:99px;color:#FFF;display:inline-block;font-family: Helvetica, Arial, sans-serif;font-size:13px;font-style:normal;font-weight:bold;line-height:50px;text-align:center;text-decoration:none;padding: 0 31px;-webkit-text-size-adjust:none;word-break:break-all;">CREA TU CUENTA GRATIS</a>
            <!--[if mso]> </center> </v:roundrect> <![endif]-->
          </div>
        </td>
      </tr>
    </table>
  </td>
</tr>
```
> Secundario verde

<table border="0" cellpadding="0" cellspacing="0" width="100%" style="border: 0px;">
  <tr style="border: 0px;">
    <td align="center" valign="middle" style="border: 0px;">
      <button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: transparent; color: #33AD73; border: 1px solid #33AD73;">REGÍSTRATE GRATIS</button>
    </td>
    <td align="center" valign="middle" style="border: 0px;">
      <button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: rgba(51,173,115,.2); color: #33AD73; border: 1px solid #33AD73;">REGÍSTRATE GRATIS</button>
    </td>
  </tr>
</table>

```css
.primary-green {
  background-color: #33AD73;
  color: #FFFFFF;
}

.primary-green:hover {
  background-color: #4CCA8E;
}
```

Esto va en la cabecera del email:
```html
<style type="text/css">

.button-green--td:hover,
.button-green--a:hover {
  background: #008046 !important;
  border-color: #008046 !important;
}/* Button primary-green */

</style>
```

Esto va en el cuerpo del email:
```html
<tr>
  <td align="center" style="padding-top: 30px;">
    <table border="0" cellspacing="0" cellpadding="0" class="responsive-button">
      <tr>
        <td align="center">
          <div style="display:inline-block;">
            <!--[if mso]> <v:roundrect xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w="urn:schemas-microsoft-com:office:word" arcsize="99%" stroke="f" fillcolor="#33AD73" style="height:55px;v-text-anchor:middle;width:255.39px;" > <w:anchorlock/> <center style="width:100%;" > <![endif]-->
            <a href="#" target="_blank" class="button-green--a" style="box-sizing:content-box;background-color:#33AD73;border-radius:99px;color:#FFF;display:inline-block;font-family: Helvetica, Arial, sans-serif;font-size:13px;font-style:normal;font-weight:bold;line-height:50px;text-align:center;text-decoration:none;padding: 0 31px;-webkit-text-size-adjust:none;word-break:break-all;">CREA TU CUENTA GRATIS</a>
            <!--[if mso]> </center> </v:roundrect> <![endif]-->
          </div>
        </td>
      </tr>
    </table>
  </td>
</tr>
```
> Primario amarillo

<table border="0" cellpadding="0" cellspacing="0" width="100%" style="border: 0px;">
  <tr style="border: 0px;">
    <td align="center" valign="middle" style="border: 0px;">
      <button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: #FCE579; color: #302100; border: 1px solid #FCE579;">REGÍSTRATE GRATIS</button>
    </td>
    <td align="center" valign="middle" style="border: 0px;">
      <button style="font-size: 15px; line-height: 15px; font-weight: 600; text-align: center; border-radius: 30px; padding: 20px 42px; background-color: #b4a250; color: #302100; border: 1px solid #b4a250;">REGÍSTRATE GRATIS</button>
    </td>
  </tr>
</table>

```css
.primary-yellow {
  background-color: #FCE579;
  color: #302100;
}

.primary-yellow:hover {
  background-color: #b4a250;
}
```

Esto va en la cabecera del email:
```html
<style type="text/css">

.button-yellow--td:hover,
.button-yellow--a:hover {
  background: #008046 !important;
  border-color: #008046 !important;
}/* Button primary-green */

</style>
```

Esto va en el cuerpo del email:
```html
<tr>
  <td align="center" style="padding-top: 30px;">
    <table border="0" cellspacing="0" cellpadding="0" class="responsive-button">
      <tr>
        <td align="center">
          <div style="display:inline-block;">
            <!--[if mso]> <v:roundrect xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w="urn:schemas-microsoft-com:office:word" arcsize="99%" stroke="f" fillcolor="#33AD73" style="height:55px;v-text-anchor:middle;width:255.39px;" > <w:anchorlock/> <center style="width:100%;" > <![endif]-->
            <a href="#" target="_blank" class="button-yellow--a" style="box-sizing:content-box;background-color:#33AD73;border-radius:99px;color:#FFF;display:inline-block;font-family: Helvetica, Arial, sans-serif;font-size:13px;font-style:normal;font-weight:bold;line-height:50px;text-align:center;text-decoration:none;padding: 0 31px;-webkit-text-size-adjust:none;word-break:break-all;">CREA TU CUENTA GRATIS</a>
            <!--[if mso]> </center> </v:roundrect> <![endif]-->
          </div>
        </td>
      </tr>
    </table>
  </td>
</tr>
```
