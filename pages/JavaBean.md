- Ein JavaBean stellt das **Model** zur Verfügung
- Es ist weder ein ~~POJO~~, noch eine ~~Enterprise Java Bean~~
- # MVC Muster und Interaktion mit Servlets
	- [[draws/2022-04-11-14-10-20.excalidraw]]
	- Servlet => Control
	- JSP => View
	- JavaBean => Model
	-
- # Sichtbarkeitsbereiche
	- Session Scrope
	- Request Scope
	- Application Scope
		- ```java
		  ServletContext application = request.getServletContext();
		  application.setAttribute("...", "...");
		  ```
- # Normierungen
	- Getter und Setter die sich 1:1 an den Attributnamen anlehnen
		- z.B. `name` => `setName()`, `getName()`
	- Muss der Interface `Serializable` implementieren
	- Muss einen leeren Konstruktor verwenden