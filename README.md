Primera práctica: EJERCICIOS GESTIÓN RAMAS

Ejercicio 1
git config --global nombre de usuario
git config --global el email
git config --global color.ui auto
git config --list

Ejercicio 2
mkdir libro
cd libro
git init
dir

Ejercicio 3
git status
echo Capítulo 1: Introducción a Git >> indice.txt
echo Capítulo 2: Flujo de trabajo básico >> indice.txt
echo Capítulo 4: Repositorios remotos >> indice.txt
git status
git add nombre del fichero
git status

Ejercicio 4
git commit -m "Añadido índice del libro"
git status

Ejercicio 5
echo Capítulo 3: Gestión de ramas >> indice.txt
git diff
git commit -m "Añadido capítulo 3 sobre gestión de ramas"

Ejercicio 6
git diff
git commit --amend -m "Añadido capítulo 3 sobre gestión de ramas al índice."
git diff

Segunda práctica: EJERCICIOS DE MANEJO DEL HISTORIAL DE CAMBIOS

Ejercicio 1

git log
mkdir capitulos
echo Git es un sistema de control de versiones ideado por Linus Torvalds. >> capitulos/capitulo1.txt
git add .
git commit -m "Añadido capítulo 1."
git log

Ejercicio 2

echo El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios. >> capitulos/capitulo2.txt
git add .
git commit --amend -m "Añadido capítulo 2"
git diff HEAD-2..HEAD

Ejercicio 3

echo Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas. >> capitulos/capitulo2.txt
git add .
git commit --amend -m "Añadido capítulo 3"
git log
git diff HEAD-1..HEAD

Ejercicio 4

echo Capítulo 5: Conceptos avanzados >> indice.txt
git add .
git commit -m "Añadido capítulo 5 al índice."
git annotate indice.txt

Tercera práctica: EJERCICIOS GESTIÓN RAMAS

Ejercicio 1

cd libro
git branch bibliografia
git checkout bibliografia
git branch -a

Ejercicio 2

Echo capitulo 4 >> capitulo4.txt 
Git add capitulo4.txt 
Git commit –m “Añadido capitulo 4” 
Git log

Ejercicio 3

Git switch bibliografia
Echo Chacon, S. and Straub, B. Pro Git. Apress. >> bibliografía.txt 
Git add bibliografía.txt 
Git commit –m “Añadida primera referencia bibliografica” 
Git log

Ejercicio 4

Git merge master 
Git log 
Git branch –d bibliografia 
Git log 

Ejercicio 5

Git branch bibliografia
Git switch bibliografia
echo Scott Chacon and Ben Straub. Pro Git. Apress. > bibliografia.txt
echo Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014) >> bibliografia.txt
Git add bibliografia.txt
Git commit -m “Añadida nueva referencia bibliográfica”
Git checkout master
echo Chacon, S. and Straub, B. Pro Git. Apress > bibliografia.txt
echo Loeliger, J. and McCullough, M. Version control with Git. >> bibliografia.txt
Git add bibliografia.txt
Git commit –m “Añadida nueva referencia bibliográfica” 
Git merge bibliografia
Echo Chacon, S. and Straub, B. Pro Git. Apress. > bibliografia.txt
Echo Loeliger, J. and McCullough, M. Version control with Git. >> bibliografia.txt
Echo Hodson, R. Ry’s Git Tutorial. Smashwords (2014) >> bibliografia.txt
Git add bibliografia
Git commit –m “Resuelto conflicto de bibliografía” 
Git log

Práctica cuarta: EJERCICIOS DE REPOSITORIOS REMOTOS

Ejercicio 1: 

git branch libro-git
