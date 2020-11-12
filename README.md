# kaambesaj
## El Maestro de Kukulkan OS

# Basado en Mozzarella Ashbadger
Este proyecto lo encontré leyendo el libro que vende el autor de los tutoriales de PyQT.
El material está en Inglés.
Lo transformamos para que sea un navegador HTML que descargará vía GIT las últimas versiones de los tutoriales y ambientes de laboratorio.

Mozarella Ashbadger is the latest revolution in web 
browsing! Go back and forward! Print! Save files! Get help! 
(you’ll need it). Any similarity to other browsers is entirely 
coincidental.

> If you think this app is neat and want to learn more about
PyQt in general, take a look at my [free PyQt tutorials](https://www.learnpyqt.com)
which cover everything you need to know to start building your own applications with PyQt.

## Code notes

### Tabbing

Adding tab support complicates the internals of the browser a bit, since we
now need to keep track of the currently active browser view, both to update
UI elements (URL bar, HTTPs icon) to changing state in the currently active
window, and to ensure the UI events are dispatched to the correct web view.

This is achieved by using intermediate slots which filter events, and by
adding signal redirection (using lamba functions to keep it short).

## Other licenses

Icons used in the application are by [Yusuke Kamiyaman](http://p.yusukekamiyamane.com/).
