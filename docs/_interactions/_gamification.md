# Gamificación

<iframe height="699" style="width: 100%;" scrolling="no" title="Gamificación" src="//codepen.io/IgnacioRodrigues/embed/MNqjeg/?height=699&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/MNqjeg/'>Gamificación</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

```html
<style type="text/css">
    a[x-apple-data-detectors] {
        color: inherit !important;
        text-decoration: none !important;
        font-size: inherit !important;
        font-family: inherit !important;
        font-weight: inherit !important;
        line-height: inherit !important;
    }
    * {
        -webkit-font-smoothing: antialiased;
    }
    body {
        height:100% !important;
        Margin:0 !important;
        padding:0 !important;
        width:100% !important;
        padding: 0;
        min-width: 100%;
        background-color: #ffffff;
        font-family: Calibri, sans-serif, 'Open Sans';
        -webkit-font-smoothing: antialiased;
    }
    table {
        border-spacing: 0;
        color: #333333;
        font-family: Calibri, sans-serif, 'Open Sans';
    }
    img {
        border: 0;
    }
    .wrapper {
        width: 100%;
        table-layout: fixed;
        -webkit-text-size-adjust: 100%;
        -ms-text-size-adjust: 100%;
    }
    .webkit {
        max-width: 600px;
    }
    .outer {
        Margin: 0 auto;
        width: 100%;
        max-width: 600px;
    }
    .full-width-image img {
        width: 100%;
        max-width: 600px;
        height: auto;
    }
    .inner {
        padding: 10px;
    }
    p {
        Margin: 0;
        padding-bottom: 10px;
    }
    p, li, td, {
        font-family: Calibri, sans-serif, 'Open Sans';
        font-size: 14px;
        color: #333333;
        -webkit-font-smoothing: antialiased;
    }
    .h1 {
        font-size: 21px;
        font-weight: bold;
        Margin-top: 15px;
        Margin-bottom: 5px;
        font-family: Calibri, sans-serif, 'Open Sans';
        -webkit-font-smoothing: antialiased;
    }
    .h2 {
        font-size: 18px;
        font-weight: bold;
        Margin-top: 10px;
        Margin-bottom: 5px;
        font-family: Calibri, sans-serif, 'Open Sans';
        -webkit-font-smoothing: antialiased;
    }

    .one-column .contents {
        text-align: left;
        font-family: Calibri, sans-serif, 'Open Sans';
        -webkit-font-smoothing: antialiased;
    }
    .one-column p {
        font-size: 14px;
        Margin-bottom: 10px;
        font-family: Calibri, sans-serif, 'Open Sans';
        -webkit-font-smoothing: antialiased;
    }

    .two-column {
        text-align: center;
        font-size: 0;
    }
    .two-column .column {
        width: 100%;
        max-width: 300px;
        display: inline-block;
        vertical-align: top;
    }
    .contents {
        width: 100%;
    }
    .two-column .contents {
        font-size: 14px;
        text-align: left;
    }
    .two-column img {
        width: 100%;
        max-width: 280px;
        height: auto;
    }
    .two-column .text {
        padding-top: 10px;
    }

    .three-column {
        text-align: center;
        font-size: 0;
        padding-top: 10px;
        padding-bottom: 10px;
    }
    .three-column .column {
        width: 100%;
        max-width: 200px;
        display: inline-block;
        vertical-align: top;
    }
    .three-column .contents {
        font-size: 14px;
        text-align: center;
    }
    .three-column img {
        width: 100%;
        max-width: 180px;
        height: auto;
    }
    .three-column .text {
        padding-top: 10px;
    }
    .appleFix a {
        color: #848484;
    }

    @media only screen and (max-device-width: 640px){
        .main-header {
            font-size: 20px !important;
        }
        .main-section-header {
            font-size: 28px !important;
        }
        .hide {
            display: none !important;
        }
        .align-center {
            text-align: center !important;
        }
        .deviceWidth {
            width: 400px !important;
        }

    }

    @media only screen and (max-device-width: 550px) {
        span[class="mv-copy1"] {
            font-size:18px !important;
            line-height:14px !important;
        }
        span[class="mv-copy2"] {
            font-size:45px !important;
            line-height:41px !important;
        }
        span[class="mv-copy3"] {
            font-size:18px !important;
            line-height:21px !important;
        }
        span[class="mv-copy4"] {
            font-size:35px !important;
            line-height:35px !important;
        }
        span[class="mv-copy5"] {
            font-size:23px !important;
            line-height:29px !important;
        }

    }

    @media only screen and (max-device-width: 414px) {
        .deviceWidth {
            width: 320px !important;
        }
        .mv-copy1 {
            font-size:18px !important;
            line-height:14px !important;
        }
        .mv-copy2 {
            font-size:45px !important;
            line-height:41px !important;
        }
        .mv-copy3 {
            font-size:18px !important;
            line-height:21px !important;
        }
        .mv-copy4 {
            font-size:35px !important;
            line-height:35px !important;
        }
        .mv-copy5 {
            font-size:23px !important;
            line-height:29px !important;
        }

    }


    @media only screen and (max-device-width: 375px) {
        .deviceWidth {
            width: 290px !important;
        }
    }

    @media only screen and (max-device-width: 320px){
        .main-header {
            font-size: 20px !important;
        }
        .main-section-header {
            font-size: 24px !important;
        }
        .align-center {
            text-align: center !important;
        }
        .deviceWidth {
            width: 220px !important;
        }
    }

</style>
<!--[if (gte mso 9)|(IE)]>
<style type="text/css">
    table {border-collapse: collapse !important;}
    .image_table {background-color:#ffffff;}
</style>
<![endif]-->
```

```html
<center class="wrapper" style="width:100%;table-layout:fixed;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%;">
    <div class="webkit" style="max-width:600px;margin:0 auto;">
        <!--[if (gte mso 9)|(IE)]>
        <table width="600" align="center" cellpadding="0" cellspacing="0" border="0" style="border-spacing:0;font-family: Calibri, sans-serif;color:#333333;" >
        <tr>
            <td style="padding-top:0;padding-bottom:0;padding-right:0;padding-left:0;" >
        <![endif]-->

        <!--START BODY-->
        <table class="outer" align="center" style="border-spacing:0;font-family: Calibri, sans-serif, &#39;Open Sans&#39;;color:#333333;Margin:0 auto;width:100%;max-width:600px;">
        <tbody><tr>
            <td style="padding-top:0;padding-bottom:0;padding-right:0;padding-left:0;">

                <!-- ======= start hero article ======= -->
                <table class="one-column" border="0" cellpadding="0" cellspacing="0" width="100%" style="border-spacing:0;max-width: 600px;">
                <tbody><tr>
                    <td align="center" style="">
                            <style>
                                body{
                                  -webkit-text-size-adjust:100%;
                                  }

                                  @media (max-device-width: 21024px) {
                                    .kinetic{
                                      display:block!important;
                                      max-height:none!important;
                                    }
                                    .fallback{
                                      display:none!important;
                                    }
                                  }

                            </style>

                            <center>
                                <table cellpadding="0" cellspacing="0" width="600">
                                <!--[if !mso 9]><!-->
                                <tbody><tr>
                                    <td style="z-index:500;padding:0px;position:relative;font-family:Lobster,Arial Bold,sans-serif;color:#ffffff;font-size:0px;line-height:0px;text-align:center;">
                                        <div class="kinetic" style="mso-hide:all;display:none;max-height:0;overflow:hidden;font-size:15px; line-height:15px;background-color:#44d7fb;color:#2e2a29;">
                                            <div style="font-size:35px; line-height:40px; mso-line-height:exactly;">&nbsp;</div>
                                              <span class="mv-copy1" style="font-family:Helvetica, Arial, sans-serif; font-size:16px; line-height:12px; font-weight:bold;">HIT THE ROAD THIS SUMMER WITH THE</span><br>
                                               <div style="font-size:6px; line-height:6px; mso-line-height:exactly;">&nbsp;</div>
                                              <span class="mv-copy2" style="font-family:Georgia, &#39;Times New Roman&#39;, Times, serif; font-size:40px; line-height:36px;">#UnitedStatesofBooks</span><br>
                                              <div style="font-size:20px; line-height:20px; mso-line-height:exactly;">&nbsp;</div>
                                              <span class="mv-copy3" style="font-family:Helvetica, Arial, sans-serif; font-size:15px; line-height:17px;">Follow along as we celebrate books from sea to shining sea. <br>
                                              Click the billboards to discover books set in each state.</span><br>
                                                 <div style="font-size:18px; line-height:18px; mso-line-height:exactly;">&nbsp;</div>
                                              <span class="mv-copy4" style="font-family:Georgia, &#39;Times New Roman&#39;, Times, serif; font-size:30px; line-height:30px; font-weight:bold;">BUCKLE UP.</span>
                                              <br>
                                              <span class="mv-copy5" style="font-family:Georgia, &#39;Times New Roman&#39;, Times, serif; font-size:18px; line-height:24px; font-weight:bold;">It's going to be a book-y ride!</span>
                                        </div>
                                    </td>
                                </tr>
                                <!--DAT JOURNEY THO-->
                                <tr>
                                    <td>
                                        <div class="kinetic" style="display:none;max-height:0;overflow:hidden;">
                                            <div style="position:relative;height:2410px;width:600px;font-size:0;line-height:0;">
                                                <!--STATIC ELEMENT-->
                                                <div style="z-index:300;position:fixed;top:0px;left:0px;width:100%;height:100%;left:0px;text-align:center;overflow:hidden;">
                                                    <img src="https://i.imgur.com/zIC90w4.png">
                                                </div>
                                                <!--//STATIC ELEMENT-->

                                                <!--BACKGROUND-->
                                                <div style="position:relative;top:0px;z-index:200;max-height:0px;overflow:visible;display:inline-block;">
                                                    <img src="https://i.imgur.com/gKh0mUr.png" style="display:block; width:600px;">
                                                </div>
                                                <!--//BACKGROUND-->

                                                <!--FOREGROUND-->
                                                <div style="position:relative;top:0px;z-index:400;max-height:0px;overflow:visible;display:inline-block;">
                                                    <img src="https://i.imgur.com/g9OM3F9.png" border"0"="" style="display:block; width:600px;">
                                                    <a href="#" style="text-decoration:none; border:none;" target="_blank"><img src="https://i.imgur.com/7HLEEkQ.png" border"0"="" style="display:block; width:600px;"></a>
                                                    <a href="#" style="text-decoration:none; border:none;" target="_blank"><img src="https://i.imgur.com/hMaBWRO.png" border"0"="" style="display:block; width:600px;"></a>
                                                    <a href="#" style="text-decoration:none; border:none;" target="_blank"><img src="https://i.imgur.com/EpauB2F.png" border"0"="" style="display:block; width:600px;"></a>
                                                    <a href="#" style="text-decoration:none; border:none;" target="_blank"><img src="https://i.imgur.com/jEatPMy.png" border"0"="" style="display:block; width:600px;"></a>
                                                    <a href="#" style="text-decoration:none; border:none;" target="_blank"><img src="https://i.imgur.com/vFtD7O6.png" border"0"="" style="display:block; width:600px;"></a>
                                                    <a href="#" style="text-decoration:none; border:none;" target="_blank"><img src="https://i.imgur.com/1hhCThX.png" border"0"="" style="display:block; width:600px;"></a>
                                                </div>
                                                <!--//FOREGROUND-->


                                            </div>
                                        </div>
                                    </td>
                                </tr>
                                <!--<![endif]-->
                                <!--//DAT JOURNEY THO-->

                                <tr>
                                    <td>
                                        <table class="image_table" style="line-height: 100%;z-index:600;position:relative;" border="0" width="100%" cellpadding="0" cellspacing="0">
                                        <tbody><tr>
                                            <td style="background-color:#ffffff;line-height:1px;font-size:1px;">&nbsp;
                                                <table border="0" width="100%" cellpadding="0" cellspacing="0">
                                                <tbody><tr>
                                                    <td style="padding:0px;">

                                                        <!-- START FALLBACK SECTION -->
                                                        <center>
                                                            <table border="0" width="100%" cellpadding="0" cellspacing="0" class="fallback" style="font-family: &#39;Helvetica Neue&#39;, Helvetica; margin: 0; padding: 0;">
                                                            <tbody><tr>
                                                                <td class="padding" style="font-family: &#39;Helvetica Neue&#39;, Helvetica; margin: 0; padding: 0px;">
                                                                    <!--[if (gte mso 9)|(IE)]>
                                                                    <p style="mso-table-lspace:0;mso-table-rspace:0; margin:0">
                                                                    <![endif]-->

                                                                    <div width="100%" style="background-color:#6fdef5;color:#2e2a29;font-size:14px;line-height:30px;text-align:center;">
                                                                        <div style="font-size:35px; line-height:40px; mso-line-height:exactly;">&nbsp;</div>
                                                                        <span class="mv-copy1" style="font-family:Helvetica, Arial, sans-serif; font-size:16px; line-height:12px; font-weight:bold;">HIT THE ROAD THIS SUMMER WITH THE</span><br>
                                                                         <div style="font-size:6px; line-height:6px; mso-line-height:exactly;">&nbsp;</div>
                                                                        <span class="mv-copy2" style="font-family:Georgia, &#39;Times New Roman&#39;, Times, serif; font-size:40px; line-height:36px;">#UnitedStatesofBooks</span><br>
                                                                        <div style="font-size:20px; line-height:20px; mso-line-height:exactly;">&nbsp;</div>
                                                                        <span class="mv-copy3" style="font-family:Helvetica, Arial, sans-serif; font-size:15px; line-height:17px;">Follow along as we celebrate books from sea to shining sea. <br>
                                                                        Click the billboards to discover books set in each state.</span><br>
                                                                           <div style="font-size:18px; line-height:18px; mso-line-height:exactly;">&nbsp;</div>
                                                                        <span class="mv-copy4" style="font-family:Georgia, &#39;Times New Roman&#39;, Times, serif; font-size:30px; line-height:30px; font-weight:bold;">BUCKLE UP.</span>
                                                                        <br>
                                                                        <span class="mv-copy5" style="font-family:Georgia, &#39;Times New Roman&#39;, Times, serif; font-size:18px; line-height:24px; font-weight:bold;">It's going to be a book-y ride!</span>
                                                                    </div>


                                                                    <img src="https://i.imgur.com/bEESZ6G.jpg" border="0" style="display:block;">
                                                                    <a href="#" style="text-decoration:none; border:none;"><img src="https://i.imgur.com/Q9QqGja.png" border="0" style="display:block;"></a>
                                                                    <a href="#" style="text-decoration:none; border:none;"><img src="https://i.imgur.com/CQhERgd.jpg" border="0" style="display:block;"></a>
                                                                    <a href="#" style="text-decoration:none; border:none;"><img src="https://i.imgur.com/OrWci8m.jpg" border="0" style="display:block;"></a>
                                                                    <a href="#" style="text-decoration:none; border:none;"><img src="https://i.imgur.com/g9A8hBI.jpg" border="0" style="display:block;"></a>
                                                                   <a href="#" style="text-decoration:none; border:none;"><img src="https://i.imgur.com/klz8788.jpg" border="0" style="display:block;"></a>
                                                                    <a href="#" style="text-decoration:none; border:none;"><img src="https://i.imgur.com/GnknvKC.jpg" border="0" style="display:block;"></a>
                                                                    <!--[if (gte mso 9)|(IE)]>
                                                                    </p>
                                                                    <![endif]-->
                                                                </td>
                                                            </tr>
                                                            </tbody></table>
                                                        </center>
                                                        <!-- END FALLBACK SECTION -->

                                                        <!-- START INTERACTIVE SECTION -->
                                                        <!--[if !mso 9]><!-->
                                                        <div border="0" width="100%" cellpadding="0" cellspacing="0" class="kinetic" style="mso-hide:all;display:none;max-height:0;overflow:hidden;text-align:center;">&nbsp;
                                                        </div>
                                                        <!--<![endif]-->
                                                        <!-- END INTERACTIVE SECTION -->

                                                    </td>
                                                </tr>
                                                </tbody></table>
                                            </td>
                                        </tr>
                                        </tbody></table>
                                    </td>
                                </tr>
                                </tbody></table>
                            </center>
                    </td>
                </tr>
                </tbody></table>
            </td>
        </tr>
        </tbody></table>
    <!--[if (gte mso 9)|(IE)]>
    </td>
    </tr>
    </table>
    <![endif]-->
    </div>
</center>
```
