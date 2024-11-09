#Command line
- print working directory
```bash
Get inside the thecmdchallenge/ directory:
```
```bash
ls: abre la lista de carpetas
```
```bash
cd thecmdchallenge/: te lleva a la carpeta que quieres
```
```bash
Print current directory path
pwd: te dice donde estás.
```
```bash
List all the files from the current directory including the hidden ones:
ls -a: .  ..  boringfolder  console_master.md  funcode  kamehameha  small-name
```
```bash
Now list all the files inside the project, recursively (all files in the hierarchy)
ls -R:
boringfolder  console_master.md  funcode  kamehameha  small-name

./boringfolder:
babel.png               c9.png    dropzone.js       hello.txt  jquery.png  sass.png      webpack.png
breathecode.shadow.png  css3.png  even-more-boring  html5.png  js.png      scale.fix.js

./boringfolder/even-more-boring:
i-cant-believe-how-boring

./boringfolder/even-more-boring/i-cant-believe-how-boring:
the-ultimate-boring-inception

./boringfolder/even-more-boring/i-cant-believe-how-boring/the-ultimate-boring-inception:
myfirstcopy.txt  the-mostboring-text.txt

./funcode:
baby.jpg             kids.jpg
baby.success.1.jpg   mouse.1.html
baby.success.jpg     mouse.html
borat.success.1.jpg  regexer.1.css
borat.success.jpg    regexer.1.js
einstein.1.png       regexer.css
einstein.png         regexer.js
forms.1.html         rigoberto.1.jpg
forms.html           rigoberto.jpg
frame.1.html         scared-baby.1.jpg
frame.html           scared-baby.jpg
images               script.js
invalid.png          the-most-funny
keyboard.1.html      valid.png
keyboard.html        view-source_projects.breathecode.local_p_php_senior_msql_mysql-tester_.htm
kids.1.jpg

./funcode/images:
hello

./funcode/images/hello:
invalid.png

./funcode/the-most-funny:
lol

./funcode/the-most-funny/lol:
the-ultimate-joke.txt

./kamehameha:
dragon-ball-jokes.md

./small-name:
bigger-name-than-before

./small-name/bigger-name-than-before:
omg-this-folder-has-a-huuuuuuge-name-and-i-tired-to-type

./small-name/bigger-name-than-before/omg-this-folder-has-a-huuuuuuge-name-and-i-tired-to-type:
this-is-probably-the-longest-folder-name-you-have-ever-seen-but-believe--im-sure-there-are-other-folder-bigger-than-this-one-because-people-sometimes-like-to-assign-huge-names-to-their-personal-stuff-supercalifragilisticexpialidocious

./small-name/bigger-name-than-before/omg-this-folder-has-a-huuuuuuge-name-and-i-tired-to-type/this-is-probably-the-longest-folder-name-you-have-ever-seen-but-believe--im-sure-there-are-other-folder-bigger-than-this-one-because-people-sometimes-like-to-assign-huge-names-to-their-personal-stuff-supercalifragilisticexpialidocious:
trophy.txt
```
```bash
Para el ejercicio anterior también hemos encontrado:
find . -type f
```
```bash
clear: borra la pantalla del terminal
```
```bash
Go to the last level below the small-name folder and show on the console the content of the trophy.txt file
find . -name "trophy.txt"
./bigger-name-than-before/omg-this-folder-has-a-huuuuuuge-name-and-i-tired-to-type/this-is-probably-the-longest-folder-name-you-have-ever-seen-but-believe--im-sure-there-are-other-folder-bigger-than-this-one-because-people-sometimes-like-to-assign-huge-names-to-their-personal-stuff-supercalifragilisticexpialidocious/trophy.txt
```
```bash
Move one level up and get to the funcode directory and list all files with the JavaScript typical extension
cd..: para salir de la carpeta anterior
cd funcode: para entrar en esa carpeta
ls: para ver todos los archivos de la carpeta
find . -type f -name "*.js": para localizar solo los archivos javascript.
```
```bash
Create a new directory inside funcode/the-most-funny/ called “not-that-funny“
cd the-most-funny
mkdir "not-that-funny": para crear la carpeta
ls: para ver todos los archivos de the-most-funny y asegurarse
```
```bash
Create a copy of the-mostboring-text.txt (you can find it within /boringfolder/‘s children) and name it lol.txt
find . -name "the-mostboring-text.txt": para encontrar la dirección del documento
cd even-more-boring: entrar en carpeta
hasta encontrar the-ultimate-boring-inception y the-mostboring-text.txt
haces cp the-mostboring-text.txt lol.txt
ls para ver lo creado.
```
```bash
Move funcode/kids.jpg inside funcode/images/hello/
mv kids.jpg hello: para mover ese mismo archivo dentro de hello
también he hecho una búsqueda previa mediante ls y cd para ir entrando y visualizando las carpetas,
también con un find . -name "kids.jpg" para encontrar la dirección.
```
```bash
rm -r small-name: para borrar un directorio no vacío.
solo rm o rmdir no funcionan si el directorio es no vacío.
```
```bash
Print in the command line the content of the-ultimate-joke.txt
What do you call a programmer from Finland? ..... NERDIC!

Got it?? :)
~
~
~
~
~
~
~
(END)
lo hice yendo hasta la carpeta en cuestión, con el procedimiento descrito en anteriores
ejercicios. una vez dentro del archivo escribí: less the-ultimate-joke.txt
```
```bash
llego hasta la lista donde está boringfolder
ahí, de nuevo remuevo un archhivo no vacío con rm -r boringfolder.
```
```bash
Open the file kamehameha/dragon-ball-jokes.md using the VI command line text editor
vi kamehameha/dragon-ball-jokes.md
comando encontrado en la página keepcoding.
```
```bash
con el comando dd se borra la lína sobre la que estés
con el comando w se guardan los cambios
con el comando q se sale del modo ediitor 
con el comando esc se vuelve a la terminal de comandos
```
```bash



@davidmata97-cell ➜ /workspaces/davidexercise-terminal-challenge (master) $ ls
assets      index.js      package.json       README.es.md  slides           webpack.config.js
COMMAND.md  learn.json    package-lock.json  README.md     thecmdchallenge
index.html  node_modules  preview.png        server.js     Untitled
@davidmata97-cell ➜ /workspaces/davidexercise-terminal-challenge (master) $ cd thecmdchallenge/
@davidmata97-cell ➜ /workspaces/davidexercise-terminal-challenge/thecmdchallenge (master) $ pwd
/workspaces/davidexercise-terminal-challenge/thecmdchallenge
@davidmata97-cell ➜ /workspaces/davidexercise-terminal-challenge/thecmdchallenge (master) $ 