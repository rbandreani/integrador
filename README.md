# Ejercicio Integrador GIT

## Primera Parte
1. Iniciar un nuevo repositorio local en un directorio vacío.
```sh
# Empezamos inicializando y configurando el repositorio local.
git init # inicializo el repositorio
git config --global user.name "usuario"
git config --global user.email "email@email.com"
```

2. Crear un archivo README.md
```sh
# Creamos el archivo y lo precargamos 
touch README.md
git add README.md # si quisiera añadir todos los archivos hago "- git add ."
```

3. Crear un nuevo commit inicial con mensaje "Commit Inicial"
```sh
- git commit -m "Commit Inicial"
git add README.md # si quisiera añadir todos los archivos hago "- git add ."
```

## Segunda Parte
1. Crear una rama con el feature "navbar".
```sh
# primero me aseguro estar en el main
git checkout main
git checkout -b navbar #creo la rama navbar
```

2. Modificar el README.md cambiando su contenido a "NavBar".
```sh
# hago los cambios en el archivo manualmente
```

3. Registrar el commit en el nuevo branch
```sh
git add . #cargo todos aunque solo teengo el README.md
git commit -m "Nuevo cambio en la rama navbar"
```

## Tercera Parte
1. Crear una cuenta en GitHub.
```sh
# creo una cuenta manualmente en GitHub
```

2. Crear un repositorio apto para GitHub Pages (usuario/usuario.github.io).
```sh
# creo un repositorio
# en settings del repositorio, voy a pages
# selecciono la rama y le doy a guardar
# esperar que GitHub cree la pagina
```

3. Subir un documento .html a dicho repositorio con tu nombre.
```sh
# primero debemos conectar el repositorio remoto mediante HTTPS, sino podemos usar SSH
# abrimos la consola dentro de la carpeta del repositorio local
git remote add origin https://github.com/usuario/repositorio
git branch -M main
git add index.html
git commit -m "agrego el html"
git push -u origin main
```

## Cuarta Parte
1. Hacer Fork de https://github.com/nestjs/nest en tu cuenta.
```sh
# primero abrimos el repositorio
# le damos click a fork y configuiramos
```

2. Clonar el repositorio en un cambio local. 
```sh
# abrimos la consola donde tengamos los repositorios locales
git clone https://github.com/usuario/nest
# este nos crea primero la carpeta "nest" y luego los elementos correspondientes al repositorio
```

3. Realizar un cambio en dicho repositorio. 
```sh
# borramos las carpetas sample y scritps
```

4. Registrar el commit.
```sh
# entro a la carpeta de nest
git init 
git remote add nest git@github.com:roquitoit/nest.git
git branch -M main
git commit -m "borro las carpetas sample y scripts"
```

5. Hacer push a los cambios en dicho repositorio
```sh
git push -u nest main
# en github figurara "main had recent pushes time ago
```

## Quinta Parte
1. Clonar el repositorio local de NestJS.
```sh
# vuelvo a la rama master para tener todo como antes
git checkout master
# evito clonar el repositorio local
git clone C:/....
```


2. Buscar en todo el repositorio todas las ocurrencias del decorador "Get".
```sh
git grep -r '@\Get' 
```

3. Buscar en todo el repositorio todas las ocurrencias del decorador "Post".
```sh
git grep -r '@\Post' 
```


4. Buscar en todo el repositorio todas las ocurrencias del decorador "Put".
```sh
git grep -r '@\Put' 
```

5. Buscar en todo el repositorio todas las ocurrencias del decorador "Delete"
```sh
git grep -r '@\Delete' 
```