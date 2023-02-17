![alt text](https://github.com/Magicjg/curso_git/blob/master/logo/logo.png "Alanjg_")

# Curso git.

## Comandos basicos de git para repositorios con pasos para su practica y aprender a usar git.

***

[Para darle formato a el radme se usa Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

`git init` : Crea un repositorio local. 

`git status` : Dice el estado actual de nuestro repocitorio local.

`git add [archivo/.]` : Agregar los archivos a nuestra area de trabajo para luego hacer el commit se puede hacer con los nombres de los archivos o con el punto se sube todo lo que este en la carpeta.

`git commit [-a] -m "mensaje"` : sirve para verificar el cambio y que se efectuen en el repositorio local el `-m` sirve para el mensaje y se puede utilizar el `-a` como el commit add pero para hacer todo de una sola ves (no recomendado).

`git log [--oneline]`: Dice los commits que hay en mi git local el `oneline` es para que lo muestre en una sola linea. 

`git chekout [identificador]` : Regresar a un comit anterior el identificador es el que aparece en el log y identifica al commit.

`git chekout [nombre de la rama]` : Para volver al estado inicial y poder seguir haciendo cambios.

`git reset [--hard] [identificador]` : Volver a un directorio anterior y borra el que este despues con la opcion hard se borran todos los comimits que esten despues de al que quieres regresar y se borraran por completo.

`git restore [archivo]` : Para recuperar un archivo que hayas borrado pero que este arriba en el commit y asi recuperas ese archivo. 

***

### Crear repositorio en github.

`git remote add origin [url/shh]` : Para conectarnos a el repositorio ya sea con la url o por ssh a donde subiremos nuestro repo.

[Entra aqui para ver la documentacion de el uso de ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=linux).

para crear nuestra llave pribada y publica usamos `ssh-keygen -t ed25519 -C "your_email@example.com"` utiliza el correo de tu cuenta, te pide donde guardar las clabes por defecto es `/home/user/.ssh/`. 

Con ssh para que ya no te pida la contraseña usamos `eval "$(ssh-agent -s)"` y despues `vssh-add ~/.ssh/[nombre de la llave con .pub]` para que ya no pida la contraseña hasta que cerremos esa terminal. 
Hay que recordar subir la llave publica a git hub. 

`git remote -v` : Para ver el origen a donde esta nuestro repo conectado.

`git branch -M [nombre]` : es para cambiar el nombre de la rama pricipal.


`git push -u origin [nombre de la rama]` : Sirve para subir todo al repositorio o sudir los cambios echos al repositorio en linea en github despues del primer push ya no se tierne que utilizar `-u origin`.

`rm -rf [carpeta]` : Para borar la carpeta de la repo localmente por que esta proteguida se usa `-f` de force y `-r` de recursivo por que es una carpeta. 

`git clone [url/ssh]` : Se utiliza para copiar el repositorio en nuestra computadora.                                    

***

### Crear ramas y subir a ramas.

`git chekout -b [nombre de rama]` : Para crear una rama `-b` es de branch.

`git branch`: Para ver todas las ramas que existen.

***

### Hay que agregar la rama ahora a github

`git push -u origin [nobre de la rama]` : Se crea la rama en el servidor remoto de git y origin es el nombre del servidor.


`git pull` : Bajar cambios que se hayan echo.





