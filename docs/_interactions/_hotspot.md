# Hotspot

<iframe height="1281" style="width: 100%;" scrolling="no" title="Hotspot" src="//codepen.io/IgnacioRodrigues/embed/vozmKb/?height=1281&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/vozmKb/'>Hotspot</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

Los puntos calientes sirven para agregar información a un producto o articulo, se puede poner una llamada a la acción para comprar el producto o más información a un sitio web externo.

```html
<style type="text/css">
    body {
        -webkit-animation: bugfix infinite 1s
    }

    @-webkit-keyframes bugfix from {
        padding: 0
    }

    to {
        padding: 0
    }

    table {
        border-collapse: collapse;
        mso-table-lspace: 0pt;
        mso-table-rspace: 0pt;
    }

    table td {
        border-collapse: collapse;
    }

    body {
        -ms-text-size-adjust: 100%;
        margin: 0;
        padding: 0;
        color: #7b858e;
        font-family: AkkuratNestBook, Helvetica;
        font-size: 14px;
        mso-margin-top-alt: 0px;
        mso-margin-bottom-alt: 0px;
        mso-padding-alt: 0px 0px 0px 0px;
    }

    .ExternalClass,
    .ExternalClass p,
    .ExternalClass span,
    .ExternalClass font,
    .ExternalClass td,
    .ExternalClass div {
        line-height: 100%;
    }

    .ReadMsgBody {
        width: 100%;
    }

    .ExternalClass {
        width: 100%;
    }

    img {
        outline: none;
        text-decoration: none;
        -ms-interpolation-mode: bicubic;
    }

    a img {
        border: none;
    }

    html {
        -webkit-text-size-adjust: none !important;
    }

    #outlook a {
        padding: 0
    }

    .ExternalClass .outlook-button {
        padding: 7px 30px 9px !important;
        /* Outlook.com does not like line-height:0px => adjusting padding top/bottom on our bulletproof CTA button */
    }

    table#desktop-hide {
        display: block !important;
    }
    /*Hide webkit only section in Outlook 07-13*/

    #webkit-only,
    #webkit-only table,
    #webkit-only tr,
    #webkit-only td,
    #webkit-only img,
    #webkit-only label,
    #webkit-only input,
    #webkit-only div,
    #galleryImgs,
    #bodyImgs {
        mso-hide: all;
    }

    .div-gmail-hack {
        display: none;
    }

    @media screen and (-webkit-min-device-pixel-ratio: 0) {
        .webkit-only-copy {
            display: inline-block !important;
            line-height: 22px !important;
            font-size: 16px !important
        }
        .mobile-show {
            display: none
        }
        table.product-supports tr:first-child td {
            padding-bottom: 5px;
        }
        table.product-supports td img {
            padding: 0 8px 0 0;
        }
        table#desktop-hide {
            display: none !important;
        }
        /*Show webkit content*/
        .webkit-only-copy {
            display: inline !important;
            font-size: 16px !important;
            line-height: 22px !important;
            max-height: 22px !important
        }
        #webkit-only {
            display: block !important;
            max-height: none !important;
            width: 700px;
        }
        #header,
        #gallery {
            width: 680px;
        }
        #galleryImgs .bodyImgs div:not(.divInitial) {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            margin: 0 auto;
        }
        #galleryImgs div.divOne,
        #galleryImgs div.divTwo,
        #galleryImgs div.divThree,
        #galleryImgs div.divFour {
            display: none;
            width: 280px
        }
        label {
            cursor: pointer;
        }
        .background-image {
            position: relative;
            background: url(http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wwn-background-desktop.jpg);
            background-repeat: no-repeat;
            background-size: 100%;
            background-position: 0 15px;
        }
        label div {
            background-size: cover
        }
        label div.pulse-button {
            position: absolute;
            width: 34px;
            height: 34px;
            border: none;
            box-shadow: 0 0 0 0 rgba(0, 174, 214, 0.9);
            border-radius: 50%;
            background-color: #00aed6;
            background-image: url(http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/icons/plus_icon.png);
            background-size: cover;
            background-repeat: no-repeat;
            cursor: pointer;
            -webkit-animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
            -moz-animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
            -ms-animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
            animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
        }
        label[for=product1] div.product-img {
            width: 280px;
            height: 230px;
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wemo-pdt.png');
        }
        label[for=product1] div.pulse-button {
            left: 377px;
            top: 388px;
        }
        label[for=product2] div.product-img {
            width: 210px;
            height: 240px;
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/skybell-pdt.png');
        }
        label[for=product2] div.pulse-button {
            left: 628px;
            top: 647px;
        }
        label[for=product4] div.product-img {
            width: 210px;
            height: 188px;
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/rachio-pdt.png');
        }
        label[for=product4] div.pulse-button {
            left: 400px;
            top: 915px;
        }
        label[for=product3] div.product-img {
            width: 190px;
            height: 240px;
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/lifx-pdt.png');
        }
        label[for=product3] div.pulse-button {
            left: 125px;
            top: 640px;
        }
        /********Creating functionality************/
        /*Product 1 */
        #product1:checked ~ #gallery #galleryImgs div.divInitial,
        #product1:checked ~ #gallery #galleryImgs div.divTwo,
        #product1:checked ~ #gallery #galleryImgs div.divFour,
        #product1:checked ~ #gallery #galleryImgs div.divThree {
            display: none !important;
        }
        #product1:checked ~ #gallery #galleryImgs div.divOne {
            display: block !important;
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=desktop&ea=click-wemo');
        }
        /*Product 2*/
        #product2:checked ~ #gallery #galleryImgs div.divInitial,
        #product2:checked ~ #gallery #galleryImgs div.divOne,
        #product2:checked ~ #gallery #galleryImgs div.divThree,
        #product2:checked ~ #gallery #galleryImgs div.divFour {
            display: none !important;
        }
        #product2:checked ~ #gallery #galleryImgs div.divTwo {
            display: block !important;
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=desktop&ea=click-skybell');
        }
        /*Product 3*/
        #product3:checked ~ #gallery #galleryImgs div.divInitial,
        #product3:checked ~ #gallery #galleryImgs div.divOne,
        #product3:checked ~ #gallery #galleryImgs div.divTwo,
        #product3:checked ~ #gallery #galleryImgs div.divFour {
            display: none !important;
        }
        #product3:checked ~ #gallery #galleryImgs div.divThree {
            display: block !important;
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=desktop&ea=click-lifx');
        }
        /*Product 4*/
        #product4:checked ~ #gallery #galleryImgs div.divInitial,
        #product4:checked ~ #gallery #galleryImgs div.divOne,
        #product4:checked ~ #gallery #galleryImgs div.divTwo,
        #product4:checked ~ #gallery #galleryImgs div.divThree {
            display: none !important;
        }
        #product4:checked ~ #gallery #galleryImgs div.divFour {
            display: block !important;
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=desktop&ea=click-rachio');
        }
        @ -webkit-keyframes pulse {
            to {
                box-shadow: 0 0 0 25px rgba(0, 174, 214, 0);
            }
        }
        @-moz-keyframes pulse {
            to {
                box-shadow: 0 0 0 25px rgba(20, 174, 214, 0);
            }
        }
        @-ms-keyframes pulse {
            to {
                box-shadow: 0 0 0 25px rgba(0, 174, 214, 0);
            }
        }
        @keyframes pulse {
            to {
                box-shadow: 0 0 0 25px rgba(0, 174, 214, 0);
            }
        }
    }

    @media only screen and (max-device-width: 736px) {
        #webkit-only {
            width: 100%;
        }
        .full-width {
            width: 100% !important;
        }
        .mobile-show {
            display: block !important
        }
        .mobile-hide {
            display: none !important
        }
        .show {
            max-height: auto;
            display: none;
            position: relative;
            top: -40px;
            padding: 0px !important;
        }
        .mobile-background {
            background: url(http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wwn-background-mobile.jpg);
        }
        .reset-padding {
            padding: 0 !important;
        }
        .padding-top-0 {
            padding-top: 0px !important;
        }
        .logo {
            padding: 22px 0 !important;
        }
        input[type=checkbox]:checked + div + div + div {
            display: block;
            max-height: auto;
            overflow: all;
            border: none;
            width: 90% !important
        }
        input[type=checkbox]:checked + div + div {
            z-index: 1;
            filter: grayscale(100%);
            -webkit-filter: grayscale(100%);
            -ms-filter: grayscale(100%);
            -ms-transform: rotate(46deg);
            -webkit-transform: rotate(46deg);
            transform: rotate(46deg) scale(0.7);
        }
        label[for=product1-mob] div.product-img {
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wemo-pdt-mob.png');
        }
        label[for=product2-mob] div.product-img {
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/lifx-pdt-mob.png');
        }
        label[for=product3-mob] div.product-img {
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/skybell-pdt-mob.png');
        }
        label[for=product4-mob] div.product-img {
            background-image: url('http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/rachio-pdt-mob.png');
        }
        .pulse-button {
            position: relative !important;
        }
        .hl {
            font-size: 32px !important
        }
        .cta-button {
            width: 90%;
        }
        input[type=checkbox]:checked + div + div + div#divOneMobile {
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=mobile&ea=click-wemo');
        }
        input[type=checkbox]:checked + div + div + div#divTwoMobile {
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=mobile&ea=click-lifx');
        }
        input[type=checkbox]:checked + div + div + div#divThreeMobile {
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=mobile&ea=click-skybell');
        }
        input[type=checkbox]:checked + div + div + div#divFourMobile {
            background-image: url('http://www.google-analytics.com/collect?tid=UA-19609914-25&t=event&cid=0014000000uAAOuAAO&cn=wwn_announce_internal&dl=http://email.nest.com/works_with_nest_announce&cd1=nestcustomers&cs=email&ec=email&cm=m-email&v=1&cm1=1&ul=en_US&cd5=click&el=mobile&ea=click-rachio');
        }
        /* Target iPhone 5 and less */
        @media only screen and (max-device-width: 374px) {
            .font-size-11px {
                font-size: 11px !important;
            }
            .mobile-background {
                background-size: 595px auto;
                background-position: -120px -69px;
            }
            label div.product-img {
                width: 320px;
                height: 235px;
            }
            label[for=product1-mob] div.pulse-button {
                left: 54px;
                top: -183px;
            }
            label[for=product2-mob] div.pulse-button {
                left: 56px;
                top: -195px;
            }
            label[for=product3-mob] div.pulse-button {
                left: 78px;
                top: -178px;
            }
            label[for=product4-mob] div.pulse-button {
                left: 100px;
                top: -165px;
            }
            input[id=product1-mob]:checked + div + div,
            input[id=product3-mob]:checked + div + div,
            input[id=product4-mob]:checked + div + div {
                left: 120px;
                top: 0px;
            }
            input[id=product2-mob]:checked + div + div {
                left: 120px;
                top: 40px;
            }
        }
        /* Target iPhone 6 */
        @media only screen and (min-device-width: 375px) and (max-device-width: 413px) {
            .mobile-background {
                background-size: 640px auto;
                background-position: -120px -69px;
            }
            label div.product-img {
                width: 375px;
                height: 275px;
            }
            label[for=product1-mob] div.pulse-button {
                left: 62px;
                top: -215px;
            }
            label[for=product2-mob] div.pulse-button {
                left: 65px;
                top: -225px;
            }
            label[for=product3-mob] div.pulse-button {
                left: 90px;
                top: -205px;
            }
            label[for=product4-mob] div.pulse-button {
                left: 118px;
                top: -190px;
            }
            input[id=product1-mob]:checked + div + div,
            input[id=product3-mob]:checked + div + div,
            input[id=product4-mob]:checked + div + div {
                left: 140px;
                top: 0px;
            }
            input[id=product2-mob]:checked + div + div {
                left: 140px;
                top: 40px;
            }
        }
        /* Target iPhone 6+ */
        @media only screen and (min-device-width: 414px) and (max-device-width: 736px) {
            .mobile-background {
                background-size: 498px auto;
                background-position: -30px -69px;
            }
            label div.product-img {
                width: 414px;
                height: 303px;
            }
            label[for=product1-mob] div.pulse-button {
                left: 67px;
                top: -233px;
            }
            label[for=product2-mob] div.pulse-button {
                left: 70px;
                top: -245px;
            }
            label[for=product3-mob] div.pulse-button {
                left: 100px;
                top: -225px;
            }
            label[for=product4-mob] div.pulse-button {
                left: 130px;
                top: -210px;
            }
            input[id=product1-mob]:checked + div + div,
            input[id=product3-mob]:checked + div + div,
            input[id=product4-mob]:checked + div + div {
                left: 160px;
                top: 0px;
            }
            input[id=product2-mob]:checked + div + div {
                left: 160px;
                top: 40px;
            }
        }
</style>
```
```html
<div style="position: relative; width:100%; margin-left:auto; margin-right:auto;background-color:#e9eaee">
    <!-- non iOS top line HACK -->
    <div class="padding-top-0" style="mso-hide: all;width: 100%; background-color: #e9eaee; margin-left: auto; margin-right: auto; padding-top: 1px;"></div>
    <!-- /non iOS top line HACK -->
    <table id="webkit-only" align="center" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt" width="100%">
        <tbody>
            <tr>
                <td align="center" style="border-collapse: collapse;" width="100%">
                    <div style="position: relative; width: 100%;margin: 0 auto;">
                        <div id="webkit-only" style=" max-height: 0; overflow: hidden; display: none;border-collapse: collapse; background-color: #FFFFFF">
                            <input id="product1" name="myradio" style="display:none!important" type="radio">
                            <input id="product2" name="myradio" style="display:none!important" type="radio">
                            <input id="product3" name="myradio" style="display:none!important" type="radio">
                            <input id="product4" name="myradio" style="display:none!important" type="radio">
                            <!-- /HEADER-->
                            <table align="center" border="0" cellpadding="0" cellspacing="0" id="gallery" class="background-image mobile-hide" bgcolor="#22428d" style="mso-table-lspace: 0pt; mso-table-rspace: 0pt;">
                                <tbody>
                                    <tr>
                                        <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 44px; line-height:40px; padding: 26px 10px 12px; font-weight: 200">Construye tu casa conectada.</td>
                                    </tr>
                                    <tr>
                                        <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 16px; line-height: 22px; padding: 13px 80px 0; font-weight: 200">Con tantos productos diferentes, puede ser confuso descubrir cómo crear un hogar conectado. Resulta que es algo de lo que sabemos una o dos cosas. Así que elegimos algunos de nuestros productos favoritos de Works with Nest y los agregamos a Nest Store. Son productos que se pueden conectar a Nest para hacer cosas reflexivas y facilitarle la vida.</td>
                                    </tr>
                                    <tr>
                                        <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 16px; line-height: 22px; padding: 15px 80px 17px; font-weight: 200">Comenzamos con interruptores, luces, un timbre y un controlador de rociadores, con más en camino. Haga clic en un producto a continuación para ver cómo funciona con sus productos Nest.</td>
                                    </tr>
                                    <tr>
                                        <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; font-size: 24px; padding: 0 70px;">
                                            <a href="#" style="color:#67d0eb; ; text-decoration: none">Compre ahora > </a>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td id="galleryImgs" valign="top">
                                            <!--[if !gte mso 9]>
                        <!---->
                                            <table align="center" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" width="680">
                                                <tbody>
                                                    <tr>
                                                        <td width="190"></td>
                                                        <td align="center" width="280">
                                                            <label for="product1">
                                                                <div class="product-img"></div>
                                                                <div class="pulse-button"></div>
                                                            </label>
                                                        </td>
                                                        <td align="center" width="210"></td>
                                                    </tr>
                                                    <tr>
                                                        <td align="center" width="190">
                                                            <label for="product3">
                                                                <div class="product-img"></div>
                                                                <div class="pulse-button"></div>
                                                            </label>
                                                        </td>
                                                        <td width="280" align="center" class="bodyImgs" style="position: relative; height:295px">
                                                            <div class="divInitial" style="mso-hide:all;width:280px; color: white; font-size: 40px">
                                                                <table border="0" cellpadding="0" cellspacing="0" style=" border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" width="100%">
                                                                    <tbody>
                                                                        <tr>
                                                                            <td width="280" height="295" align="center" style="color: #4a4a4a; font-size: 14px"></td>
                                                                        </tr>
                                                                    </tbody>
                                                                </table>
                                                            </div>
                                                            <!-- WEMO Card !-->
                                                            <div class="divOne" style="display: none;color: white; font-size: 40px;">
                                                                <table class="full-width" width="280" height="295" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: rgba(255,255,255,0.95)">
                                                                    <tbody>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">Wemo</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                                                <a href="#" style="color: #00AFD8; text-decoration: none">The Wemo Switch</a>can work with Nest to turn off lights, fans and small appliances when you're away. And on when you're back&nbsp;home.</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center">
                                                                                <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                                                <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                    <!--[if !gte mso 9]>
                                                                                                        <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>
                                                                                                    <!--<![endif]-->
                                                                                                </a>
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                                <!-- /CTA BUTTON -->
                                                                            </td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                                                <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td align="left" width="80" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px">Works with</td>
                                                                                            <td align="left" width="80" style="padding-left: 15px; padding-bottom: 5px">Platforms</td>
                                                                                        </tr>
                                                                                        <tr>
                                                                                            <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                                                <img src="https://i.imgur.com/fErR9TE.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                            <td align="left" style="padding-left: 15px">
                                                                                                <img src="https://i.imgur.com/0ZfFqrf.png" width="17" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/PBmzdub.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                            </td>
                                                                        </tr>
                                                                    </tbody>
                                                                </table>
                                                            </div>
                                                            <!-- /WEMO Card !-->
                                                            <!-- SKYBELL Card !-->
                                                            <div class="divTwo" style="display: none;color: white; font-size: 40px">
                                                                <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                                                    <tbody>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">SkyBell</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                                                <a href="#" style="color: #00AFD8; text-decoration: none">The SkyBell HD Wi-Fi Video Doorbell</a>can automatically record video at your front door when Nest&nbsp;Cam detects motion or sound while you're&nbsp;away.</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center">
                                                                                <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                                                <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                    <!--[if !gte mso 9]>
                                                <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                                                    <!--<![endif]-->
                                                                                                </a>
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                                <!-- /CTA BUTTON -->
                                                                            </td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                                                <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td align="left" width="90" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px">Works with</td>
                                                                                            <td align="left" width="70" style="padding-left: 15px; padding-bottom: 5px">Platforms</td>
                                                                                        </tr>
                                                                                        <tr>
                                                                                            <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                                                <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/mYMtcnV.png" width="13" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/Ncm0QOi.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                            <td align="left" style="padding-left: 15px">
                                                                                                <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                            </td>
                                                                        </tr>
                                                                    </tbody>
                                                                </table>
                                                            </div>
                                                            <!-- /SKYBELL Card !-->
                                                            <!-- LIFX Card !-->
                                                            <div class="divThree" style="display: none;color: white; font-size: 40px">
                                                                <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                                                    <tbody>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">LIFX</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                                                <a href="#" style="color: #00AFD8; text-decoration: none">LIFX Color 1000 lights</a>can turn on if Nest&nbsp;Cam senses motion. And when you're away, LIFX lights can randomly switch on and off so it looks like you're&nbsp;home.</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center">
                                                                                <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                                                <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                    <!--[if !gte mso 9]>
                                                <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                                                    <!--<![endif]-->
                                                                                                </a>
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                                <!-- /CTA BUTTON -->
                                                                            </td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                                                <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td align="left" width="120" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px">Works with</td>
                                                                                            <td align="left" width="70" style="padding-left: 15px; padding-bottom: 5px">Platforms</td>
                                                                                        </tr>
                                                                                        <tr>
                                                                                            <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                                                <img src="https://i.imgur.com/KVKDrfr.png" width="20" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/mYMtcnV.png" width="13" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/hRP339H.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                            <td align="left" style="padding-left: 15px">
                                                                                                <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                            </td>
                                                                        </tr>
                                                                    </tbody>
                                                                </table>
                                                            </div>
                                                            <!-- /LIFX Card !-->
                                                            <!-- RACHIO Card !-->
                                                            <div class="divFour" style="display: none;color: white; font-size: 40px">
                                                                <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                                                    <tbody>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">Rachio</td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                                                <a href="#" style="color: #00AFD8; text-decoration: none">The Rachio Smart Sprinkler Controller</a>automatically creates a watering schedule that can lower your water bill. And it shows your savings in your monthly Nest Home&nbsp;Report.
                                                                            </td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center">
                                                                                <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                                                <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                    <!--[if !gte mso 9]>
                                                <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                                                    <!--<![endif]-->
                                                                                                </a>
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                                <!-- /CTA BUTTON -->
                                                                            </td>
                                                                        </tr>
                                                                        <tr>
                                                                            <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px 22px">
                                                                                <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                                                    <tbody>
                                                                                        <tr>
                                                                                            <td align="left" width="80" style="border-right: 1px solid #dcdfe2; padding-bottom:5px">Works with</td>
                                                                                            <td align="left" width="100" style="padding-left: 15px; padding-bottom:5px">Platforms</td>
                                                                                        </tr>
                                                                                        <tr>
                                                                                            <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                                                <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/mYMtcnV.png" width="20" height="20" alt="">
                                                                                            </td>
                                                                                            <td align="left" style="padding-left: 15px">
                                                                                                <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                                                <img src="https://i.imgur.com/yzbT055.png" width="33" height="20" alt="">
                                                                                            </td>
                                                                                        </tr>
                                                                                    </tbody>
                                                                                </table>
                                                                            </td>
                                                                        </tr>
                                                                    </tbody>
                                                                </table>
                                                            </div>
                                                            <!-- /RACHIO Card !-->
                                                        </td>
                                                        <td align="center" width="210">
                                                            <label for="product2">
                                                                <div class="product-img"></div>
                                                                <div class="pulse-button"></div>
                                                            </label>
                                                        </td>
                                                    </tr>
                                                    <tr>
                                                        <td width="190"></td>
                                                        <td align="center" width="280">
                                                            <label for="product4">
                                                                <div class="product-img"></div>
                                                                <div class="pulse-button"></div>
                                                            </label>
                                                        </td>
                                                        <td width="210"></td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                            <!--<![endif]-->
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                            <!-- MOBILE !-->
                            <div class="mobile-show mobile-width" style="display: none;background:url(&#39;http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/texture-pattern_01.jpg&#39;);background-size: 100%">
                                <table border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;">
                                    <tbody>
                                        <tr>
                                            <td align="center" style="color:#ffffff; font-size: 32px; padding: 19px 24px 12px 24px">Build your connected&nbsp;home.&nbsp;</td>
                                        </tr>
                                        <tr>
                                            <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 16px; line-height: 22px; padding: 0 24px">With so many different products out there, it can be confusing to figure out how to create a connected&nbsp;home. Turns out that's something we know a thing or two about. So we've picked out a few of our favorite Works with Nest products and added them to the Nest Store. They're products that can connect to Nest to do thoughtful things and make your life&nbsp;easier.</td>
                                        </tr>
                                        <tr>
                                            <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 16px; line-height: 22px; padding: 15px 24px 17px 24px">We're starting with switches, lights, a doorbell and a sprinkler controller&nbsp;–&nbsp;with more on the way. Click on a product below to see how it works with&nbsp;your&nbsp;Nest&nbsp;products.</td>
                                        </tr>
                                        <tr>
                                            <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif;font-size: 24px; padding: 0 70px 15px">
                                                <a href="#" style="color:#67d0eb; ; text-decoration: none">Shop now &gt;</a>
                                            </td>
                                        </tr>
                                    </tbody>
                                </table>
                            </div>
                            <div class="mobile-show mobile-width mobile-background" style="display: none;">
                                <!-- WEMO Mobile !-->
                                <label for="product1-mob">
                                    <input type="checkbox" id="product1-mob" style="display: none">
                                    <div class="product-img"></div>
                                    <div class="pulse-button"></div>
                                    <div id="divOneMobile" class="show">
                                        <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                            <tbody>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">Wemo</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                        <a href="#" style="color: #00AFD8; text-decoration: none">The Wemo Switch</a>can work with Nest to turn off lights, fans and small appliances when you're away. And on when you're back&nbsp;home.</td>
                                                </tr>
                                                <tr>
                                                    <td align="center">
                                                        <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                            <!--[if !gte mso 9]>
                                      <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                            <!--<![endif]-->
                                                                        </a>
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                        <!-- /CTA BUTTON -->
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                        <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td align="left" width="80" style="border-right: 1px solid #dcdfe2;padding-bottom:5px">Works with</td>
                                                                    <td align="left" width="80" style="padding-left: 15px;padding-bottom:5px">Platforms</td>
                                                                </tr>
                                                                <tr>
                                                                    <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                        <img src="https://i.imgur.com/KVKDrfr.png" width="20" height="20" alt="">
                                                                    </td>
                                                                    <td align="left" style="padding-left: 15px">
                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                        <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                    </td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </label>
                                <!-- /WEMO Mobile !-->
                                <!-- LIFX Mobile !-->
                                <label for="product2-mob">
                                    <input type="checkbox" id="product2-mob" style="display: none">
                                    <div class="product-img"></div>
                                    <div class="pulse-button"></div>
                                    <div id="divTwoMobile" class="show" style="top:0px">
                                        <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                            <tbody>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">LIFX</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                        <a href="#" style="color: #00AFD8; text-decoration: none">LIFX Color 1000 lights</a>can turn on if Nest&nbsp;Cam senses motion. And when you're away, LIFX lights can randomly switch on and off so it looks like you're&nbsp;home.</td>
                                                </tr>
                                                <tr>
                                                    <td align="center">
                                                        <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                            <!--[if !gte mso 9]>
                                      <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                            <!--<![endif]-->
                                                                        </a>
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                        <!-- /CTA BUTTON -->
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                        <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td align="left" width="120" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px">Works with</td>
                                                                    <td align="left" width="100" style="padding-left: 15px; padding-bottom: 5px">Platforms</td>
                                                                </tr>
                                                                <tr>
                                                                    <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                        <img src="https://i.imgur.com/KVKDrfr.png" width="20" height="20" alt="">
                                                                        <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" alt="">
                                                                        <img src="https://i.imgur.com/mYMtcnV.png" width="13" height="20" alt="">
                                                                        <img src="https://i.imgur.com/Ncm0QOi.png" width="20" height="20" alt="">
                                                                    </td>
                                                                    <td align="left" style="padding-left: 15px">
                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                        <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                    </td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </label>
                                <!-- /LIFX Mobile !-->
                                <!-- SkyBell Mobile !-->
                                <label for="product3-mob">
                                    <input type="checkbox" id="product3-mob" style="display: none">
                                    <div class="product-img"></div>
                                    <div class="pulse-button"></div>
                                    <div id="divThreeMobile" class="show">
                                        <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                            <tbody>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">SkyBell</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                        <a href="#" style="color: #00AFD8; text-decoration: none">The SkyBell HD Wi-Fi Video Doorbell</a>can automatically record video at your front door when Nest&nbsp;Cam detects motion or sound while you're&nbsp;away.</td>
                                                </tr>
                                                <tr>
                                                    <td align="center">
                                                        <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                            <!--[if !gte mso 9]>
                                      <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                            <!--<![endif]-->
                                                                        </a>
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                        <!-- /CTA BUTTON -->
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                        <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td align="left" width="90" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px">Works with</td>
                                                                    <td align="left" width="70" style="padding-left: 15px; padding-bottom: 5px">Platforms</td>
                                                                </tr>
                                                                <tr>
                                                                    <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                        <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" alt="">
                                                                        <img src="https://i.imgur.com/mYMtcnV.png" width="13" height="20" alt="">
                                                                        <img src="https://i.imgur.com/Ncm0QOi.png" width="20" height="20" alt="">
                                                                    </td>
                                                                    <td align="left" style="padding-left: 15px">
                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                        <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                    </td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </label>
                                <!-- /SkyBell Mobile !-->
                                <!-- Rachio Mobile !-->
                                <label for="product4-mob">
                                    <input type="checkbox" id="product4-mob" style="display: none">
                                    <div class="product-img"></div>
                                    <div class="pulse-button"></div>
                                    <div id="divFourMobile" class="show">
                                        <table align="center" class="full-width" width="280" height="295" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;background-color: rgba(255,255,255,0.95)">
                                            <tbody>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; color: #7b858e; padding: 25px 22px 1px 22px">Rachio</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 0px 22px 5px 22px; line-height: 18px">
                                                        <a href="#" style="color: #00AFD8; text-decoration: none">The Rachio Smart Sprinkler Controller</a>automatically creates a watering schedule that can lower your water bill. And it shows your savings in your monthly Nest Home&nbsp;Report.
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td align="center">
                                                        <table class="cta-button" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                            <!--[if !gte mso 9]>
                                      <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                            <!--<![endif]-->
                                                                        </a>
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                        <!-- /CTA BUTTON -->
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 11px 0 23px  22px">
                                                        <table class="product-supports" align="center" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" cellpadding="0" cellspacing="0" border="0">
                                                            <tbody>
                                                                <tr>
                                                                    <td align="left" width="80" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px">Works with</td>
                                                                    <td align="left" width="100" style="padding-left: 15px; padding-bottom: 5px">Platforms</td>
                                                                </tr>
                                                                <tr>
                                                                    <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                        <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" alt="">
                                                                        <img src="https://i.imgur.com/Ncm0QOi.png" width="20" height="20" alt="">
                                                                    </td>
                                                                    <td align="left" style="padding-left: 15px">
                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" alt="">
                                                                        <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" alt="">
                                                                        <img src="https://i.imgur.com/yzbT055.png" width="33" height="20" alt="">
                                                                    </td>
                                                                </tr>
                                                            </tbody>
                                                        </table>
                                                    </td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </label>
                            </div>
                            <!-- /Rachio Mobile !-->
                            <!-- /MOBILE !-->
                            <!-- /Gallery !-->
                        </div>
                    </div>
                </td>
            </tr>
        </tbody>
    </table>
    <!-- Fallback !-->
    <div id="desktop-hide" style="position: relative; width:100%; max-width:700px; margin-left:auto; margin-right:auto">
        <table id="desktop-hide" align="center" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; width:700px" width="700">
            <tbody>
                <tr>
                    <td align="center" style="border-collapse: collapse;width:700px" width="700">
                        <!-- /HEADER-->
                        <table align="center" width="100%" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; background-color: #ffffff;" bgcolor="#ffffff" cellpadding="0" cellspacing="0" border="0">
                            <tbody>
                                <tr>
                                    <td class="logo" align="center" style="border-collapse: collapse; padding: 22px 0 22px 20px;">
                                        <img src="https://i.imgur.com/C1mOlX7.png" width="55" height="25" border="0" alt="nest" style="border: none; display: block; -ms-interpolation-mode: bicubic; white-space: pre;">
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                        <!-- /HEADER-->
                        <table bgcolor="#223e7d" align="center" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; width:700px">
                            <tbody>
                                <tr>
                                    <td align="center" background="wwn-background-desktop-fallback-v2.jpg" style="position: relative;  background: url(&#39;http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wwn-background-desktop-fallback-v2.jpg&#39;); background-size: 700px 1440px">
                                        <!--[if !gte mso 15]>
                      <v:image xmlns:v="urn:schemas-microsoft-com:vml" id="theImage" style='behavior: url(#default#VML);height:1360px; width:700px;top:100;left:0;border:0;z-index:1;'
                      src="http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wwn-background-desktop-fallback-v2.jpg"
                      />
                      <v:shape xmlns:v="urn:schemas-microsoft-com:vml" id="theText" style='behavior: url(#default#VML); display:inline-block;position:absolute; height:1360px; width:700px;top:0;left:-10px;border:0;z-index:2;'>
                        <div>
                        <![endif]-->
                                        <!--[if gte mso 15]>
                          <v:image xmlns:v="urn:schemas-microsoft-com:vml" id="theImage" style='behavior: url(#default#VML);height:1360px; width:700px;top:100;left:0;border:0;z-index:1;'
                          src="http://marketing-assets.nest.com.s3.amazonaws.com/email-assets/images/marketing/2016/works-with-nest-announce/wwn-background-desktop-fallback-v2.jpg"
                          />
                          <v:shape xmlns:v="urn:schemas-microsoft-com:vml" id="theText" style='behavior: url(#default#VML); display:inline-block;position:absolute; height:1360px; width:700px;top:0;left:0px;border:0;z-index:2;'>
                            <div>
                            <![endif]-->
                                        <table align="center" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px">
                                            <tbody>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 44px; line-height:40px; padding: 26px 10px 12px; font-weight: 200">Construye tu casa conectada.</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 16px; line-height: 22px; padding: 13px 80px 0; font-weight: 200">Con tantos productos diferentes, puede ser confuso descubrir cómo crear un hogar conectado. Resulta que es algo de lo que sabemos una o dos cosas. Así que elegimos algunos de nuestros productos favoritos de Works with Nest y los agregamos a Nest Store. Son productos que se pueden conectar a Nest para hacer cosas reflexivas y facilitarle la vida.</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; color:#ffffff; font-size: 16px; line-height: 22px; padding: 15px 80px 17px; font-weight: 200">Comenzamos con interruptores, luces, un timbre y un controlador de rociadores, con más en camino. Haga clic en un producto a continuación para ver cómo funciona con sus productos Nest.</td>
                                                </tr>
                                                <tr>
                                                    <td align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; font-size: 24px; padding: 0 70px;">
                                                        <a href="#" style="color:#67d0eb; ; text-decoration: none">Compre ahora > </a>
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td valign="top">
                                                        <table align="center" border="0" cellpadding="0" cellspacing="0" width="700" style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt; mso-padding-alt: 0px;width:700px">
                                                            <tbody>
                                                                <tr>
                                                                    <td width="13" style="width:13px"></td>
                                                                    <td valign="top" style="padding: 18px 0 8px">
                                                                        <!-- WEMO !-->
                                                                        <table align="center" border="0" cellpadding="0" cellspacing="0" width="330" height="480" style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; width:330px; height:480px">
                                                                            <tbody>
                                                                                <tr>
                                                                                    <td bgcolor="#ffffff" align="center">
                                                                                        <a href="#" border="0">
                                                                                            <img src="https://i.imgur.com/gflpIw0.png" width="300" height="auto" alt="">
                                                                                        </a>
                                                                                        <table align="center" class="full-width" width="280" height="240" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="width:280px; height:240px;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px;background-color: rgba(255,255,255,0.95)">
                                                                                            <tbody>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; font-weight: 300; color: #7b858e; padding: 0px 22px 1px 22px">Wemo</td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 14px; padding: 10px 0px 35px; line-height: 18px">
                                                                                                        <a href="#" style="color: #00AFD8; text-decoration: none">The Wemo Switch</a>can work with Nest to turn off lights, fans and small appliances when you're away. And on when you're back&nbsp;home.</td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center">
                                                                                                        <table class="cta-button" style="width:270px;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;  mso-padding-alt: 0px;background-color: #ffa02f; border-radius: 2px; text-align: center" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                                            <tbody>
                                                                                                                <tr>
                                                                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="center">
                                                                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                                            <!--[if !gte mso 9]>
                                                              <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                                                                            <!--<![endif]-->
                                                                                                                        </a>
                                                                                                                    </td>
                                                                                                                </tr>
                                                                                                            </tbody>
                                                                                                        </table>
                                                                                                    </td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 25px 0 23px">
                                                                                                        <table class="product-supports" align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; font-color: #4a4a4a;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; text-align: center" cellpadding="0" cellspacing="0" border="0">
                                                                                                            <tbody>
                                                                                                                <tr>
                                                                                                                    <td align="left" width="80" style="border-right: 1px solid #dcdfe2;padding-bottom:5px;width:80px">Works with</td>
                                                                                                                    <td align="left" width="80" style="padding-left: 15px;padding-bottom:5px;width:80px">Platforms</td>
                                                                                                                </tr>
                                                                                                                <tr>
                                                                                                                    <td align="left" style="border-right: 1px solid #dcdfe2;">
                                                                                                                        <img src="https://i.imgur.com/KVKDrfr.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                    </td>
                                                                                                                    <td align="left" style="padding-left: 15px">
                                                                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                    </td>
                                                                                                                </tr>
                                                                                                            </tbody>
                                                                                                        </table>
                                                                                                    </td>
                                                                                                </tr>
                                                                                            </tbody>
                                                                                        </table>
                                                                                    </td>
                                                                                </tr>
                                                                            </tbody>
                                                                        </table>
                                                                        <!-- /WEMO !-->
                                                                    </td>
                                                                    <td width="13" style="width:13px"></td>
                                                                    <td valign="top" style="padding: 18px 0 8px">
                                                                        <!-- LIFX !-->
                                                                        <table align="center" border="0" cellpadding="0" cellspacing="0" width="330" height="480" style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; width:330px; height:480px">
                                                                            <tbody>
                                                                                <tr>
                                                                                    <td bgcolor="#ffffff" align="center">
                                                                                        <a href="#" border="0">
                                                                                            <img src="https://i.imgur.com/QPfrDXh.png" width="294" height="auto" alt="">
                                                                                        </a>
                                                                                        <table align="center" class="full-width" width="280" height="240" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px;width:280px; height:240px;background-color: rgba(255,255,255,0.95)">
                                                                                            <tbody>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 24px; font-weight: 300; color: #7b858e; padding: 5px 22px 1px 22px">LIFX</td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif; color: #4a4a4a; font-size: 14px; padding: 10px 10px 16px; line-height: 18px">
                                                                                                        <a href="#" style="color: #00AFD8; text-decoration: none">LIFX Color 1000 lights</a>can turn on if Nest&nbsp;Cam senses motion. And when you're away, LIFX lights can randomly switch on and off so it looks like you're&nbsp;home.</td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center">
                                                                                                        <table class="cta-button" style="width:270px;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; ;mso-cellspacing: 0px; mso-padding-alt: 0px;background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                                            <tbody>
                                                                                                                <tr>
                                                                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                                            <!--[if !gte mso 9]>
                                                              <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                                                                            <!--<![endif]-->
                                                                                                                        </a>
                                                                                                                    </td>
                                                                                                                </tr>
                                                                                                            </tbody>
                                                                                                        </table>
                                                                                                    </td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 25px 0 23px">
                                                                                                        <table class="product-supports" align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; font-color: #4a4a4a;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; ;mso-cellspacing: 0px; mso-padding-alt: 0px;text-align: center" cellpadding="0" cellspacing="0" border="0">
                                                                                                            <tbody>
                                                                                                                <tr>
                                                                                                                    <td align="left" width="120" style="border-right: 1px solid #dcdfe2; padding-bottom: 5px; width:120px">Works with</td>
                                                                                                                    <td align="left" width="70" style="padding-left: 15px; padding-bottom: 5px; width:70px">Platforms</td>
                                                                                                                </tr>
                                                                                                                <tr>
                                                                                                                    <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                                                                        <img src="https://i.imgur.com/KVKDrfr.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/mYMtcnV.png" width="13" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/Ncm0QOi.png" width="20" height="20" alt="">
                                                                                                                    </td>
                                                                                                                    <td align="left" style="padding-left: 15px">
                                                                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/ZunsQBV.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                    </td>
                                                                                                                </tr>
                                                                                                            </tbody>
                                                                                                        </table>
                                                                                                    </td>
                                                                                                </tr>
                                                                                            </tbody>
                                                                                        </table>
                                                                                        <!-- /LIFX Card !-->
                                                                                    </td>
                                                                                </tr>
                                                                            </tbody>
                                                                        </table>
                                                                    </td>
                                                                    <td width="13" style="width:13px"></td>
                                                                </tr>
                                                                <tr>
                                                                    <td width="13" style="width:13px"></td>
                                                                    <td valign="top" style="padding: 8px 0 18px">
                                                                        <!-- SkyBell !-->
                                                                        <table align="center" border="0" cellpadding="0" cellspacing="0" width="330" height="480" style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; width:330px; height:480px">
                                                                            <tbody>
                                                                                <tr>
                                                                                    <td bgcolor="#ffffff" align="center">
                                                                                        <a href="#" border="0">
                                                                                            <img src="https://i.imgur.com/kalaYt5.png" width="300" height="auto" alt="">
                                                                                        </a>
                                                                                        <table align="center" class="full-width" width="280" height="290" bgcolor="#FFFFFF" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px;background-color: rgba(255,255,255,0.95);width:280px; height:290px">
                                                                                            <tbody>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; font-weight: 300; color: #7b858e; padding: 0 22px 1px 22px">SkyBell</td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 10px 0px 16px; line-height: 18px">
                                                                                                        <a href="#" style="color: #00AFD8; text-decoration: none">The SkyBell HD Wi-Fi Video Doorbell</a>can automatically record video at your front door when Nest&nbsp;Cam detects motion or sound while you're&nbsp;away.
                                                                                                        <br>
                                                                                                    </td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center">
                                                                                                        <table class="cta-button" style="width:270px;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; mso-cellspacing: 0px; mso-padding-alt: 0px;background-color: #ffa02f; border-radius: 2px" bgcolor="#ffa02f" cellpadding="0" cellspacing="0" border="0">
                                                                                                            <tbody>
                                                                                                                <tr>
                                                                                                                    <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px;" align="left">
                                                                                                                        <a href="#" style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px;">
                                                                                                                            <!--[if !gte mso 9]>
                                                              <!----><span style="padding: 13px 37px; display: block"><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>

                                                                                                                            <!--<![endif]-->
                                                                                                                        </a>
                                                                                                                    </td>
                                                                                                                </tr>
                                                                                                            </tbody>
                                                                                                        </table>
                                                                                                    </td>
                                                                                                </tr>
                                                                                                <tr>
                                                                                                    <td align="center" style="font-size:10px; color:#a7b3bc; padding: 25px 0 23px">
                                                                                                        <table class="product-supports" align="center" style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; font-color: #4a4a4a;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px;text-align: center" cellpadding="0" cellspacing="0" border="0">
                                                                                                            <tbody>
                                                                                                                <tr>
                                                                                                                    <td align="left" width="90" style="border-right: 1px solid #dcdfe2;padding-bottom:5px; width:90px">Works with</td>
                                                                                                                    <td align="left" width="70" style="padding-left: 15px;padding-bottom:5px; width:70px">Platforms</td>
                                                                                                                </tr>
                                                                                                                <tr>
                                                                                                                    <td align="left" style="border-right: 1px solid #dcdfe2">
                                                                                                                        <img src="https://i.imgur.com/hFaODUv.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/mYMtcnV.png" width="13" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/Ncm0QOi.png" width="20" height="20" style="padding-right: 5px" alt="">
                                                                                                                    </td>
                                                                                                                    <td align="left" style="padding-left: 15px">
                                                                                                                        <img src="https://i.imgur.com/hRP339H.png" width="17" height="20" style="padding-right: 5px" alt="">
                                                                                                                        <img src="https://i.imgur.com/ZunsQBV.png width=" 20 " height="20 " style="padding-right: 5px " alt=" ">
                                                                                                                        </td>
                                                                                                                    </tr>
                                                                                                                </tbody>
                                                                                                            </table>
                                                                                                        </td>
                                                                                                    </tr>
                                                                                                </tbody>
                                                                                            </table>
                                                                                        </td>
                                                                                    </tr>
                                                                                </tbody>
                                                                            </table>
                                                                            <!-- SkyBell !-->
                                                                        </td>
                                                                        <td width="13 " style="width:13px "></td>
                                                                        <td valign="top " style="padding: 8px 0 ">
                                                                            <!-- Rachio !-->
                                                                            <table align="center " border="0 " cellpadding="0 " cellspacing="0 " width="330 " height="480 " style="border-collapse: collapse;mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; width:330px; height:480px ">
                                                                                <tbody>
                                                                                    <tr>
                                                                                        <td bgcolor="#ffffff " align="center ">
                                                                                            <a href="# " border="0 ">
                                                                                                <img src="https://i.imgur.com/dkBdl5v.png " width="300 " height="auto " alt=" ">
                                                                                            </a>
                                                                                            <table align="center " class="full-width " width="288 " height="290 " bgcolor="#FFFFFF " border="0 " cellpadding="0 " cellspacing="0 " style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px;width:288px; height:290px;background-color: rgba(255,255,255,0.95) ">
                                                                                                <tbody>
                                                                                                    <tr>
                                                                                                        <td align="center " style="font-family: AkkuratNest-Light, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 24px; font-weight:300; color: #7b858e; padding: 0 22px 1px 22px ">Rachio</td>
                                                                                                    </tr>
                                                                                                    <tr>
                                                                                                        <td align="center " style="font-family: AkkuratNest-Regular, Helvetica, Arial, sans-serif;color: #4a4a4a; font-size: 14px; padding: 10px 0px 16px; line-height: 18px ">
                                                                                                            <a href="# " style="color: #00AFD8; text-decoration: none ">The Rachio Smart Sprinkler Controller</a>automatically creates a watering schedule that can lower your water bill. And it shows your savings in your monthly Nest Home&nbsp;Report.
                                                                                                        </td>
                                                                                                    </tr>
                                                                                                    <tr>
                                                                                                        <td align="center ">
                                                                                                            <table class="cta-button " style="width:270px;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px; background-color: #ffa02f; border-radius: 2px " bgcolor="#ffa02f " cellpadding="0 " cellspacing="0 " border="0 ">
                                                                                                                <tbody>
                                                                                                                    <tr>
                                                                                                                        <td style="border-collapse: collapse; padding: 0; border: 0; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; text-align: center; border-radius: 2px; color: #ffffff; mso-padding-alt: 13px 33px; " align="left ">
                                                                                                                            <a href="# " style="text-decoration: none; color: #ffffff; text-align: center; border-radius: 20px; font-family: &#39;FullerSansDT Bold&#39;, Helvetica, Arial, sans-serif; font-size: 14px; font-weight: bold; line-height: 17px; ">
                                                                                                                                <!--[if !gte mso 9]>
                                                              <!----><span style="padding: 13px 37px; display: block "><!--<![endif]-->COMPRAR<!--[if !gte mso 9]><!----></span>
                                                                                                                                <!--<![endif]-->
                                                                                                                            </a>
                                                                                                                        </td>
                                                                                                                    </tr>
                                                                                                                </tbody>
                                                                                                            </table>
                                                                                                        </td>
                                                                                                    </tr>
                                                                                                    <tr>
                                                                                                        <td align="center " style="font-size:10px; color:#a7b3bc; padding: 25px 0 23px ">
                                                                                                            <table class="product-supports " align="center " style="font-family: AkkuratNest-Book, Helvetica, Arial, sans-serif; font-color: #4a4a4a;border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;mso-cellspacing: 0px; mso-padding-alt: 0px;text-align: center " cellpadding="0 " cellspacing="0 " border="0 ">
                                                                                                                <tbody>
                                                                                                                    <tr>
                                                                                                                        <td align="left " width="80 " style="border-right: 1px solid #dcdfe2;padding-bottom:5px; width:80px ">Works with</td>
                                                                                                                        <td align="left " width="100 " style="padding-left: 15px;padding-bottom:5px; width:100px ">Platforms</td>
                                                                                                                    </tr>
                                                                                                                    <tr>
                                                                                                                        <td align="left " style="border-right: 1px solid #dcdfe2 ">
                                                                                                                            <img src="https://i.imgur.com/hFaODUv.png " width="20 " height="20 " style="padding-right: 5px " alt=" ">
                                                                                                                            <img src="https://i.imgur.com/Ncm0QOi.png " width="20 " height="20 " style="padding-right: 5px " alt=" ">
                                                                                                                        </td>
                                                                                                                        <td align="left " style="padding-left: 15px ">
                                                                                                                            <img src="https://i.imgur.com/hRP339H.png " width="17 " height="20 " style="padding-right: 5px " alt=" ">
                                                                                                                            <img src="https://i.imgur.com/ZunsQBV.png " width="20 " height="20 " style="padding-right: 5px " alt=" ">
                                                                                                                            <img src="https://i.imgur.com/yzbT055.png " width="33 " height="20 " style="padding-right: 5px " alt=" ">
                                                                                                                        </td>
                                                                                                                    </tr>
                                                                                                                </tbody>
                                                                                                            </table>
                                                                                                        </td>
                                                                                                    </tr>
                                                                                                </tbody>
                                                                                            </table>
                                                                                        </td>
                                                                                    </tr>
                                                                                </tbody>
                                                                            </table>
                                                                            <!-- /Rachio !-->
                                                                        </td>
                                                                        <td width="13 "></td>
                                                                    </tr>
                                                                </tbody>
                                                            </table>
                                                        </td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                            <!--[if gte mso 9]>
                </div>
                </v:shape>
              <![endif]-->
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
        <!-- // Fallback !-->
        <!-- FOOTER -->
        <table class="mobile-width " align="center " style="background-color: #e9eaee; width: 100%; border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; " cellpadding="0 " cellspacing="0 " border="0 ">
            <tbody>
                <tr>
                    <td class="reset-padding " align="center " style="padding-bottom: 20px ">
                        <table class="full-width " align="center " width="700 " style="background-color: #FFFFFF; position: relative; border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; " cellpadding="0 " cellspacing="0 " border="0 ">
                            <tbody>
                                <tr>
                                    <td align="center " style="text-align: center; font-family: AkkuratProLight, Helvetica; font-size: 12px; color: #7b858e; line-height: 19px; padding: 45px 0 27px 0; border-collapse: collapse; ">
                                        <table align="center " style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; margin: 0 auto; " cellpadding="0 " cellspacing="0 " border="0 ">
                                            <tbody>
                                                <tr>
                                                    <td align="center " style="border-collapse: collapse; ">
                                                        <a href="# " style="text-decoration: none; color: #00afd8; ">
                                                            <img src="https://i.imgur.com/luhAckh.png " width="9 " height="20 " border="0 " style="border: none; display: block; -ms-interpolation-mode: bicubic; white-space: pre; ">
                                                        </a>
                                                    </td>
                                                    <td width="28 " style="border-collapse: collapse; ">&nbsp;</td>
                                                    <td align="center " style="border-collapse: collapse; ">
                                                        <a href="# " style="text-decoration: none; color: #00afd8; ">
                                                            <img src="https://i.imgur.com/jc2hJIk.png " width="22 " height="17 " border="0 " style="border: none; display: block; -ms-interpolation-mode: bicubic; white-space: pre; ">
                                                        </a>
                                                    </td>
                                                    <td width="26 " style="border-collapse: collapse; ">&nbsp;</td>
                                                    <td align="center " style="border-collapse: collapse; ">
                                                        <a href="# " style="text-decoration: none; color: #00afd8; ">
                                                            <img src="https://i.imgur.com/qGRGEmT.png " width="22 " height="22 " border="0 " style="border: none; display: block; -ms-interpolation-mode: bicubic; white-space: pre; ">
                                                        </a>
                                                    </td>
                                                    <td width="26 " style="border-collapse: collapse; ">&nbsp;</td>
                                                    <td align="center " style="border-collapse: collapse; ">
                                                        <a href="# " style="text-decoration: none; color: #00afd8; ">
                                                            <img src="https://i.imgur.com/RpQjndG.png " width="17 " height="21 " border="0 " style="border: none; display: block; -ms-interpolation-mode: bicubic; white-space: pre; ">
                                                        </a>
                                                    </td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </td>
                </tr>
            </tbody>
        </table>
        <!-- /FOOTER -->
        <!-- INBOX & GMAIL MOBILE HACK -->
        <div class="mobile-hide " style="height: 0px; line-height: 0px; mso-hide: all; ">
          <pre style="width: 600px; white-space: pre; font-size: 0; line-height: 0; height: 0; padding: 0; margin: 0; max-height: 0; "><img src="https://i.imgur.com/7RnX6TT.png " width="1 " height="1 " style="border: none; display: block; -ms-interpolation-mode: bicubic; white-space: pre; " border="0 "></pre>
        </div>
        <div class="div-gmail-hack " style="display: none; white-space: nowrap; font: 15px courier; line-height: 0; ">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
        </div>
        <!-- /INBOX & GMAIL MOBILE HACK -->
    </div>
```
