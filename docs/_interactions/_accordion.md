# Acordion

<iframe height="265" style="width: 100%;" scrolling="no" title="Menu acordion" src="//codepen.io/IgnacioRodrigues/embed/XvZRjr/?height=265&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/XvZRjr/'>Menu acordion</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

```html
<style type="text/css">@media only screen and (min-width:480px) {
    .mj-column-per-100 {
        width: 100% !important;
        max-width: 100%;
    }
}

</style><style type="text/css">noinput.mj-accordion-checkbox {
    display: block!important;
}

@media yahoo,
only screen and (min-width:0) {
    .mj-accordion-element {
        display: block;
    }
    input.mj-accordion-checkbox,
    .mj-accordion-less {
        display: none!important;
    }
    input.mj-accordion-checkbox + * .mj-accordion-title {
        cursor: pointer;
        touch-action: manipulation;
        -webkit-user-select: none;
        -moz-user-select: none;
        user-select: none;
    }
    input.mj-accordion-checkbox + * .mj-accordion-content {
        overflow: hidden;
        display: none;
    }
    input.mj-accordion-checkbox + * .mj-accordion-more {
        display: block!important;
    }
    input.mj-accordion-checkbox:checked + * .mj-accordion-content {
        display: block;
    }
    input.mj-accordion-checkbox:checked + * .mj-accordion-more {
        display: none!important;
    }
    input.mj-accordion-checkbox:checked + * .mj-accordion-less {
        display: block!important;
    }
}

@goodbye {
    @gmail
}

</style>
```

```html
<div>
    <!--[if mso | IE]><table align="center" border="0" cellpadding="0" cellspacing="0" class="" style="width:600px;" width="600" ><tr><td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;"><![endif]-->
    <div style="background:#ffffff;background-color:#ffffff;Margin:0px auto;max-width:600px;">
        <table align="center" border="0" cellpadding="0" cellspacing="0" role="presentation" style="background:#ffffff;background-color:#ffffff;width:100%;">
            <tbody>
                <tr>
                    <td style="direction:ltr;font-size:0px;padding:20px;text-align:center;vertical-align:top;">
                        <!--[if mso | IE]><table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td class="" style="vertical-align:top;width:560px;" ><![endif]-->
                        <div class="mj-column-per-100 outlook-group-fix" style="font-size:13px;text-align:left;direction:ltr;display:inline-block;vertical-align:top;width:100%;">
                            <table border="0" cellpadding="0" cellspacing="0" role="presentation" style="background-color:#dededd;vertical-align:top;" width="100%">
                                <tr>
                                    <td style="font-size:0px;padding:1px;word-break:break-word;">
                                        <table cell-spacing="0" cell-padding="0" class="mj-accordion" style="width:100%;border-collapse:collapse;border:none;border-bottom:none;font-family:Ubuntu, Helvetica, Arial, sans-serif;">
                                            <tbody>
                                                <tr>
                                                    <td style="padding:0px;">
                                                        <label class="mj-accordion-element" style="font-size:13px;">
                                                            <!--[if !mso | IE]><!-->
                                                            <input class="mj-accordion-checkbox" type="checkbox" style="display:none;">
                                                            <!--<![endif]-->
                                                            <div>
                                                                <div class="mj-accordion-title">
                                                                    <table cell-spacing="0" cell-padding="0" style="width:100%;border-bottom:none;">
                                                                        <tbody>
                                                                            <tr>
                                                                                <td style="width:100%;background-color:#ffffff;color:#031017;font-size:18px;font-family:Roboto, Open Sans, Helvetica, Arial, sans-serif;padding:15px;">Why use an accordion?</td>
                                                                                <!--[if !mso | IE]><!-->
                                                                                <td class="mj-accordion-ico" style="padding:16px;background:#ffffff;vertical-align:middle;"><img src="https://i.imgur.com/b317ERd.png" alt="+" class="mj-accordion-more" style="display:none;width:24px;height:24px;"><img src="https://i.imgur.com/KKHenWa.png" alt="-" class="mj-accordion-less" style="display:none;width:24px;height:24px;"></td>
                                                                                <!--<![endif]-->
                                                                            </tr>
                                                                        </tbody>
                                                                    </table>
                                                                </div>
                                                                <div class="mj-accordion-content">
                                                                    <table cell-spacing="0" cell-padding="0" style="width:100%;border-bottom:none;">
                                                                        <tbody>
                                                                            <tr>
                                                                                <td style="background:#fafafa;font-size:14px;font-family:Open Sans, Helvetica, Arial, sans-serif;color:#505050;padding:15px;"><span style="line-height:20px">Because emails with a lot of content are most of the time a very bad experience on mobile, mj-accordion comes handy when you want to deliver a lot of information in a concise way.</span></td>
                                                                            </tr>
                                                                        </tbody>
                                                                    </table>
                                                                </div>
                                                            </div>
                                                        </label>
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td style="padding:0px;">
                                                        <label class="mj-accordion-element" style="font-size:13px;">
                                                            <!--[if !mso | IE]><!-->
                                                            <input class="mj-accordion-checkbox" type="checkbox" style="display:none;">
                                                            <!--<![endif]-->
                                                            <div>
                                                                <div class="mj-accordion-title">
                                                                    <table cell-spacing="0" cell-padding="0" style="width:100%;border-bottom:none;">
                                                                        <tbody>
                                                                            <tr>
                                                                                <td style="width:100%;background-color:#ffffff;color:#031017;font-size:18px;font-family:Roboto, Open Sans, Helvetica, Arial, sans-serif;padding:15px;">How it works</td>
                                                                                <!--[if !mso | IE]><!-->
                                                                                <td class="mj-accordion-ico" style="padding:16px;background:#ffffff;vertical-align:middle;"><img src="https://i.imgur.com/b317ERd.png" alt="+" class="mj-accordion-more" style="display:none;width:24px;height:24px;"><img src="https://i.imgur.com/KKHenWa.png" alt="-" class="mj-accordion-less" style="display:none;width:24px;height:24px;"></td>
                                                                                <!--<![endif]-->
                                                                            </tr>
                                                                        </tbody>
                                                                    </table>
                                                                </div>
                                                                <div class="mj-accordion-content">
                                                                    <table cell-spacing="0" cell-padding="0" style="width:100%;border-bottom:none;">
                                                                        <tbody>
                                                                            <tr>
                                                                                <td style="background:#fafafa;font-size:14px;font-family:Open Sans, Helvetica, Arial, sans-serif;color:#505050;padding:15px;"><span style="line-height:20px">Content is stacked into tabs and users can expand them at will. If responsive styles are not supported (mostly on desktop clients), tabs are then expanded and your content is readable at once.</span></td>
                                                                            </tr>
                                                                        </tbody>
                                                                    </table>
                                                                </div>
                                                            </div>
                                                        </label>
                                                    </td>
                                                </tr>
                                            </tbody>
                                        </table>
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
```
