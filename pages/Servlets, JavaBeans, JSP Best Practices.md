- # JavaBeans
	- Verwendung von **Wrapper Datentypen** z.B. `java.lang.Integer` in den Java Beans
		- Bei Primärschlüsseln => `java.lang.Long`
		- Bei Geldbeträgen => `java.lang.BigDecimal`
		- Bei großen Datenmengen => `byte[]`
- # JSP
	- Keine Verarbeitung in JSPs, sondern nur Anzeige => ^^Keine Methodenaufrufe auf Beans in der JSP^^
		- Kein ~~Java-Code~~ in JSPs, Keine ~~JSP-Aktionselemente~~ => Verwendung von ** [[JSP-EL]] ** und **JSTL**
	- In JPS relative Addressierung => Serlvets haben ihren Stammpfad immer im Root-Verzeichnis `WebContent` oder `webapps`
	  ```jsp
	  <html>
	    <head>
	      <!-- Benötigt, da jetzt bei Weiterleitung & Direktaufruf der Basispfad angepasst wird -->
	      <base href="${pageContext.request.requestURI}"/>
	      <script src="../js/include_js.js"></script>
	    </head>
	  </html>
	  ```
	- [[JSP]] Page header
	  ```jsp
	  <%@ page language="Java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8" %>
	  <%@ page errorPage="fehlerseite.jsp" %>
	  <%@ page isErrorPage="true/false" %>
	  <%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
	  ```
	- Verwenden der Include-Direktive (Automatisiertes Copy and Paste)
	  ```jsp
	  <%@ include file="header.jspf" %>
	  ```
- # Servlets & DB
	- Für Blobs die richtige Größe auf der Datenbankseite auswählen
		- {{embed ((62684af0-fd0f-446b-9fac-ce0ffc6446cb))}}
	- Kein Aufruf der `doGet()` Methode in `doPost()` in einem Servlet
	- ## Redirect und Forwarding
		- Schreibender Zugriff => **Redirect** um [[Doppel-POST-Problem]] zu vermeiden
		- Lesender Zugriff => **Forward**