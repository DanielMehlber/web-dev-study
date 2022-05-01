- # Fehlerseite
	- ```jsp
	  <%@ page errorPage="fehlerausgabe.jsp" %>
	  ```
	- Wenn eine Exception auf dieser Seite erfolgt wird diese an die Fehlerseite weitergegeben
	- In der Fehlerseite hat man bestimmte Beans:
		- `pageContext.exception.stackTrace`