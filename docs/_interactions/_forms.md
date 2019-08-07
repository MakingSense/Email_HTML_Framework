# Formularios

<iframe height="574" style="width: 100%;" scrolling="no" title="NQLxVW" src="//codepen.io/IgnacioRodrigues/embed/NQLxVW/?height=574&theme-id=0&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/IgnacioRodrigues/pen/NQLxVW/'>NQLxVW</a> by Ignacio Rodrigues
  (<a href='https://codepen.io/IgnacioRodrigues'>@IgnacioRodrigues</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

```html
<form method="GET" action="https://ads.fromdoppler.com/test-emails/">
  <label for="rating" style="display: block;margin-top: 20px;font-family: Arial,sans-serif;font-size: 14px;margin-bottom: 5px">&iquest;Como puntuar&iacute;a la &uacute;ltima webinar?</label>
  <input type="radio" name="rating" value="5" placeholder=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png" alt="">
  <br>
  <input type="radio" name="rating" value="4" placeholder=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt="">
  <br>
  <input type="radio" name="rating" value="3" placeholder=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt="">
  <br>
  <input type="radio" name="rating" value="2" placeholder=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt="">
  <br>
  <input type="radio" name="rating" value="1" placeholder=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-2.png"> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt=""> <img src="http://app2.dopplerfiles.com//Users/55141/Originals/star-1.png" alt="">

  <label for="nombre" style="display: block;margin-top: 20px;font-family: Arial,sans-serif;font-size: 14px;margin-bottom: 5px">&iquest;Que tem&aacute;tica le gustar&iacute;a para el pr&oacute;ximo webinar?</label>
  <select name="tematica" id="tematica" style="padding: 3px;border-radius: 5px">
    <option value=""></option>
    <option value="Tecnolog&iacute;a">Tecnolog&iacute;a</option>
    <option value="Internet">Internet</option>
    <option value="Redes sociales">Redes sociales</option>
    <option value="Automatizaci&oacute;n de tareas">Automatizaci&oacute;n de tareas</option>
  </select>

  <label for="eventos-anteriores" style="display: block;margin-top: 20px;font-family: Arial,sans-serif;font-size: 14px;margin-bottom: 5px">¿Participó en otras webinars anteriores de Doppler?</label>
  <div>
    <input type="checkbox" name="eventos-anteriores-si" value="si">
    <label for="eventos-anteriores-si" style="font-family: Arial,sans-serif;font-size: 14px">Sí</label>
    <input type="checkbox" name="eventos-anteriores-no" value="no">
    <label for="eventos-anteriores-no" style="font-family: Arial,sans-serif;font-size: 14px">No</label>
  </div>

  <label for="comentario" style="display: block;margin-top: 20px;font-family: Arial,sans-serif;font-size: 14px;margin-bottom: 5px">¿Quiere dejar un comentario?</label>
  <textarea name="comentario" id="comentario" cols="35" rows="5"></textarea>

  <input type="hidden" name="email_base" value="[[[Email]]]">
  <input type="hidden" name="cuenta_doppler" value="[[[cuentaendoppler]]]">
  <input type="hidden" name="nombre" value="[[[Nombre]]]">

  <input type="submit" name="submit" value="Enviar" style="display: block;margin-top: 10px;background-color: #FBB224;padding:10px 20px;font-size: 14px;line-height: 14px; font-weight: bold;border:none;border-radius: 7px;color:#ffffff;">
</form>
```
