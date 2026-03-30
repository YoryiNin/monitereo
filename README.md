Sistema de Monitoreo con Prometheus y Grafana (Docker)

Este proyecto implementa un sistema básico de monitoreo utilizando Docker, Prometheus y Grafana.

Permite recolectar métricas del sistema y visualizarlas en dashboards interactivos.

 Tecnologías usadas
Docker
Prometheus
Grafana
Node Exporter

 Prometheus recolecta métricas y Grafana las visualiza en dashboards

📁 Estructura del proyecto
monitoring/
│── docker-compose.yml
│── prometheus.yml
⚙ Instalación y ejecución
1. Clonar el repositorio
git clone https://github.com/tuusuario/monitoring.git
cd monitoring
2. Ejecutar el proyecto
docker compose up -d
3. Acceder a los servicios
Prometheus → http://localhost:9090
Grafana → http://localhost:3000

Usuario por defecto:

user: admin
password: admin
 Configuración de Grafana
Ir a Configuration → Data Sources

Agregar:

URL: http://prometheus:9090
Guardar y probar
 Screenshots

Aquí puedes poner imágenes de tu proyecto 👇

 Grafana Dashboard
![Grafana Dashboard](images/grafana.png)
 Prometheus Targets
![Prometheus Targets](images/prometheus.png)

 IMPORTANTE:

Crea una carpeta llamada images/ en tu repo
Guarda ahí tus capturas
GitHub las mostrará automáticamente
📈 Métricas disponibles

Ejemplos que puedes visualizar:

CPU usage → node_cpu_seconds_total
RAM usage → node_memory_Active_bytes
Disk usage
 Ejemplo de consulta
node_cpu_seconds_total
📌 Notas
Puedes agregar más exporters para monitorear otras aplicaciones
Puedes importar dashboards listos desde Grafana
 Objetivo del proyecto

Este proyecto fue creado como práctica para aprender:

Monitoreo con Prometheus
Visualización con Grafana
Uso de Docker Compose

images/Captura.PNG
images/zx.PNG

🧑 Autor

Yoryi Nin de la Rosa
