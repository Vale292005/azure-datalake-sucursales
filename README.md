# 🏢 Sistema de Sucursales - Azure Data Lake (Azurite + Trino + FileBrowser)

Este proyecto simula una arquitectura local de **Azure Data Lake Storage Gen2 (ADLS)** orientada a un sistema de gestión de inventario para sucursales en tiempo real.

Permite simular la alta de productos, verificación de stock y la compra concurrente de items en el Data Lake local (eliminando físicamente los archivos al comprar para evitar colisiones entre sucursales).

---

## 🛠️ Tecnologías y Arquitectura

* **Simulador de Azure Blob Storage:** [Azurite](https://learn.microsoft.com/es-es/azure/storage/common/storage-use-azurite) (Puerto `10000`).
* **Explorador Gráfico Web:** [FileBrowser](https://filebrowser.org/) (Puerto `8080`).
* **Motor de Consultas SQL:** [Trino](https://trino.io/) (Puerto `8081`).
* **Backend / Lógica de Negocio:** Java JDK 17+.

---

## 🚀 Requisitos Previos

Asegúrate de contar con las siguientes herramientas instaladas en tu equipo (Mac, Windows o Linux):

1. **[Docker Desktop](https://www.docker.com/products/docker-desktop/)** *(Debe estar abierto y ejecutándose)*.
2. **[Java JDK 17](https://www.oracle.com/java/technologies/downloads/)** o superior.
3. **[Git](https://git-scm.com/)**.

---

## 📦 Instrucciones para Levantar el Proyecto

### 1. Clonar el Repositorio

Abre tu terminal y ejecuta:

```bash
git clone [https://github.com/Vale292005/azure-datalake-sucursales.git](https://github.com/Vale292005/azure-datalake-sucursales.git)
cd azure-datalake-sucursales
```
### 2. Iniciar el Data Lake con Docker

Levanta la infraestructura simulada (Azurite, Trino y FileBrowser) en segundo plano:

```bash
docker compose up -d
```

### 3. Explorar el Data Lake en el Navegador
Una vez encendidos los contenedores, abre cualquier navegador (Chrome, Safari, Edge) e ingresa a:

👉 👉 [http://localhost:8080](http://localhost:8080)
