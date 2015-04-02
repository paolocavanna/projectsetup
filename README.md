# projectsetup
Steps to setup a new poject based on tools like Node.js, Grunt, SASS, Assemble etc.

# INSTALLAZIONE DEL PROGETTO
1. Installare <b>Node.js</b> [http://nodejs.org/download/] se non presente
2. Installare <b>Gist</b> [http://msysgit.github.io/] se non presente
* ATTENZIONE: nell'installare Git selezionare il secondo checkbox "Run Git from the Window command prompt".
https://github.com/bower/bower#a-note-for-windows-users
* ATTENZIONE 2: dal prompt di comandi eseguire:
	<p><code>git config --global url."https://".insteadOf git://</code></p>
Per eseguire le chiamate a Git in https
3. Installare <b>Ruby</b> [http://rubyinstaller.org/downloads/] se non presente
* ATTENZIONE: nell'installare Ruby selezionare il secondo checkbox "Add Ruby executables to your PATH".
Questo permette di eseguire i comandi Ruby dalla shell di Windows
4. Aprire la shell di Ruby e installare Compass (Sass è installato di conseguenza):
	<p><code>gem install compass</code></p>
5. Aprire la shell di Windows
6. Navigare fino alla propria cartella di progetto:
	<p><code>cd /cartella</code></p>
7. Installare <b>Grunt</b> [http://gruntjs.com/] globalmente:
	<p><code>npm install -g grunt-cli</code></p>
	Eseguire <code>grunt -v</code> per assicurarsi della corretta installazione di Grunt.
	<br>
	Se la shell dovesse riportare un errore (es.: <code>"grunt" non è riconosciuto come comando interno o esterno,
 un programma eseguibile o un file batch.</code>), si deve aggiungere <code>npm</code> alle variabili d'ambiente di Windows.
 Per farlo, è necessario eseguire da shell:
 <p><code>path=%PATH%;%APPDATA%\npm</code></p>
8. Installare <b>Bower</b> [http://bower.io/] globalmente:
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
Navigando nella cartella <i>/build/</i> si troveranno i file generati
