- ```html
  <head>
    <title>Title</title>
    <meta name="description" content="Das hier ist die Seitenbeschreibung"/>
    <meta charset="utf-8"/>
    
    <!-- Mit 'base' setzt man den relativen Pfad für alle URLs auf dieser Seite -->
    <base href="http://mypage.com/test"/>
    
    <!-- Mit 'link' bindet man andere Dateien ein -->
    <link rel="stylesheet" type="text/css" href="style.css"/>
    
    <!-- Mit 'script' bindet man JavaScripte ein -->
    <script src="javascript.js"></script>
    
    <!-- Mit 'style' setzt man lokale Style-Sheet Regeln für das HTML Dokument -->
    <style>...</style>
  </head>
  ```
- Der HTML-Head erlaubt genau 1 Titel und mehrere Meta-Elemente
- Weitere Elemente sind nicht erlaubt und machen hier keinen Sinn