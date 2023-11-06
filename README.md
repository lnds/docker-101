# docker-101


 Crea un archivo llamado `requirements.txt` que contenga lo siguiente:

```
flask == 2.3.3
```


Luego agrega el archivo `hello.py` con el siguiente contenido:

```
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

app.run(host='0.0.0.0', port=8000)
```

Ahora ejecuta docker con el siguiente comando:

```
docker init
```

Completa la configuración de modo que tu sesión se vea así:

![image](https://github.com/lnds/docker-101/assets/515492/201e8622-d073-4e18-ae3f-4bc6d94f8244)


Después ejecuta la aplicación con este comando:

```
docker compose up —build
```

Navega a la dirección `localhost:8000` y verifica que puedes acceder a tu aplicación.


