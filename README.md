
# DevOps Reservas Salud

Proyecto integrador DevOps para una plataforma web de reserva de horas médicas.

## Objetivo
Desarrollar una página web estática utilizando HTML, CSS, Nginx y Docker, aplicando prácticas de control de versiones mediante Git y GitHub.

## Funcionalidades
- Información general de atención.
- Formulario demostrativo de reserva de horas médicas.
- Visualización del estado del servicio.

## Requisitos
- Git
- Docker Desktop
- Docker Compose
- Navegador web

## Configuración del entorno

El archivo .env.example contiene un ejemplo de configuración
del puerto utilizado por el servicio.

Para personalizar el puerto, copiar .env.example como .env
y modificar APP_PORT según sea necesario.

Si no se configura esta variable, Docker Compose utilizará
el puerto 8080 de forma predeterminada.

El archivo .env no debe publicarse en GitHub.

## Instalación y ejecución

1. Clonar el repositorio:
git clone https://github.com/zith9x/DevOps_Reservas_Salud.git

2. Ingresar a la carpeta del proyecto:
cd DevOps_Reservas_Salud

3. Construir e iniciar el servicio:
docker compose up -d --build

4. Abrir la aplicación en el navegador:
http://localhost:8080

## Verificación

Consultar el estado del contenedor:
docker compose ps
Revisar los registros de funcionamiento:
docker compose logs
Consultar las métricas:
docker stats --no-stream
Detener el servicio:
docker compose down

## Seguridad
- No se utilizan credenciales ni contraseñas reales.
- El archivo .gitignore excluye archivos de configuración privados y temporales.
- El archivo .env.example contiene únicamente valores de ejemplo.
- No se deben publicar tokens, contraseñas ni datos personales.
- El formulario es demostrativo y no almacena ni envía información de pacientes.
- Las pruebas deben realizarse utilizando datos ficticios.
