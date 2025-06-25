# Habity - WebApp (Frontend Funcional)

Este repositorio contiene la interfaz web del usuario para Habity. Permite registrar e iniciar sesión, administrar hábitos, revisar el progreso, interactuar con publicaciones y recibir recomendaciones personalizadas.

## Funcionalidades cubiertas (según Product Backlog)

- Registro y login con autenticación JWT
- Dashboard de usuario
- Crear y listar hábitos
- Visualizar progreso y registro de días
- Visualizar publicaciones y reacciones

## Tecnologías

- HTML5
- CSS3
- JavaScript vanilla (sin frameworks)
- JWT (almacenado en localStorage)
- Fetch API para consumo de endpoints RESTful

## Estructura del proyecto

register/: login.html, register.html  
dashboard/: dashboard.html, agregar-habito.html, ver-habitos.html  
Progreso/: progreso.html  
ia/: ia.html  
Notificaciones/, blog/, twietterhabits/: otras funcionalidades

## Conexión al Backend

La web se conecta automáticamente al entorno adecuado:

const BASE_URL = window.location.hostname.includes("localhost")  
  ? "http://localhost:8080"  
  : "https://habity-backend.up.railway.app";

Todos los fetch() apuntan a esta constante.

## Cómo ejecutar

1. Abre cualquier HTML (ej. login.html) con Live Server en VS Code.
2. Verifica que el backend esté activo.
3. Inicia sesión, navega y prueba las funcionalidades.

## Despliegue

https://habity-webapp.vercel.app

## Ciclo de desarrollo

Las tareas se organizaron en Historias de Usuario, cada una con subtareas estimadas y distribuidas por Sprint. Ver Trello (incluido en entrega).

## Autores

- Romario Rodriguez  
- Dylan Tong Barahona  
- Chalco Falcón David Alonso  
- Chunga Vásquez Karla  
- Alvarez Augusto  

Proyecto Final - SI705 Arquitectura de Aplicaciones Web (202402)