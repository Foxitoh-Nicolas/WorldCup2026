WorldCup

La aplicación WorldCup tiene algunos errores que deben ser corregidos:

1- En la pantalla de grupos no se esta mostrando la imagen de fondo (2 Punto)

2- Figura Chile en todos los grupos, remplazarlo por los paises correctos (1 Punto)

3- Cuando se accede al detalle de un grupo siempre muestra los datos del grupo J (3 Puntos)

4- La ruedita de cargando en la pantalla de detalle esta de color Verde, cambiarlo por el mismo color que en la pantalla principal (1 Punto)

5- En el detalle de los grupos esta repetida la palabra Grupo ejemplo: "Grupo Grupo J" (1 Punto)

6- El boton para ir para atras no esta funcionando (2 Puntos)


Ejercicio 1:
Se agrega, dentro del Scaffold, en el Box que va a ocupar el tamaño de la pantalla la invocación al Composable "            BackgroundImage()", antes del when, para que se cargue el logo de fondo.

Ejercicio 2:
En el GrupoView, dentro del Compose GrupoCardView, en el "grupo.teams.forEach", se reemplaza en el Text, el text "chile" por team.

Ejercicio 3:
Dentro del archivo MainActivity, en el composable para ir a DetallePage, se cambia el grupoID que tenia por string "J" por "grupoID = grupoId".

Ejercicio 4:
Se cambia, en DetalleView, la linea del color del Compose de "Cargando" de "color = Color.Green" a "color = MaterialTheme.colorScheme.primaryContainer".

Ejercicio 5:
En el archivo "DetalleView", dentro del Composable "Contenido", se modifica en la Column el Text con el text             "text = "Grupo ${grupo.name}" " por "text = "${grupo.name}" ".

Ejercicio 6:
Dentro de Detalleview, en la topBar, hay un navitation, con un IconButton, que tiene un onClick vació. ahí se agrego onAction(DetalleIntencion.IrParaAtras) para volver a la pantalla anterior.