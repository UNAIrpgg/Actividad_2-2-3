# Instalación y Configuración de Hugo
 
Voy a crear una página en Hugo mediante visual studio code y voy a desplegarla mediante comandos en Github y Netlify.
 
---
 
## 1. Instalación de Hugo
   - Instalo la versión extendida de Hugo mediante el comando mostrado.
 
   ![Proceso de instalación de Hugo en la máquina virtual](Imagenes2/1.png)
 
---
 
## 2. Creación de un nuevo proyecto en Hugo
   - Utilizo el comando:
     ```bash
     hugo new site <actividad22_2_RAU>
     ```
   - Esto generará la estructura inicial del proyecto.
 
   ![Imagen 2: Estructura del proyecto generada por Hugo](Imagenes2/2.png)
 
## 3. Configuración del repositorio en GitHub
   - Me meto a GitHub y creo un nuevo repositorio vacío con el nombre de la actividad.
 
   ![Imagen 4: Interfaz de GitHub para crear un repositorio nuevo](Imagenes2/3.png)
 
1. **Clonar el repositorio**:
   - Para clonar este repositorio utilizo este comando
     ```bash
     git clone https://github.com/RodrigoGColl/actividad22_1_RAU.git
     ```
 
   ![Imagen 5: Proceso de clonación del repositorio en la terminal](Imagenes2/4.png)
 
---
 
## 4. Gestión de temas en Hugo
 
1. **Añado un tema al proyecto**:
   - Descargo el tema ananke y lo añado como submódulo:
     ```bash
     git submodule add <URL del tea de ananke> themes/<ananke>
     ```
 
   ![Imagen 6: Proceso de añadir un tema como submódulo](Imagenes2/5.png)
 
2. **Configuración del tema**:
   - Añado la referencia al tema en el archivo de configuración:
     ```bash
     theme = "<ananke>"
     ```
 
   ![Imagen 7: Archivo config.toml configurado con el tema](Imagenes2/6.png)
 
3. **Actualización del submódulo**:
   - Para la actualización del módulo ejecuto:
     ```bash
     git submodule init
     git submodule update
     ```
 
   ![Imagen 8: Confirmación de actualización del submódulo en la terminal](Imagenes2/7.png)
 
---
4. **Configuración del índice**

   - Así he configurado el índice de la página
   
   ![Imagen 11: Configuración del dominio en Netlify](Imagenes2/8.png)

## 5. Subida del proyecto a GitHub
 
1. **Preparar los cambios para subirlos**:
   - Añado los archivos:
     ```bash
     git add .
     ```
   - Confirmo los cambios:
     ```bash
     git commit -m "lo subo"
     ```
   - Subo los cambios al repositorio:
     ```bash
     git push -u origin master
     ```
 
   ![Imagen 9: Terminal mostrando la subida de archivos a GitHub](Imagenes2/9.png)
   ![Imagen 9: Confirmación de subida a Github](Imagenes2/15.png)
---
 
## 6. Despliegue en Netlify
 
1. **Vinculación del repositorio en Netlify**:
   - Accedo a Netlify, creo un nuevo sitio desde un repositorio y selecciono el proyecto que he hecho.
 
   ![Imagen 10: Proceso de vinculación del repositorio en Netlify](Imagenes2/18.png)
 
2. **Configurar el dominio y desplegar el sitio**:
   - Ajusto las configuraciones necesarias para el dominio y el despliegue, seguiré los siguientes pasos.
 
   ![Imagen 11: Configuración del dominio en Netlify](Imagenes2/12.png)
   ![Imagen 11: Configuración del dominio en Netlify](Imagenes2/13.png)
   ![Imagen 11: Configuración del dominio en Netlify](Imagenes2/14.png)
   ![Imagen 11: Configuración del dominio en Netlify](Imagenes2/16.png)

   - Aquí ya se ha completado
  
   ![Imagen 11: Configuración del dominio en Netlify](Imagenes2/17.png)
---