- # Problem
	- Formulardaten werden mehrfach gesendet
	- Der Nutzer schickt seine Formulardaten und klickt danach auf _Neu Laden_ im Browser => Daten werden erneut gesendet
	- ![image.png](../assets/image_1650320783263_0.png)
- # Lösung
	- **PRG Pattern** (POST, Redirect, GET)
	- ![image.png](../assets/image_1650320834874_0.png)
	-
	- Man leitet den Browser auf eine Anzeige-Seite um (**Redirect**) und lässt ihn nicht auf der Form-Ziel-Seite
	- ```java
	  reponse.redirect("...")
	  ```
	-