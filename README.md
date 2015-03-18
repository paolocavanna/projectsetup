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
	<p><code>npm install -g grunt-cli</code></p>
8. Installare [Bower] [http://bower.io/] globalmente:
	<p><code>npm install -g bower</code></p>
9. Installare i pacchetti di Bower:
	<p><code>bower install</code></p>
10. In Gruntfile.js modificare il proprio localhost:
	<p><code>connect.options.hostname</code>(riga 52)</p> 
11. Eseguire Grunt:
	<p><code>grunt</code></p>
I file su cui lavorare si trovano in:
	- hbs: /src/templates
	- css: /src/css
	- js: /src/js
12. Per aggiornare il browser automaticamente a ogni salvataggio di file, eseguire:
	<p><code>grunt server<code></p>
13. Per compilare il progetto eseguire:
	<p><code>grunt build<code></p>
Navigando nella cartella /build/ si troveranno i file generati
