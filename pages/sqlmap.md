- Ein Tool zur automatischen Suche nach SQL-Injection-Schwachstellen auf einer Webseite.
- ```shell
  sqlmap 	
  	-u "https://some.web.page" 
      --cookie="C1=1;C2=2" 
      --data="httpParam=value" 
  	-p httpParam
  ```
- Mit `--tables` kann man sich automatisch die Tabellen des DBMS ausgeben lassen
- Mit `-sql-shell` kann direkt eine interaktive SQL-Shell gestartet werden