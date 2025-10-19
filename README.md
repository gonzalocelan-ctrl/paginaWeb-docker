## Descripción del proyecto 

Este sitio web corresponde a una **cervecería artesanal** dedicada a la producción y venta de cervezas.  
La página está pensada para que los usuarios puedan:

- Conocer la historia de la cervecería y quiénes son las personas detrás del proyecto.  
- Explorar la variedad de cervezas artesanales disponibles.  
- Acceder a información de contacto para realizar consultas o pedidos.  

El proyecto fue desarrollado con **HTML, CSS y JavaScript**, empaquetado en un contenedor **Docker** y publicado en **Docker Hub**.

### Dockerfile
El proyecto incluye un archivo `Dockerfile` donde utilicé **Nginx** para contenerizar la aplicación.  
De esta manera, al ejecutar el contenedor, la página queda disponible automáticamente en el puerto 80.

### Construcción del docker
- **Construí la imagen localmente con el siguiente comando:**

  **`docker build -t gonzalocelan/paginaweb-cervezaartesanal:latest .`**

---

- **Ejecuté la imagen en mi PC de manera local:**

  **`docker run -d -p 8080:80 gonzalocelan/paginaweb-cervezaartesanal:latest`**

---

- **Finalmente, subí la imagen a Docker Hub para que pueda ser descargada y ejecutada en cualquier entorno:**

  **`docker push gonzalocelan/paginaweb-cervezaartesanal:latest`**

### Ejecucion desde Docker Hub
- **Cualquier usuario puede descargar y correr la aplicación directamente con los siguientes comandos:**
  
  **`docker pull gonzalocelan/paginaweb-cervezaartesanal:latest`**
---

  **`docker run -d -p 8080:80 gonzalocelan/paginaweb-cervezaartesanal:latest`**
  
---

La página queda disponible en http://localhost:8080.
