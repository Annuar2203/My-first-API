<h1 align = center>Mi primera API con FastAPI:)</h1>

La API creada consiste en crear, leer o consultar, eliminar y actualizar datos temporales (GET,POST,DELETE,PUT). Debido a que no usa base de datos y los datos tienen que ser obligatoriamente creados para guardarlo en memoria, es decir, se utiliza una lista para guardar los diccionarios

<h4>Lenguaje Utilizado: <a href = "https://www.python.org/">Python</a><br>
    Entorno virtual utilizado: <a href = "https://www.anaconda.com">Anaconda</a><br>
    Libreria utilizada para la creacion de la API: <a href = "https://fastapi.tiangolo.com">FastAPI</a></h4>

<h1 align = center>Requirements.txt</h1>

Para poder utilizar de manera local la API necesitmos tener algunas librerias que no vienen instaladas por defecto. En este caso como usaremos Anaconda hay que ir a la pagina oficial e instalarlo, recordar que hay que activar la opcion del `PATH` para poder manejarlo como una variable de entorno. Una vez instalado, creamos la carpeta donde vamos a crear la API y el entorno virtual, como por ejemplo sera "fastapi" y sera en el escritorio, y abrimos `cmd` y ejecutamos el siguiente codigo:

`cd desktop`. Y luego: `cd fastapi`

Una vez colocado lo anterior, se coloca:

`conda create --name fastapi python=n`. En este caso el nombre del entorno virtual puede ser el que sea, pero por orden se coloca el mismo nombre de la carpeta. `n` representa la version con la que se trabajara en el entorno virtual, actualmente seria 3, independientemente de que version especifica de <a href = "https://www.python.org/">Python 3</a> se utilice, igual se coloca asi. Una vez hecho este paso, saldran dos opciones, el `conda activate fastapi` o `conda deactivate`, se coloca el activate para activar el entorno virtual y claramente con su respectivo nombre.

Una vez hecho lo anterior, abrimos el respectivo editor de codigo (<a href= "https://code.visualstudio.com">Visual Studio Code</a>), abrimos la carpeta correspondiente y seleccionamos el interprete correspondiente que en este caso sera el de conda, abrimos la terminal de visual studio code, automaticamente el programa detectara que se esta usando Anaconda como entorno virtual y entonces, pero antes, abrimos una nueva ventana del `cmd` para poder hacer lo siguiente.

`pip install fastapi` y `pip install uvicorn`

# ¿Por que es importante hacer este paso?

Porque si lo instalamos desde el entorno virtual, tendremos que ejecutar una y otra vez los codigos para poder usar la API creada.

# Volviendo a lo anterior...

Una vez estando en visual studio con el entorno virtual activo, creamos un archivo `py` cuyo nombre sera app, es decir `app.py`, escribimos el siguiente codigo dentro del archivo:

`from fastapi import FastAPI` <br>
`app = FastAPI()`

Una vez hecho eso ya tendriamos finalizada nuestra instalacion y configuracion para el uso de la API, escribimos el siguiente codigo:

`uvicorn app:app`. Es decir que le especificamos a uvicorn que cree un entorno virtual en `app.py` en la variable app, que es donde esta almacenada la API.

Y con eso ya estaria finalizada la configuracion y la instalacion de los archivos necesarios para usar la API :).

<h3>Recomendacion</h3>

Para no estar a cada rato pulsando `Ctrl + C` para apagar la API cada vez que se guardan los cambios en el archivo y volver a escribir `uvicorn app:app`, se ejecuta el siguiente codigo:

`uvicorn app:app --reload`. Con esto bastaria guardar el archivo para que haga la reactivacion de manera automatica y sea mas optimo.

<h1 align = center>Muchas gracias! :)</h1>
