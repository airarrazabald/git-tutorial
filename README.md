# Git-tutorial

Repositorio para poner en practica git con el paso a paso trabajando con una app en .Net Core

# Preparando el proyecto a versionar

## Ambientación

* So: Windows 10

* git: <https://git-scm.com/downloads>

* dotnet 5 : <https://dotnet.microsoft.com/en-us/download/dotnet/5.0>

Para este tutorial se utiliza visual studio 2019, pero como alternativa podemos utilizar la ultima versión de visual studio 2022, inclusive visual studio code

* Visual Studio Code: <https://code.visualstudio.com/download>

* Visual Studio 2019 community edition (iniciar sesión en dev essentials) : <https://visualstudio.microsoft.com/es/dev-essentials/>

* Visual studio 2022 commnity editionu: <https://visualstudio.microsoft.com/es/vs/>

## Creación del proyecto

Lo primero es abrir el terminal de powershell

Verificamos que el sdk de .net este instalado, ejecutando el siguiente comando en la terminal

```bash
dotnet --version
```

Creamos una carpeta para trabajar nuestro proyecto

```bash
New-Item git-dotnet-tutorial -Type Directory
```

Nos posicionamos en la carpeta creada

```bash
cd .\git-dotnet-tutorial\
```

Creamos una aplicación web api

```bash
dotnet new wepapi
```

Una vez creado ya podemos abrir el proyecto en nuestro IDE Visual studio o Visual Studio Code, de aqui en adelante es opcional la herramienta a utilizar

## Implementando GIT

Verificamos si esta instalado

```bash
git --version
```

Pocisionados en la carpeta de nuestro proyecto debemos inicializar en git

```bash
git init
```

Debemos verificar que archivos estan unatracker

```bash
git status
```

Para agregar estos archivos

```bash
git add .
```

Si verificamos nuevamente el status podremos visualizar los archivos listos para confirmar. Luego confirmamos nuestros cambios con el siguiente comando

```bash
git commit -m "Linea base de nuestro proyecto"
```

Donde -m nos permite agregar el mensaje de confirmación de nuestro cambios

Adicionalmente podemos reducir los camandos anterios con el siguiente

```bash
git commit -am "Linea base de nuestro proyecto"
```

## Creando una nueva rama
