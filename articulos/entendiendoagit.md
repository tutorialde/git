
# Entendiendo a Git

Git no es tu enemigo, dale una oprtunidad para entenderlo y tendrás un gran aliado.

Me gusta pensar en git como un camara de grabación de video que es capaz de registrar escenas de un suceso con la diferencia que yo puedo indicarle a esta cámara cuando grabar, pausar o rebobinar la grabación.

Llevando la anterior descripción al contexto de un archivo, imagina que eres capáz de leer su contenido mientras alguien lo está editando. Transforma esta experiencia en un escena de video que puedes pausar, rebobinar y colocar en reproducción nuevamente. Con eso ya tienes lo básico para entender como funciona Git.

## Creando una Escena para grabar

Es probable que cuando uses git la escena ya haya sido creada por otra persona, pero entender como lo hizo te ayudará a amigarte con git. 


Ahora un poco de comandos en la terminal nos ayudará a romper el hielo con git.

Si aún no haz intalado git, te dejo un enlace sobre [como instalar git](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Instalaci%C3%B3n-de-Git)



```bash
git version
```

Si ejecutas el anterior comando, deberás ver algo similar a lo siguiente:


```bash
git version
git version 2.30.2
```

A esta altura te preguntarás como se crea una escena con git, pues se hace con el siguiente comando:

```bash
git init
```

¡Así de simple y rápido.!


Vamos con calma, hay detalles que debemos entender.

- __Locación de la escena__ : La locación de la escena es el directorio o carpeta donde ejecutas el comando _git init_, es decir antes de ejecutarlo debe posicionar la terminal en la carpeta donde grabarás la escena.

```bash
mkdir miescena  # Creando la carpeta de la escena
cd miescena     # posicionando la terminal dentro de la carpeta
git init        # Creando la escena con git       
```

Si estás trabajando con un repositorio creado previamente por alguien más, puede descargar una copia en vez de iniciarlizarlo.

```bash
git clone https://github.com/tutorialde/git.git
```

Si ejecutas el anterior comando, se creará una carpeta llamada git cuyo contenido es este tutorial al completo.

Deberás ver algo similar a lo siguiente:

```bash
git clone https://github.com/tutorialde/git.git
Cloning into 'git'...
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (5/5), 4.75 KiB | 4.75 MiB/s, done.
```


## Ramas

Op! queda algo pendiente, las llamadas ramas o branch en inglés.

Volvamos al ejemplo de la escena de video, pero ahora imagina que estas sentado en una banca de una plaza de juegos de niños. Estás sentado junto a un caballero que no conoces.

Por un momento observas la plaza y ves como un niño pequeño comienza a jugar con arena, a esto lo llamaremos la rama del niño. 

__¿Que podría haber visto el caballero junto a ti en ese mismo momento?__

Bueno, el caballero no se ha percatado del niño, sino que ha visto como un perro ha pasado corriendo por el lugar. Pues tenemos otra rama, la rama del perro.

Resumiendo tenemos dos hechos que suceden al mismo tiempo, 

1. Un niño jugando con arena y 
2. Un perro corriendo..


Puedes pensar en las ramas de git como distintas perspectivas de una misma escena, en una se toma enfoque de un objeto por sobre los demás.

Lo usual es que exista una rama llamada main, para saber en que rama estás mirando usa el siguiente comando:

```bash
git branch
```

Deberás ver algo así:

```bash
git branch
* main
```

Lo que indica que estas mirando a la rama __main__ del repositorio.


Te dejo un listado de preguntas:

- ¿Cómo crear una nueva rama?
- ¿Cómo cambiar a una rama que ha creado otra persona?

Aun falta un pequeño paso para comprender mejor las ramas de git (_ramas remotas_), pero lo veremos más adelante, con esto es suficiente para que git comienze a ser mas amigable a tus ojos.
