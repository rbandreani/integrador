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
git add REAMDE.md #cargo de nuevo el README.md
git commit -m "Nuevo cambio en la rama navbar"
```






Agrego el repositorio a GitHub
- git remote add origin https://github.com/roquitoit/test.git
- git push -u origin master

Si esto no funciona lo hacemos desde SSH

