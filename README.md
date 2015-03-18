# projectsetup
Steps to setup a new poject based on tools like Node.js, Grunt, SASS, Assemble etc.

# INSTALLAZIONE DEL PROGETTO
1. Installare [Node.js] [http://nodejs.org/download/] se non presente
2. Installare [Gist] [http://msysgit.github.io/] se non presente
* ATTENZIONE: nell'installare Git selezionare il secondo checkbox "Run Git from the Window command prompt".
https://github.com/bower/bower#a-note-for-windows-users
* ATTENZIONE 2: dal prompt di comandi eseguire:
	git config --global url."https://".insteadOf git://
Per eseguire le chiamate a Git in https
3. Installare [Ruby] [http://rubyinstaller.org/downloads/] se non presente
* ATTENZIONE: nell'installare Ruby selezionare il secondo checkbox "Add Ruby executables to your PATH".
Questo permette di eseguire i comandi Ruby dalla shell di Windows
4. Aprire la shell di Ruby e installare Compass (Sass è installato di conseguenza):
	gem install compass
5. Aprire la shell di Windows (Start > cmd > Enter)
6. Navigare fino alla propria cartella di progetto:
	cd /cartella
7. Installare [Grunt] [http://gruntjs.com/] globalmente:
	<code>npm install -g grunt-cli</code>
8. Installare [Bower] [http://bower.io/] globalmente:
	npm install -g bower
9. Installare i pacchetti di Bower:
	bower install
10. In Gruntfile.js modificare il proprio localhost:
	connect.options.hostname (riga 52)
11. Eseguire Grunt:
	grunt
I file su cui lavorare si trovano in:
	- hbs: /src/templates
	- css: /src/css
	- js: /src/js
12. Per aggiornare il browser automaticamente a ogni salvataggio di file, eseguire:
	grunt server
13. Per compilare il progetto eseguire:
	grunt build
Navigando nella cartella /build/ si troveranno i file generati
