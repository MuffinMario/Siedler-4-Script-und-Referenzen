![image from chip.de / icon](http://www.chip.de/ii/4069248_8f0d7ea928.gif)
# Siedler-4-Script-und-Referenzen
Eine Liste vieler Scripte vieler Missionen und eine .rtf Datei die Informationen über die verschiedenen Funktionen gibt. Von mir erstellt vor 2 Jahren (2015). Die .txt dateien stammen von ANDY

# HOW TO: Lua-Script aus einer Map ziehen
Es gibt viele Möglichkeiten das zu machen. Die Siedler IV erstellt bei speziellen Maps eine spezielle Arbeitsspeicher-Region, in der ein Lua-Script ohne Enkodierung abgespeichert wird.
Ein einfacher Weg diese einfach zu kopieren, wäre mit dem Programm ![Cheat Engine](http://cheatengine.org). Dieses Besitzt ein Memory Viewer. Darin enthalten kann man ganz einfach nach einem Text in dem Arbeitsspeicher suchen. So gut wie alle Lua-Scripts besitzen eine function mit dem namen 
register_functions(). Diese wird vom Spiel selber gelesen und registriert die im Lua Code enthaltenn Funktionen. Somit kann man sehr einfach im Memory Viewer unter Search->Find Memory den text "function register_functions()" eingeben und man findet dort die Speicherregion, in der der Script abgelegt ist. Dort nun nur noch die Anfangs-Adresse und End-Adresse vom Script kopieren, dann auf File->Save Memory Region gehen und die beiden adressen eingeben. Cheat Engine kann dann den Speicher Ausschnitt speichern und diesen kann man dann z.B. mit Notepad++ öffnen bzw. ansehen

Andere Funktionen zu suchen wären "function new_game()" "request_event(" "unrequest_event(" "req_func(". Weitere Funktionen sind in der enthaltenen .RTF Datei zu finden
