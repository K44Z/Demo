# FPT-Ubung1
Current version: Friday Nightly Release Build 1.0
#Beschreibung
In unserer FPT Uebung 1 sollen wir in Gruppen einen Mediaplayer erstellen dazu wurde ein Projektskelet mit 3 Interface zurverfügungg gestellt

Aufgabe war es diese zu implementieren und dazugehörige Funktionalitäten hinzuzüfen.

Hier wird der Fortschritt aktuell gehalten

Friday Nightly Release Build 1.0 
Die Aktuellste Version ist NRB1.0 in dieser Version sind GUI und und diverse Methoden schon vorhanden, aktuell fehlen die Soundausgabe und Editierung von Metadaten.

Patchnotes (Aus Merge Beschreibung)
Short version
increased core readability and added a little fun


Added:
- Interfaces and abstract classes
	- IVieww (Interface), IController(abstract class)
		-both are required for upcoming UI, every UI should follow the same rule
		  View should implement a localization method
		  Controller should implement link method and basic variables such like        
                  View, Applicationmodel and a Hashmap which contains 
                  localization information

- singleton pattern usage: Model, every view

- new method to util
 	- load(Classname: String):HashMap
 		 this method can be used to load localization files
 		 Filecontent: "Objectname:text"
 		 where Objectname should be replaced with UI element and text should be replaced with locale text
  			example: Map<String, String> localeDetailView = core.util.load("DetailView");

Fixed:
- Quiting mainview behaves right, now the application should close, forcibly
- access modifiers: review every variable and modify its access modifiers, each variable should be private,
                  needed variable could be access with getVariablename()

- re-comment every class as a result of the patch
