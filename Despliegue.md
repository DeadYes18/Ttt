# Despliegue de la Aplicación PokeDex

## 1. Introducción

El presente documento describe de manera detallada el proceso realizado para el despliegue de la aplicación web PokeDex en un entorno de nube. Durante esta actividad se aplicaron conceptos básicos de desarrollo web, control de versiones y buenas prácticas de seguridad, con el objetivo de garantizar que la aplicación fuera accesible públicamente y cumpla con ciertos estándares mínimos de protección.

---

## 2. Preparación del entorno

En primer lugar, se descargó el código fuente de la aplicación desde el repositorio proporcionado. Posteriormente, se descomprimieron los archivos en el equipo local y se verificó su correcta estructura.

Se confirmó la existencia del archivo principal `index.html`, junto con la carpeta `assets`, la cual contiene los recursos necesarios como estilos, scripts e imágenes. Esta verificación fue importante para asegurar que la aplicación funcionara correctamente al momento de ser desplegada.

---

## 3. Creación del repositorio

Se procedió a crear un repositorio público en GitHub con el nombre `pokedex`, cumpliendo con los requisitos establecidos.

Luego, se realizó la carga de los archivos del proyecto, asegurando que la estructura quedara organizada correctamente en la raíz del repositorio. Esto incluyó:

* Archivo principal `index.html`
* Carpeta `assets` con todos sus recursos
* Archivo `README.md`

Este paso permitió tener el proyecto versionado y listo para su integración con una plataforma de despliegue.

---

## 4. Despliegue en la nube

Para el despliegue de la aplicación, se utilizó la plataforma Vercel, la cual permite publicar aplicaciones web de manera rápida y sencilla.

El proceso consistió en:

1. Iniciar sesión en Vercel utilizando la cuenta de GitHub.
2. Importar el repositorio `pokedex`.
3. Configurar el proyecto como una aplicación estática.
4. Ejecutar el despliegue automático.

Una vez finalizado este proceso, la plataforma generó una URL pública mediante la cual se puede acceder a la aplicación desde cualquier navegador.

---

## 5. Implementación de seguridad

Con el fin de mejorar la seguridad de la aplicación, se configuraron encabezados HTTP mediante un archivo `vercel.json` ubicado en la raíz del repositorio.

Entre los encabezados implementados se encuentran:

* **X-Frame-Options:** Previene ataques de tipo clickjacking.
* **X-Content-Type-Options:** Evita la interpretación incorrecta de archivos.
* **Referrer-Policy:** Limita la información enviada en las solicitudes.
* **Content-Security-Policy:** Controla los recursos que puede cargar la aplicación.

Estas configuraciones contribuyen a reducir riesgos comunes en aplicaciones web.

---

## 6. Verificación de seguridad

Para evaluar la efectividad de las medidas implementadas, se utilizó la herramienta en línea https://securityheaders.com/.

A través de esta plataforma se analizó la aplicación desplegada, obteniendo una calificación basada en los encabezados de seguridad configurados. Esto permitió identificar el nivel de protección alcanzado y validar las mejoras realizadas.

---

## 7. Conclusión

El proceso de despliegue de la aplicación PokeDex se realizó de manera exitosa, logrando que el sistema esté disponible en la web y sea accesible públicamente.

Además, se integraron medidas básicas de seguridad que fortalecen la protección de la aplicación frente a posibles vulnerabilidades. Esta experiencia permitió comprender la importancia de no solo desplegar una aplicación funcional, sino también de garantizar su seguridad en un entorno real.
