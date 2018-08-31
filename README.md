# CCS APP
## Compilación
El estilo está basado en la plantilla iOS de Ionic, por lo que para verse adecuadamente se requiere compilar como:
```sh
$ ionic serve -t ios
```
Si se tiene problemas con la visualización asegurarse que la URL sea similar a:
```sh
http://localhost:8100/?ionicplatform=ios
```
## Fuentes
Una vez compilado se requiere copiar manualmente el contenido de la carpeta `ccs-fonts/` dentro de `www/assets/fonts/`, las definiciones tipográficas se encuentran al inicio de: `src/app/app.scss`.
## Comentarios
Los comentarios de [pinkxel](http://pinkxel.com/) inician y se pueden buscar con el prefijo `pinkxel:` a lo largo del código intervenido.
## Notas de la segunda revisión de diseño
```sh
Políticas
1. Se agregó las nuevas cabeceras en el .ts
2. Plantilla de políticas

Seguros
1. Todo el recuadro de seguro es un botón
2. Las clases principales son:
.service-wrapper		// Cuerpo del cuadro de seguro
	. head-info			// Información de cabecera (Título y vigencia)
3. Se cambió la función:
openPagar() -> openMore()


Detalle de seguro
	polizSegViaje.nomRiesgo = 'SEGURO DE VIAJE'
		1. Evitar MAYÚSCULAS, de preferencia solo la primera, excepción de siglas por ejemplo: EPS o SCTR Pensiones, evitar: S.C.T.R (puntos)
		2. Se removió ion-item


.textfont-default
	.textfont-detail

Estilo para Material Design
@App({
  templateUrl: 'build/app.html',
  config: {
    mode: 'md'
  }
})

<ion-item style="width: 100%; border: 0px solid #00ffff" no-lines stext-wrap>

color="dark"

.plain
.info

pinkxel: Ya no se requiere este bloque debido a 'no-lines' de ionic


Registro
1. Se cambió el botón de políticas
2. Se quitó estilos en html
3. PROBLEMA de render

<ion-list-header color="guinda">

Minúsculas y : o .

Quitar código que no sirve.


No poner un list dentro de un row se reduce ancho
```

Soporte: <pinkxel@pinkxel.com>