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
"dependencies": {
    "moment": "^2.30.1",
    "react": "^18.3.1"
  },
  "devDependencies": {
    "eslint": "^9.15.0"
  }

  ## Instalar paquetes de manera global
  `$ npm install -g cowsay`


  npm list: para listar los paquetes instalados en este proyecto
  npm list -g: para listar los paquetes instalados de manera global