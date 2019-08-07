# Carrusel de imagenes

El componente de carrousel se ve en algunos clientes de correo indicados al final, en los clientes de correo que no se ven se renderiza un gif simulando el slider de imagenes.

<iframe height="720" style="width: 100%;" scrolling="no" title="Slide" src="//codepen.io/IgnacioRodrigues/embed/OKQeLa/?height=720&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/OKQeLa/'>Slide</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

Esto va en la cabecera del email:

```html
<style type="text/css">
/* Taking power control over styles */

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
	font-family: AkkuratProLight, Helvetica;
	font-size: 14px;
	mso-margin-top-alt: 0px;
	mso-margin-bottom-alt: 0px;
	mso-padding-alt: 0px 0px 0px 0px;
}
.ExternalClass,  .ExternalClass p,  .ExternalClass span,  .ExternalClass font,  .ExternalClass td,  .ExternalClass div {
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
	padding: 0;/* Forces Outlook desktop to provide a "view in browser link" */
}
.ExternalClass .outlook-button {
	padding: 7px 30px 9px !important;/* Outlook.com does not like line-height:0px => adjusting padding top/bottom on our bulletproof CTA button */
}
</style>
    <!-- TARGETS Outlook 2007/2010/2013 !-->
    <!--[if gte mso 9]>
      <style type="text/css" media="all">
        .outlook-button {
          padding: 7px 30px 9px !important;
        }
      </style>
    <![endif]-->

    <!-- Carousel FALLBACK for Gmail Desktop !-->
    <style type="text/css">
#first {
	float: left;
}
#third {
	float: left;
}
#second {
	float: right;
}
* [summary=gmail] {
	max-width: 600px !important;
	width: 600px !important;
	display: block !important;
	max-height: 100% !important;
	font-size: 12px !important;
	line-height: 100% !important;
	overflow: visible !important;
}
* [summary=gmail] div[char="first"] {
	padding-top: 180px !important;
	width: 49px !important;
	max-width: 49px !important;
}
* [summary=gmail] div[char="first"],  * [summary=gmail] div[char="third"] {
	float: left !important;
}
* [summary=gmail] div[char="second"] {
	float: right !important;
	padding-top: 180px !important;
	width: 49px !important;
	max-width: 49px !important;
}
* [summary=gmail] div[char="first"] img,  * [summary=gmail] div[char="second"] img {
	width: 49px !important;
	max-width: 49px !important;
}
/**Initial State**/

* [summary=gmail] div[char="third"] {
	padding-left: 20px !important;
}
* [summary=gmail] div[char="third"] img[src*="protect2_1"] {
	width: 475px !important;
	max-width: 475px !important;
	display: inline !important;
}
/**Hover effects**/

* [summary=gmail] div[char="first"]:hover ~ div:last-child img[src*="protect2_3"] {
	padding-top: 1px !important;
	max-width: 474px !important;
	width: auto !important;
}
* [summary=gmail] div[char="first"]:hover ~ div:last-child img[src*="protect2_1"],  * [summary=gmail] div[char="first"]:hover ~ div:last-child img[src*="protect2_2"] {
	display: none !important;
}
* [summary=gmail] div[char="second"]:hover ~ div:last-child img[src*="protect2_3"],  * [summary=gmail] div[char="second"]:hover ~ div:last-child img[src*="protect2_1"] {
	display: none !important;
}
* [summary=gmail] div[char="second"]:hover ~ div:last-child img[src*="protect2_2"] {
	padding-top: 1px !important;
	max-width: 474px !important;
	width: auto !important;
}
/*Gmail doesn't show desktop only content*/

* [summary=desktop-hide] {
	display: none !important;
}
/**Safe guard that all non-Gmail email clients will ignore table**/

.gmail {
	display: none !important;
}
</style>
    <style type="text/css">
        /*Show fallback content */

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
        #webkit-only input {
            mso-hide: all;
        }
        /**Fix issue with GalleryIcons on iphone 5 & 4*/

        @media all and (max-width: 321px) {
            #galleryIcons > table {
                width: 80% !important;
            }
            #galleryIcons td {
                padding: 0 !important;
                text-align: center !important;
            }
        }
        /**Target webkit only*/

        @media screen and (-webkit-min-device-pixel-ratio: 0) {
            /* Preheader will show for all non-iOS who can't fully enjoy the carousel */

            .preheader {
                display: none;
                visibility: hidden;
                opacity: 0;
                color: transparent;
                height: 0;
                width: 0;
                line-height: 0px;
                font-size: 0px
            }
			.play-button {
				padding-top: 1px !important
			}

            /*Hide fallback content*/

            table#desktop-hide {
                display: none !important;
            }
            /*Show webkit content*/

            #webkit-only {
                display: block !important;
                max-height: none !important;
                padding-bottom: 35px !important
            }
            /*And here we are.... */
            /* Styling the gallery */
            /* -webkit-tap-highlight-color set to white/transparent will remove the grey flash on iPhone / iPad on tap (hover)*/
            #galleryIcons table {
                position: absolute;
                width: 320px;
                bottom: 0;
                margin: 0 auto;
                left: 20px;
                right: 0;
				-webkit-tap-highlight-color: rgba(0,0,0,0);
				}
            #galleryImgs .bodyImgs img:not(.one) {
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                margin: 0 auto;
				}
            #galleryImgs img.two,
            #galleryImgs img.three {
                display: block !important;
                opacity: 0;
            }
            label {
                cursor: pointer;
            }
            label.left,
            #galleryIcons td:first-child {
                padding-left: 10px;

            }
            label.right,
            #galleryIcons td:last-child {
                padding-right: 10px;

            }
            /**Set initial States of labels**/

            #galleryImgs img {
                transition: 0.6s opacity;
            }
			#galleryIcons div {
	-webkit-backface-visibility: hidden;
}
            div.one {
                width: 82px;
                height: 82px;
                background-image: url(http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/images/thumbnail_1.jpg);
                background-position: -83px 1px;
                background-repeat: no-repeat;
                background-size: 165px 82px;
            }
            div.two {
                width: 82px;
                height: 82px;
                background-image: url(http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/images/thumbnail_2.jpg);
                background-position: -83px 1px;
                background-repeat: no-repeat;
                background-size: 165px 82px;
            }
            div.three {
                width: 82px;
                height: 82px;
                background-image: url(http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/images/thumbnail_3.jpg);
                background-position: -83px 1px;
                background-repeat: no-repeat;
                background-size: 165px 82px;
            }
            div.one:hover,
            div.two:hover,
            div.three:hover {
                background-position: 0px 1px;
            }

            /*Creating initial State through a pre-checked radio button*/

            #initialState:checked ~ #gallery #galleryIcons div.one {
                background-position: 0px 1px;
            }
            #initialState:checked ~ #gallery #galleryImgs label.one {
                display: block !important;
            }
            /*Hover State*/
            /*Have to increase selector inheritance (Hence multiple ID's) to over ride checkbox default states*/

            #container table#gallery td#galleryIcons div.one:hover,
            #container table#gallery td#galleryIcons div.two:hover,
            #container table#gallery td#galleryIcons div.three:hover {
                background-position: 0px 1px;
            }
            /**Hover state for icons not being hovered on so current icon decreases in size**/

            #initialState:checked ~ #gallery #galleryIcons:hover div.one,
            #leftArrow1:checked ~ #gallery #galleryIcons:hover div.three,
            #rightArrow1:checked ~ #gallery #galleryIcons:hover div.two,
            #leftArrow2:checked ~ #gallery #galleryIcons:hover div.one,
            #rightArrow2:checked ~ #gallery #galleryIcons:hover div.three,
            #leftArrow3:checked ~ #gallery #galleryIcons:hover div.two,
            #rightArrow3:checked ~ #gallery #galleryIcons:hover div.one,
            #icon1:checked ~ #gallery #galleryIcons:hover div.one,
            #icon2:checked ~ #gallery #galleryIcons:hover div.two,
            #icon3:checked ~ #gallery #galleryIcons:hover div.three {
                background-position: -83px 1px;
            }
            #initialState:checked ~ #gallery #galleryIcons:hover div.one:hover,
            #leftArrow1:checked ~ #gallery #galleryIcons:hover div.three:hover,
            #rightArrow1:checked ~ #gallery #galleryIcons:hover div.two:hover,
            #leftArrow2:checked ~ #gallery #galleryIcons:hover div.one:hover,
            #rightArrow2:checked ~ #gallery #galleryIcons:hover div.three:hover,
            #leftArrow3:checked ~ #gallery #galleryIcons:hover div.two:hover,
            #rightArrow3:checked ~ #gallery #galleryIcons:hover div.one:hover,
            #icon1:checked ~ #gallery #galleryIcons:hover div.one:hover,
            #icon2:checked ~ #gallery #galleryIcons:hover div.two:hover,
            #icon3:checked ~ #gallery #galleryIcons:hover div.three:hover {
                background-position: 0px 1px;
            }
            /********Creating functionality************/
            /*Left Arrow Product 1 - Looping to Product 3*/

            #leftArrow1:checked ~ #gallery #galleryImgs img.one,
            #leftArrow2:checked ~ #gallery #galleryImgs img.one {
                opacity: 0;
            }
            #leftArrow1:checked ~ #gallery #galleryImgs img.three {
                opacity: 1;
            }
            #leftArrow1:checked ~ #gallery #galleryImgs label.one,
            #leftArrow2:checked ~ #gallery #galleryImgs label.one {
                display: none;
            }
            #leftArrow1:checked ~ #gallery #galleryImgs label.three {
                display: block !important;
            }
            #leftArrow1:checked ~ #gallery #galleryIcons div.one {
                background-position: -83px 1px;

            }
            #leftArrow1:checked ~ #gallery #galleryIcons div.three {
                background-position: 0px 1px;
            }
            /*Right Arrow Product 1*/

            #rightArrow1:checked ~ #gallery #galleryImgs img.one,
            #rightArrow1:checked ~ #gallery #galleryImgs img.three {
                opacity: 0;
            }
            #rightArrow1:checked ~ #gallery #galleryImgs img.two {
                opacity: 1;
            }
            #rightArrow1:checked ~ #gallery #galleryImgs label.one,
            #rightArrow1:checked ~ #gallery #galleryImgs label.three {
                display: none;
            }
            #rightArrow1:checked ~ #gallery #galleryImgs label.two {
                display: block !important;
            }
            #rightArrow1:checked ~ #gallery #galleryIcons div.one {
                background-position: -83px 1px;
            }
            #rightArrow1:checked ~ #gallery #galleryIcons div.two {
                background-position: 0px 1px;
            }
            /*Left Arrow Product 2*/

            #leftArrow2:checked ~ #gallery #galleryImgs img.two,
            #leftArrow2:checked ~ #gallery #galleryImgs img.three {
                opacity: 0;
            }
            #leftArrow2:checked ~ #gallery #galleryImgs img.one {
                opacity: 1;
            }
            #leftArrow2:checked ~ #gallery #galleryImgs label.two,
            #leftArrow2:checked ~ #gallery #galleryImgs label.three {
                display: none;
            }
            #leftArrow2:checked ~ #gallery #galleryImgs label.one {
                display: block !important;
            }
            #leftArrow2:checked ~ #gallery #galleryIcons div.two {
                background-position: -83px 1px;
            }
            #leftArrow2:checked ~ #gallery #galleryIcons div.one {
                background-position: 0px 1px;
            }
            /*Right Arrow Product 2*/

            #rightArrow2:checked ~ #gallery #galleryImgs img.one,
            #rightArrow2:checked ~ #gallery #galleryImgs img.two {
                opacity: 0;
            }
            #rightArrow2:checked ~ #gallery #galleryImgs img.three {
                opacity: 1;
            }
            #rightArrow2:checked ~ #gallery #galleryImgs label.one,
            #rightArrow2:checked ~ #gallery #galleryImgs label.two {
                display: none;
            }
            #rightArrow2:checked ~ #gallery #galleryImgs label.three {
                display: block !important;
            }
            #rightArrow2:checked ~ #gallery #galleryIcons div.two {
                background-position: -83px 1px;
            }
            #rightArrow2:checked ~ #gallery #galleryIcons div.three {
                background-position: 0px 1px;
            }
            /*Left Arrow Product 3*/

            #leftArrow3:checked ~ #gallery #galleryImgs img.three,
            #leftArrow3:checked ~ #gallery #galleryImgs img.one {
                opacity: 0;
            }
            #leftArrow3:checked ~ #gallery #galleryImgs img.two {
                opacity: 1;
            }
            #leftArrow3:checked ~ #gallery #galleryImgs label.one,
            #leftArrow3:checked ~ #gallery #galleryImgs label.three {
                display: none;
            }
            #leftArrow3:checked ~ #gallery #galleryImgs label.two {
                display: block !important;
            }
            #leftArrow3:checked ~ #gallery #galleryIcons div.three {
                background-position: -83px 1px;
            }
            #leftArrow3:checked ~ #gallery #galleryIcons div.two {
                background-position: 0px 1px;
            }
            /*Right Arrow Product 3 - Looping to Product 1*/

            #rightArrow3:checked ~ #gallery #galleryImgs img.two,
            #rightArrow3:checked ~ #gallery #galleryImgs img.three {
                opacity: 0;
            }
            #rightArrow3:checked ~ #gallery #galleryImgs img.one {
                opacity: 1;
            }
            #rightArrow3:checked ~ #gallery #galleryImgs label.two,
            #rightArrow3:checked ~ #gallery #galleryImgs label.three {
                display: none;
            }
            #rightArrow3:checked ~ #gallery #galleryImgs label.one {
                display: block !important;
            }
            #rightArrow3:checked ~ #gallery #galleryIcons div.three {
                background-position: -83px 1px;
            }
            #rightArrow3:checked ~ #gallery #galleryIcons div.one {
                background-position: 0px 1px;

            }
            /*Icon Product 1*/

            #icon1:checked ~ #gallery #galleryImgs img.two,
            #icon1:checked ~ #gallery #galleryImgs img.three {
                opacity: 0;
                -webkit-backface-visibility: hidden;
                backface-visibility: hidden;

            }
            #icon1:checked ~ #gallery #galleryImgs img.one {
                opacity: 1;
                -webkit-backface-visibility: hidden;
                backface-visibility: hidden;
            }
            #icon1:checked ~ #gallery #galleryIcons div.two,
            #icon1:checked ~ #gallery #galleryIcons div.three {
                background-position: -83px 1px;
            }

			#icon1:checked ~ #gallery #galleryIcons div.one {
                background-position: 0px 1px;
            }
            #icon1:checked ~ #gallery #galleryImgs label.one {
                display: block !important;
            }
            /*Icon Product 2*/

            #icon2:checked ~ #gallery #galleryImgs img.one,
            #icon2:checked ~ #gallery #galleryImgs img.three {
                opacity: 0;
            }
            #icon2:checked ~ #gallery #galleryImgs img.two {
                opacity: 1;
                -webkit-backface-visibility: hidden;
            }
            #icon2:checked ~ #gallery #galleryIcons div.one,
            #icon2:checked ~ #gallery #galleryIcons div.three {
                background-position: -83px 1px;
            }
            #icon2:checked ~ #gallery #galleryIcons div.two {
                background-position: 0px 1px;
            }
            #icon2:checked ~ #gallery #galleryImgs label.two {
                display: block !important;
            }
            /*Icon Product 3*/

            #icon3:checked ~ #gallery #galleryImgs img.one,
            #icon3:checked ~ #gallery #galleryImgs img.two {
                opacity: 0;
            }
            #icon3:checked ~ #gallery #galleryImgs img.three {
                opacity: 1;
            }
            #icon3:checked ~ #gallery #galleryIcons div.one,
            #icon3:checked ~ #gallery #galleryIcons div.two {
                background-position: -83px 1px;
            }
            #icon3:checked ~ #gallery #galleryIcons div.three {
                background-position: 0px 1px;
            }
            #icon3:checked ~ #gallery #galleryImgs label.three {
                display: block !important;
            }
        }
        /* Global style for mobile devices */

        @media only screen and (max-width: 736px) {
            #galleryIcons table {
                left: 10px;
            }.hide {
                display: none !important;
            }
            td[class="icons"] {
                height: 80px !important;
            }
            .pb0 {
                padding-bottom: 0px !important
            }
            .cb {
                line-height: 19px !important;
                text-align: left !important;
                padding-left: 0px !important;
                padding-right: 0px !important;
            }
			.play-button {
				padding-top: 1px !important
			}
            *[class="mobile"] {
                display: block !important;
                width: 100% !important
            }
            *[class="mobile-hide"] {
                display: none !important
            }
            *[class="desktop-hide"] {
                display: none !important;
                max-height: 0px !important;
            }
            *[class="cta-bottom"] {
                display: block !important;
                max-height: 100% !important;
                font-size: 12px !important;
                line-height: 100% !important;
                overflow: visible !important;
                padding-bottom: 35px !important
            }
            [class="hl"] {
                padding-top: 25px !important;
            }
            [class="pb5"] {
                padding-bottom: 5px !important;
            }
            [class="pt30"] {
                padding-top: 30px !important;
            }
        }
        /* Target iPhone 5 and less */

        @media only screen and (min-width: 219px) and (max-width: 374px) {
            [class="hl"] {
                font-size: 30px !important;
                line-height: 33px !important;
                padding-left: 5px !important;
                padding-right: 5px !important
            }
            [class="sl"] {
                font-size: 16px !important;
                line-height: 18px !important;
                padding-top: 3px !important;
                padding-left: 6px !important;
                padding-right: 6px !important
            }
            [class="thb"] {
                width: 80% !important;
            }
            [class="pb10"] {
                padding-bottom: 10px !important;
            }
            [class="pb20"] {
                padding-bottom: 20px !important;
            }
            [class="pc"] {
                padding: 30px 0 5px !important;
            }
            [class="wc"] {
                width: 85% !important;
            }
            .w80 {
                width: 80px !important;
                height: auto !important;
            }
            .w150 {
                width: 220px !important;
                height: auto !important;
            }
            .w160 {
                width: 170px !important;
                height: auto !important;
            }
            .w170 {
                width: 220px !important;
                height: auto !important;
                top: 90px !important;
            }

            [class="pbGallery"] {
                padding-bottom: 130px !important;
            }
            #galleryIcons table {
                left: 10px;
            }
            div.one,
            div.two,
            div.three {
                width: 75px;
                height: 75px;
                background-position: -74px 1px;
                background-repeat: no-repeat;
                background-size: 147px 73px
            }
            div.one {
                background-image: url(http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/images/thumbnail_1.jpg);
            }
            div.two {
                background-image: url(http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/images/thumbnail_2.jpg);
            }
            div.three {
                background-image: url(http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/images/thumbnail_3.jpg);
            }
            div.one:focus,
            div.two:focus,
            div.three:focus {
                background-position: -20px 1px;
            }
            #initialState:checked ~ #gallery #galleryIcons:hover div.one,
            #leftArrow1:checked ~ #gallery #galleryIcons:hover div.three,
            #rightArrow1:checked ~ #gallery #galleryIcons:hover div.two,
            #leftArrow2:checked ~ #gallery #galleryIcons:hover div.one,
            #rightArrow2:checked ~ #gallery #galleryIcons:hover div.three,
            #leftArrow3:checked ~ #gallery #galleryIcons:hover div.two,
            #rightArrow3:checked ~ #gallery #galleryIcons:hover div.one,
            #icon1:checked ~ #gallery #galleryIcons:hover div.one,
            #icon2:checked ~ #gallery #galleryIcons:hover div.two,
            #icon3:checked ~ #gallery #galleryIcons:hover div.three {
                background-position: -74px 1px;
            }
            #container table#gallery td#galleryIcons div.one:hover,
            #container table#gallery td#galleryIcons div.two:hover,
            #container table#gallery td#galleryIcons div.three:hover {
                background-position: 0px 1px;
            }
            /*Icons*/

            #icon1:checked ~ #gallery #galleryIcons div.two,
            #icon1:checked ~ #gallery #galleryIcons div.three,
            #icon2:checked ~ #gallery #galleryIcons div.one,
            #icon2:checked ~ #gallery #galleryIcons div.three,
            #icon3:checked ~ #gallery #galleryIcons div.one,
            #icon3:checked ~ #gallery #galleryIcons div.two {
                background-position: -74px 1px;
            }
            #icon1:checked ~ #gallery #galleryIcons div.one,
            #icon2:checked ~ #gallery #galleryIcons div.two,
            #icon3:checked ~ #gallery #galleryIcons div.three {
                background-position: 0px 1px;
            }
        }
        /* Target iPhone 6 */

        @media only screen and (min-width: 375px) and (max-width: 413px) {

            [class="hl"] {
                font-size: 35px !important;
                line-height: 37px !important;
            }
            [class="sl"] {
                font-size: 17px !important;
                line-height: 20px !important;
                padding-top: 3px;
            }
            [class="thb"] {
                width: 300px !important;
            }
            [class="pb10"] {
                padding-bottom: 10px !important;
            }
            [class="pb20"] {
                padding-bottom: 20px !important;
            }
            [class="pc"] {
                padding: 30px 0 5px !important;
            }
            [class="wc"] {
                width: 85% !important;
            }
            .w80 {
                width: 80px !important;
                height: auto !important;
            }
            .w150 {
                width: 245px !important;
                height: auto !important;
            }
            .w160 {
                width: 161px !important;
                height: auto !important;
            }
            .w170 {
                width: 250px !important;
                height: auto !important;
                top: 100px !important;
            }
        }
        /* Target iPhone 6+ */

        @media only screen and (min-width: 414px) and (max-width: 736px) {
            [class="thb"] {
                width: 310px !important;
            }
            [class="hl"] {
                font-size: 40px !important;
                line-height: 42px !important;
            }
            [class="right"] {
                display: none !important;
            }
            [class="sl"] {
                font-size: 19px !important;
                line-height: 21px !important;
                padding-top: 3px;
            }
            [class="pb10"] {
                padding-bottom: 10px !important;
            }
            [class="pb20"] {
                padding-bottom: 20px !important;
            }
            [class="pc"] {
                padding: 30px 0 5px !important;
            }
            [class="wc"] {
                width: 88% !important;
            }
            .w80 {
                width: 90px !important;
                height: auto !important;
            }
            .w150 {
                width: 260px !important;
                height: auto !important;
            }
            .w160 {
                width: 200px !important;
                height: auto !important;
            }
            .w170 {
                width: 290px !important;
                height: auto !important;
                top: 100px !important;
            }
        }
    </style>
```

Esta parte va en el cuerpo del email:

```html
<div class="preheader" style="position: relative; width:100%; margin-left:auto; margin-right:auto; font-size:1px; line-height:1px; display: none; color:#f2f3f3; background-color: #f2f3f3;">The new Nest Protect. The smoke alarm other alarms look up&nbsp;to.</div>
<div class="preheader" style="position: relative; width:100%; margin-left:auto; margin-right:auto;font-family:AkkuratProLight, Helvetica, Arial, sans-serif; font-size:11px; line-height:14px; color:#7b858e; background-color: #f2f3f3; padding-bottom: 5px; padding-top:5px; text-align: center"> There's more to see. <a href="http://marketing-assets.nest.com/email-assets/images/marketing/announcement/protect-2/T2_announcement_nest_c_en_US.html?utm_campaign=protect-2-launch-2015&amp;utm_medium=email&amp;utm_source=nest&amp;utm_content=web-version" target="_blank" style="font-family: &#39;FullerSansDT Regular&#39;, Helvetica, Arial, sans-serif; color: #00afd8; text-decoration: none; -webkit-text-size-adjust:none;">Click here</a> to get the full interactive&nbsp;experience.</div>
<div style="position: relative; width:100%; background-color: #ffffff; margin-left:auto; margin-right:auto;">
      <table align="center" border="0" cellpadding="0" cellspacing="0" id="container" style="background-color: #ffffff; border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt" width="100%">
    <tbody><tr>
          <td align="center" style="border-collapse: collapse;" width="100%"><div style="position: relative; width: 100%; max-width: 700px; margin: 0 auto">

              <!--Webkit Only-->
              <div id="webkit-only" class="mobile" style="font-size: 0; max-height: 0; overflow: hidden; display: none">
              <!-- Carousel - This is where the magic hapens -->
              <input checked="" id="initialState" name="myradio" style="display:none;" type="radio">
              <input id="leftArrow1" name="myradio" style="display:none;" type="radio">
              <input id="rightArrow1" name="myradio" style="display:none;" type="radio">
              <input id="leftArrow2" name="myradio" style="display:none;" type="radio">
              <input id="rightArrow2" name="myradio" style="display:none;" type="radio">
              <input id="leftArrow3" name="myradio" style="display:none;" type="radio">
              <input id="rightArrow3" name="myradio" style="display:none;" type="radio">
              <input id="icon1" name="myradio" style="display:none;" type="radio">
              <input id="icon2" name="myradio" style="display:none;" type="radio">
              <input id="icon3" name="myradio" style="display:none;" type="radio">
              <table align="center" border="0" cellpadding="0" cellspacing="0" id="gallery" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; position: relative;">
                  <tbody><tr>
                  <td width="275" align="center" id="galleryIcons"><table width="275" border="0" cellpadding="0" cellspacing="0" class="thb" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;">
                      <tbody><tr>
                      <td class="one"><label class="icon" for="icon1">
                          <div class="one"></div>
                          </label></td>
                      <td class="two"><label class="icon" for="icon2">
                          <div class="two"></div>
                          </label></td>
                      <td class="three"><label class="icon" for="icon3">
                          <div class="three"></div>
                          </label></td>
                    </tr>
                    </tbody></table></td>
                </tr>
                  <tr>
                  <td id="galleryImgs" valign="top"><table class="mobile-hide" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" width="100%">
                      <tbody><tr>
                      <td class="pb5" align="right" style="padding-bottom: 20px"><label class="one left" for="leftArrow1" style="display: none;"><img height="49" src="https://i.imgur.com/7aeyDjT.jpg" width="49"> </label>
                          <label class="two left" for="leftArrow2" style="display: none;"><img height="49" src="https://i.imgur.com/7aeyDjT.jpg" width="49"> </label>
                          <label class="three left" for="leftArrow3" style="display: none;"><img height="49" src="https://i.imgur.com/7aeyDjT.jpg" width="49"> </label></td>
                      <td align="center" class="bodyImgs" style="position: relative; width: 432px" valign="middle"><img class="one w150" src="https://i.imgur.com/PqO49Q9.jpg" style="max-width: 432px; width: 100%; padding-top:40px" width="492"><img class="two w160" src="https://i.imgur.com/QSxUAPg.jpg" style="display: none; max-width: 492px; width: 100%; padding-top:30px" width="492"><img class="three w170" src="https://i.imgur.com/AHDkuOP.jpg" style="display: none; max-width: 492px; width: 100%; padding-top:40px" width="492"></td>
                      <td class="pb5" align="left" style="padding-bottom: 20px"><label class="one right" for="rightArrow1" style="display: none;"><img height="49" src="https://i.imgur.com/3urHckd.jpg" width="49"> </label>
                          <label class="two right" for="rightArrow2" style="display: none;"><img height="49" src="https://i.imgur.com/3urHckd.jpg" width="49"> </label>
                          <label class="three right" for="rightArrow3" style="display: none;"><img height="49" src="https://i.imgur.com/3urHckd.jpg" width="49"> </label></td>
                    </tr>
                    </tbody></table>
                      <table class="mobile" border="0" cellpadding="0" cellspacing="0" style="display: none; border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" width="100%">
                      <tbody><tr>
                          <td align="center" class="bodyImgs" style="position: relative; width: 492px" valign="middle"><img class="one" src="https://i.imgur.com/LEscjHD.jpg" style="max-width: 492px; width: 100%;" width="492"><img class="two" src="https://i.imgur.com/zQbA30R.jpg" style="display: none; max-width: 492px; width: 89%;" width="492"><img class="three" src="https://i.imgur.com/ezUqMJT.jpg" style="display: none; max-width: 492px; width: 100%;" width="492"></td>
                        </tr>
                    </tbody></table></td>
                </tr>
                  <tr>
                  <td class="icons" height="80" style="font-size:0; line-height:0">&nbsp;</td>
                </tr>
                </tbody></table>
              <!-- /Gallery !-->
            </div>
              <!--<![endif]-->

              <!-- Fallback - No carousel but a sweet animated gif-->
              <table border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt;" width="492" align="center" class="desktop-hide" id="desktop-hide">              <tbody><tr>
                  <td align="center" width="76%" style="position: relative; font-size: 20px; padding-top:30px"><img src="https://i.imgur.com/mKcVPk9.gif" width="492" style="line-height: 285px; font-size: 350px; color:#00afd8" alt="○"></td>
                </tr>
              <tr>
                  <td height="15" style="font-size:0; line-height:0">&nbsp;</td>
                </tr>
            </tbody></table>
              <!-- // Fallback Gallery !-->

              <!-- CTA displayed on mobile !-->
              <div class="cta-bottom" style="font-size: 0; max-height: 0; overflow: hidden; display: none">
              <table align="center" border="0" cellpadding="0" cellspacing="0" style="border-collapse: collapse; mso-table-lspace: 0pt; mso-table-rspace: 0pt; mso-hide:all">
                  <tbody><tr>
                  <td class="outlook-button" align="center" style="background-color: #ffa02f; border-radius: 3px; color:#ffffff; font-family: &#39;FullerSansDT Regular&#39;, Helvetica, Arial, sans-serif; font-size:14px; padding: 8px 20px; line-height:18px; font-weight:bold; text-align:center; text-decoration:none; -webkit-text-size-adjust:none; text-transform: uppercase"><a href="https://store.nest.com/product/smoke-co-alarm/?utm_campaign=protect-2-launch-2015&amp;utm_source=nest&amp;utm_content&amp;utm_medium=email&amp;utm_content=buy-now-mobile" target="_blank" style="background-color: #ffa02f; border-radius: 3px; color:#ffffff; font-family: &#39;FullerSansDT Regular&#39;, Helvetica, Arial, sans-serif; font-size:14px; font-weight:bold; text-align:center; text-decoration:none; -webkit-text-size-adjust:none; text-transform: uppercase"> buy now </a></td>
                </tr>
                </tbody></table>
            </div>
              <!-- / CTA displayed on mobile !-->

              <!-- Gmail Android auto-sizing hack - Forcing to display the desktop version in Gmail app. Thanks Justin from Fresh Inbox for the hack!-->
              <div style="display:none; white-space:nowrap; font:15px courier; color:#ffffff;"> - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - </div>
              <!-- !-->
            </div>
          </td>
        </tr>
      </tbody>
    </table>
    </div>
```

> Soporte en clientes de correo

| Clientes de escritorio | Soporte | Clientes de movil | Soporte |
| :------------- | :------------- | :------------- | :------------- |
| Apple Mail 11 (macOS 10.13) | ✅ | Android 4.4 (Android 4.4) | ✅ |
| Apple Mail 12 (Dark Mode) | ✅ | Android 5.1 (Android 5.1) | ⚠️ GIF |
| Color Blindness (simulated) | ✅ | Android 6.0 (Android 6.0) | ⚠️ GIF |
| IBM Notes 10 (Windows 10) | ⚠️ GIF | Gmail App (Android 7.1) | ⚠️ GIF |
| IBM Notes 9 (Windows 10) | ⚠️ GIF | Gmail App (Android 8.0) | ⚠️ GIF |
| Lotus Notes 8.5 (Windows 10) | ⚠️ GIF | Gmail App (iOS 10.3.2) | ⚠️ GIF |
| Outlook 2007 (Windows 10) | ⚠️ GIF | Outlook (Android 7.0)) | ✅ |
| Outlook 2010 (Windows 10) | ⚠️ GIF | Outlook iOS (iOS 11.3.1) | ✅ |
| Outlook 2013  (Windows 10) | ⚠️ GIF | Samsung Mail  (Android 6.0) | ⚠️ GIF |
| Outlook 2013 DPI (Windows 10) | ⚠️ GIF | Samsung Mail (Android 7.0) | ⚠️ GIF |
| Outlook 2016 (macOS 10.12.6) | ⚠️ GIF | iPad (Retina) | ✅ |
| Outlook 2016 (Windows 7) | ⚠️ GIF | iPad Mini (iOS 11.3.2) | ✅ |
| Outlook 2017 (Windows 10) | ⚠️ GIF | iPad Pro (10.5 inch) | ✅ |
| Outlook 2019 (Dark Mode) | ⚠️ GIF | iPad Pro (12.9 inch) | ✅ |
| Outlook 2019 (Windows 10) | ⚠️ GIF | iPhone 6 (iOS 9.3) | ✅ |
| Outlook 2019 (Dark Mode) | ✅ | iPhone 6 Plus (iOS 9.3) | ✅ |
| Outlook 2019 120 DPI (Windows 10) | ✅ | iPhone 6s (iOS 10.3) | ✅ |
| Outlook 2019 120 DPI (Windows 10) | ⚠️ GIF | iPhone 6s Plus (iOS 10.3) | ✅ |
| Windows 10 Mail (Windows 10) | ⚠️ GIF | iPhone 7 (iOS 11.3.1) | ✅ |
| | | iPhone 7 Plus (iOS 11.3.1) | ✅ |
| | | iPhone 8 (iOS 11.3.1) | ✅ |
| | | iPhone 8 Plus (iOS 11.3.1) | ✅ |
| | | iPhone SE (iOS 11.3.1) | ✅ |
| | | iPhone X (iOS 11.3.1) | ✅ |
| | | iPhone XR (iOS 12) | ✅ |
| | | iPhone XS (iOS 12) | ✅ |
| | | iPhone XS Max (iOS 12) | ✅ |
