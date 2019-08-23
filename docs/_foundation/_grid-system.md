# Sistema de grillas

Nuestro sistema de cuadrícula se compone de 8 columnas flexibles con un padding de 15px. A continuación podrán visualizar los diferentes tamaños.


> Base HTML para comenzar a maquetar un email
## Base HTML

```html
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="x-apple-disable-message-reformatting">
  <title></title>

  <!-- CSS -->
  <style>
    /* CLIENT-SPECIFIC STYLES */

    /* Prevent WebKit and Windows mobile changing default text sizes */
    body,
    table,
    td,
    a {
      -webkit-text-size-adjust: 100%;
      -ms-text-size-adjust: 100%;
    }

    /* Remove spacing between tables in Outlook 2007 and up */
    table,
    td {
      mso-table-lspace: 0pt;
      mso-table-rspace: 0pt;
    }

    /* Allow smoother rendering of resized image in Internet Explorer */
    img {
      -ms-interpolation-mode: bicubic;
    }

    /* RESET STYLES */
    img {
      border: 0;
      height: auto;
      line-height: 100%;
      outline: none;
      text-decoration: none;
    }

    table {
      border-collapse: collapse !important;
    }

    body {
      height: 100% !important;
      margin: 0 !important;
      padding: 0 !important;
      width: 100% !important;
    }

    /* Centers email on Android. */
    div[style*="margin: 16px 0"] {
      margin: 0 !important;
      font-size: 100% !important;
    }

    /* Removing blue links in Apple Mail */
    a[x-apple-data-detectors] {
      color: inherit !important;
      text-decoration: none !important;
      font-size: inherit !important;
      font-family: inherit !important;
      font-weight: inherit !important;
      line-height: inherit !important;
    }

    @media screen and (max-width: 480px) {
      .container__fluid {
        display: block;
        width: 100% !important;
      }
    }

    }
  </style>
  <!--[if gte mso 9]>
	<xml>
		<o:OfficeDocumentSettings>
			<o:AllowPNG/>
			<o:PixelsPerInch>96</o:PixelsPerInch>
		</o:OfficeDocumentSettings>
	</xml>
  <![endif]-->
</head>

<body style="margin: 0 !important; padding: 0 !important;">
  <table align="center" cellpadding="0" cellspacing="0" border="0" width="100%">
    <tr>
      <td align="center" valign="top">
        <!--[if mso]>
      <table cellspacing="0" cellpadding="0" border="0" width="600" align="center">
      <tr>
      <td>
      <![endif]-->

        <!-- Email Body : BEGIN -->
        <table align="center" cellspacing="0" cellpadding="0" border="0" width="100%" style="max-width: 600px; width: 100%;" class="container__fluid">
          <!-- Aquí va el contenido-->
        </table>
        <!-- Email Body : END -->

        <!--[if mso]>
      </td>
      </tr>
      </table>
      <![endif]-->
      </td>
    </tr>
  </table>
</body>

</html>
```

> Tamaño de grilla

## Grilla 1 de 1

?> _TIP_ - Con esta grilla podemos indicar la base de un email

<div style="background: #FFD665; width: 100%; padding: 15px 15px;">
  <p style="background: #FFE6A0; padding: 15px 15px; margin: 0; max-width: 100%; text-align: center; font-size: 1.4rem; font-weight: 500;">
    1/1
  </p>
</div>

### Snippet HTML - Grilla 1 de 1

```html
<tr>
  <td align="center" height="100%" valign="top" width="100%">
    <!--[if (gte mso 9)|(IE)]>
    <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
    <tr>
    <td align="center" valign="top" width="600">
    <![endif]-->
      <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:600px;">
        <tr>
          <td align="center" valign="top">

           1/1

          </td>
        </tr>
      </table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
  </td>
</tr>
```
<br>

## Grilla 1 de 2

<div style="background: #FFD665; width: 100%; float: none; padding: 15px 5px 15px 15px; margin: 0px auto;">
  <div style="background: #FFD665; max-width: 100%; width: 49%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/2
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 49%;  padding-left: 15px; padding-right: 0px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/2
    </p>
  </div>
</div>

### Snippet HTML - Grilla 1 de 2

```html
<tr>
  <td align="center" valign="top" width="100%">
    <!--[if (gte mso 9)|(IE)]>
    <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
    <tr>
    <td align="center" valign="top" width="600">
    <![endif]-->
    <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:600px;" bgcolor="#FFFFFF">
      <tr>
        <td align="center" valign="top" style="font-size:0;">
          <!--[if (gte mso 9)|(IE)]>
          <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
          <tr>
          <td align="left" valign="top" width="295">
          <![endif]-->
          <div style="display:inline-block; max-width:295px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:295px;" class="container__fluid">
              <tr>
                <td align="center" valign="top" style="padding: 10px 10px;">

                  1/2

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="295">
          <![endif]-->
          <div style="display:inline-block; max-width:295px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:295px;" class="container__fluid">
              <tr>
                <td align="center" valign="top" style="padding: 10px 10px;">

                  1/2

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          </tr>
          </table>
          <![endif]-->
        </td>
      </tr>
    </table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
  </td>
</tr>
```
<br>

## Grilla 1 de 3

<div style="background: #FFD665; width: 100%; float: none; padding: 15px 5px 15px 15px; margin: 0px auto;">
  <div style="background: #FFD665; max-width: 100%; width: 32%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/3
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 32%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/3
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 33.33%; padding-left: 0px; padding-right: 0px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/3
    </p>
  </div>
</div>

### Snippet HTML - Grilla 1 de 3

```html
<tr>
  <td align="center" valign="top" width="100%">
    <!--[if (gte mso 9)|(IE)]>
    <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
    <tr>
    <td align="center" valign="top" width="600">
    <![endif]-->
    <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:600px;" bgcolor="#FFFFFF">
      <tr>
        <td align="center" valign="top" style="font-size:0;">
          <!--[if (gte mso 9)|(IE)]>
          <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
          <tr>
          <td align="left" valign="top" width="195">
          <![endif]-->
          <div style="display:inline-block; max-width:195px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:195px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top">

                  1/3

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="195">
          <![endif]-->
          <div style="display:inline-block; max-width:195px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:195px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top">

                  1/3

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="195">
          <![endif]-->
          <div style="display:inline-block; max-width:195px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:195px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top">

                  1/3

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          </tr>
          </table>
          <![endif]-->
        </td>
      </tr>
    </table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
  </td>
</tr>
```
<br>

## Grilla 1 de 4

<div style="background: #FFD665; width: 100%; float: none; padding: 15px 5px 15px 15px; margin: 0px auto;">
  <div style="background: #FFD665; max-width: 100%; width: 24%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/4
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 24%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/4
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 24%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/4
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 25%; padding-left: 0px; padding-right: 0px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/4
    </p>
  </div>
</div>

### Snippet HTML - Grilla 1 de 4

```html
<tr>
  <td align="center" valign="top" width="100%">
    <!--[if (gte mso 9)|(IE)]>
    <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
    <tr>
    <td align="center" valign="top" width="600">
    <![endif]-->
    <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:600px;" bgcolor="#FFFFFF">
      <tr>
        <td align="center" valign="top" style="font-size:0;">
          <!--[if (gte mso 9)|(IE)]>
          <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
          <tr>
          <td align="left" valign="top" width="145">
          <![endif]-->
          <div style="display:inline-block; max-width:145px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:145px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla cuatro

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="145">
          <![endif]-->
          <div style="display:inline-block; max-width:145px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:145px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla cuatro

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="145">
          <![endif]-->
          <div style="display:inline-block; max-width:145px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:145px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla cuatro

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="145">
          <![endif]-->
          <div style="display:inline-block; max-width:145px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:195px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla cuatro

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          </tr>
          </table>
          <![endif]-->
        </td>
      </tr>
    </table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
  </td>
</tr>
```
<br>

## Grilla 1 de 8

<div style="background: #FFD665; width: 100%; float: none; padding: 15px 5px 15px 15px; margin: 0px auto;">
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 0px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
</div>

### Snippet HTML - Grilla 1 de 8

```html
<tr>
  <td align="center" valign="top" width="100%">
    <!--[if (gte mso 9)|(IE)]>
    <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
    <tr>
    <td align="center" valign="top" width="600">
    <![endif]-->
    <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:600px;" bgcolor="#FFFFFF">
      <tr>
        <td align="center" valign="top" style="font-size:0;">
          <!--[if (gte mso 9)|(IE)]>
          <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
          <tr>
          <td align="left" valign="top" width="70">
          <![endif]-->
          <div style="display:inline-block; max-width:70px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:70px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla 1/8

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="525">
          <![endif]-->
          <div style="display:inline-block; max-width:525px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:525px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla 7/8

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          </tr>
          </table>
          <![endif]-->
        </td>
      </tr>
    </table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
  </td>
</tr>
```
<br>

## Grilla mixta

<div style="background: #FFD665; width: 100%; float: none; padding: 15px 5px 15px 15px; margin: 0px auto;">
  <div style="background: #FFD665; max-width: 100%; width: 12%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      1/8
    </p>
  </div>
  <div style="background: #FFD665; max-width: 100%; width: 87%; padding-left: 0px; padding-right: 15px; display: inline-block;">
    <p style="background: #FFE6A0; padding: 15px 15px; margin: 0px 0px; text-align: center; font-size: 1.4rem; font-weight: 500;">
      7/8
    </p>
  </div>
</div>

### Snippet HTML - Grilla 1 de 8

```html
<tr>
  <td align="center" valign="top" width="100%">
    <!--[if (gte mso 9)|(IE)]>
    <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
    <tr>
    <td align="center" valign="top" width="600">
    <![endif]-->
    <table align="center" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:600px;" bgcolor="#FFFFFF">
      <tr>
        <td align="center" valign="top" style="font-size:0;">
          <!--[if (gte mso 9)|(IE)]>
          <table align="center" border="0" cellspacing="0" cellpadding="0" width="600">
          <tr>
          <td align="left" valign="top" width="70">
          <![endif]-->
          <div style="display:inline-block; max-width:70px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:70px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla 1/8

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          <td align="left" valign="top" width="70">
          <![endif]-->
          <div style="display:inline-block; max-width:525px; vertical-align:top; width:100%;">
            <table align="left" border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:525px;" class="deviceWidth">
              <tr>
                <td align="center" valign="top" style="font-size:14px;">

                  Grilla 7/8

                </td>
              </tr>
            </table>
          </div>
          <!--[if (gte mso 9)|(IE)]>
          </td>
          </tr>
          </table>
          <![endif]-->
        </td>
      </tr>
    </table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
  </td>
</tr>
```

## Puntos de interrupción

Nuestros diferentes tamaños de columna cambian automáticamente las dimensiones una vez que alcanzan ciertos puntos de interrupción. La siguiente tabla muestra los puntos de interrupción de la consulta de medios.

<table>
    <thead>
        <tr class="odd">
            <th colspan="1"></th>
            <th colspan="3">Breakpoints</th>
        </tr>
        <tr class="even">
            <th>Grilla</th>
            <th>960px o más</th>
            <th>Entre 960px y 640px</th>
            <th>640px o menos</th>
        </tr>
    </thead>
    <tbody>
        <tr class="odd">
            <td><code>tamaño 1 de 8</code></td>
            <td>12.5%</td>
            <td>50%</td>
            <td>100%</td>
        </tr>
        <tr class="even">
            <td><code>tamaño 1 de 4</code>, <code>tamaño 2 de 8</code></td>
            <td>25%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="odd">
            <td><code>tamaño 1 de 3</code></td>
            <td>33.33%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="even">
            <td><code>tamaño 3 de 8</code></td>
            <td>37.5%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="odd">
            <td><code>tamaño 1 de 2</code>, <code>tamaño 2 de 4</code>, <code>tamaño 4 de 8</code></td>
            <td>50%</td>
            <td>50%</td>
            <td>100%</td>
        </tr>
        <tr class="even">
            <td><code>tamaño 5 de 8</code></td>
            <td>62.5%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="odd">
            <td><code>tamaño 2 de 3</code></td>
            <td>66.67%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="even">
            <td><code>tamaño 3 de 4</code>, <code>tamaño 6 de 8</code></td>
            <td>75%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="odd">
            <td><code>tamaño 7 de 8</code></td>
            <td>87.5%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
        <tr class="even">
            <td><code>tamaño 1 de 1</code>, <code>tamaño 2 de 2</code>, <code>tamaño 3 de 3</code>, <code>tamaño 4 de 4</code>, <code>tamaño 8 de 8</code></td>
            <td>100%</td>
            <td>100%</td>
            <td>100%</td>
        </tr>
    </tbody>
</table>
