- # Allgemeines
	- Name-Wert-Paare die **von dem Server erzeugt** und auf dem Client **für eine definierbare Zeit** gespeichert werden.
	- Die Cookies können eine längere Lebensdauer als die Session auf der Serverseite haben, da sie den **Neustart des Browsers überleben**.
	- Die Cookies werden automatisch vom Browser im HTTP-Header übertragen und können **bis zu 4KB groß sein**.
	- Pro Domain dürfen 20 Cookies abgespeichert werden.
- # Umsetzung
	- ## Java Servlets
		- ```java
		  String content = "...";
		  Cookie cookie = new Cookie("name", content);
		  cookie.setMaxAge(60 * 60 * 24 * 7);
		  //               ^^^^^^^^^^^^^^^^ Lebensdauer in Sekunden = 7 Tage
		  cookie.setDomain(".thi.de");
		  //               ^^^^^^^^^ Jede Domain, die mit .thi.de endet
		  cookie.setPath("/Demoprojekt");
		  
		  reponse.addCookie(cookie);
		  ```