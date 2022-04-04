- ```html
  <input type="..."/>
  ```
- # Eingabe von Text
	- `text`
	- `password`
	- `tel`
	- `url`
	- `email`
- # Eingabe von Zeitangabe
	- `date`
	- `datetime`
	- `datetime-local`
	- `week`
	- `month`
	- `time`
- # Eingabe von Zahlen
	- `number`
	- `range`
- # Treffen einer Auswahl
	- `radio`
	  ```html
	  <!-- Das Label wird den Radio-Button zugeordnet, somit kann auch das
	   Label angeklickt werden -->
	  <input id="r1" type="radio" name="room" value="budged"/>
	  	<label for="r1">Budged</label>
	  ```
	- `checkbox`
	- ```html
	  <select multiple name="thema" size=3>
	    <option value="thema1">Thema 1</option>
	    <option value="thema2">Thema 2</option>
	  </select>
	  <!-- Bei der Absendung werden bei Mehrfachauswahl einfach mehrere
	   Einträge im Query String mit dem namen "thema" gesendet
	  	z.B. ?thema=thema1&thema=thema2-->
	  ```
- # Auslösen von Benutzerinterkationen
	- `button`
	- `submit`
	- `image`
	- `reset`
	- Jedoch sind diese veraltet, man verwendet nun **Buttons**, mit denen mach die `form` attribute überschreiben kann (z.B. um die Daten an unterschiedliche Endpunkte zu senden)
	  ```html
	  <button type="submit">Absenden</button>
	  ```
- # Sonstige
	- `hidden`
	- `file`
	  ```html
	  <input type="file" enctype="multipart/form-data">
	  ```
	- `color`