## Instalar cosas 
`$ npm install {nombre del paquete}`


## Instalar cosas solo para el desarrollo
ambas opciones son validas, solo que la segunda es la versión abraviada
`$ npm install {nombre del paquete}  --save-dev`
`$ npm install {nombre del paquete}  -D`
Sí no se le coloca ningun flag (todas las cosas que llevan un guión antes) queda como dependencia de producción tambien.
Las dependencias de desarrollo son aquellos paquetes que necesitamos en un proyecto mientras estamos desarrollándolo, pero una vez tenemos el código generado del proyecto, no vuelven a hacer falta


## Instalar una dependencia que si o si va a ser ocupada en producción
`$ npm install {nombre del paquete}  --save`
`$ npm install {nombre del paquete}  -S`
`$ npm install {nombre del paquete}` Esta es la primera manera y sí, será llevada a producción

En el archivo package.json se crean objetos que contienen las dependencias diciendo el ambiente en el que se ejecutarán, las puedes cambiar de posición a mano y se modifica
```json
"dependencies": {
    "moment": "^2.30.1",
    "react": "^18.3.1"
  },
  "devDependencies": {
    "eslint": "^9.15.0"
  }
```


## Instalar paquetes de manera global
`$ npm install -g cowsay`

`npm list` para listar los paquetes instalados en este proyecto
`npm list -g` para listar los paquetes instalados de manera global


## Instalar dependencias de manera opcional
`$ npm install eslint -o`
Al ejecutar el comando sí está global, pasa a opcional


## Probar previamente dependencias para evitar tener problemas 
`$ npm install react-dom --dry-run`
No la instalará solo verá sí no tiene problemas con otras librerías, sí los tiene, te dirá, sí no saldrá todo normal en la consola.
Sí todo está bien puedes instalarlos


## Instalar una versión en particular
`$ npm install json-server@0.15.0`
Te instalará esa versión de del paquete


## Instalar la versión más reciente de un paquete
`$ npm install json-server@latest`
Instalará la versión más reciente de un paquete, sí tienes una versión antigua, al actualizará


## Instalar dependencias de un proyecto que clone
`$ npm install`
Leerá el package.json e instalará las dependencias tanto las de producción (las normales) como las de desarrollo