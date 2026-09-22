# Corios CMMS — Software de Gestión de Mantenimiento Industrial

<div align="center">

![Latest Release](https://img.shields.io/github/v/release/CoriosMwRaw/Corios_CMMS-Releases?style=for-the-badge&color=2563eb&label=Versi%C3%B3n%20Oficial)
![Platform](https://img.shields.io/badge/Plataforma-Windows%2064--bit-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Architecture](https://img.shields.io/badge/Modo-Offline--First%20%2B%20Cloud-10b981?style=for-the-badge)
![Standard](https://img.shields.io/badge/Cumplimiento-ISO%209001%20%2F%20IATF%2016949-8b5cf6?style=for-the-badge)
![Support](https://img.shields.io/badge/Soporte-Industrial%20Tier--1-f59e0b?style=for-the-badge)

<br/>

**El sistema de gestión computarizada del mantenimiento (CMMS / GMAO) diseñado para maximizar la disponibilidad de planta, erradicar paros no planificados y automatizar el control de almacén.**

[Descargar Instalador](#-descarga-e-instalación-rápida) •
[Módulos Destacados](#-módulos-y-capacidades-industriales) •
[Compatibilidad de Hardware](#-compatibilidad-de-hardware-industrial) •
[Requisitos del Sistema](#-requisitos-del-sistema) •
[Soporte Empresarial](#-soporte-y-licenciamiento)

</div>

---

## 🏭 ¿Qué es Corios CMMS?

**Corios CMMS** es una suite de software industrial diseñada específicamente para plantas de manufactura, talleres mecánicos, líneas de ensamble y centros de distribución. A diferencia de las plataformas web tradicionales que se congelan cuando falla el internet, **Corios CMMS** opera con tecnología **Offline-First**: la aplicación corre directamente en las estaciones de trabajo con latencia cero, manteniendo los datos 100% operativos aún sin red y sincronizando automáticamente con la nube en segundo plano cuando la conexión se restablece.

```
   [Piso de Planta]                                [Nube Central]
  ┌─────────────────────────────────┐             ┌──────────────────────────────────┐
  │  Terminal Kiosko / Taller       │             │  Clúster Seguro en la Nube       │
  │  • Escaneo de QR con pistola 2D │             │  • Respaldo corporativo continuo │
  │  • Creación de OTs sin internet │ ◄─────────► │  • Reportes consolidados multi-  │
  │  • Salida de refacciones al día │ (Auto-Sync) │    planta y dashboards remotos   │
  │  • Cero esperas ni bloqueos     │             │  • Métricas MTTR, MTBF y OEE     │
  └─────────────────────────────────┘             └──────────────────────────────────┘
```

---

## ⚡ Módulos y Capacidades Industriales

### 🏷️ 1. Ecosistema de Códigos QR para Máquinas y Refacciones
- **Escaneo Rápido en Modo Kiosko (`Ctrl + Q`):** El operador o técnico simplemente apunta la pistola lectora láser o 2D al chasis del equipo. En menos de 2 segundos, el sistema abre la ventana de *Nueva Orden de Trabajo* con la máquina, modelo y área ya seleccionados.
- **Impresión de Etiquetas Térmicas (50 x 30 mm):** Generación e impresión directa de etiquetas industriales de alta durabilidad con logotipo corporativo, nombre del activo, número de serie/SKU, ubicación de planta y código QR nítido.

### 📋 2. Gestión Integral de Órdenes de Trabajo & Monitoreo de SLAs
- **Control Estricto de Tiempos de Respuesta y Resolución:** Monitoreo en tiempo real de metas SLA (por ejemplo, respuesta en $\le$ 15 min y resolución en $\le$ 120 min).
- **Ficha Técnica Oficial Imprimible:** Generación con un solo clic de la hoja técnica vectorial de la orden, desglosando causa raíz de falla, procedimiento realizado, refacciones utilizadas, equipo de técnicos intervinientes y **recuadros reglamentarios de firma** para el técnico responsable y la aceptación formal del supervisor de producción.

### 📦 3. Almacén Inteligente, Kardex y Requisiciones de Compra
- **Kardex Electrónico Completo:** Auditoría rigurosa de cada entrada, salida, ajuste y devolución de componentes con trazabilidad por máquina y técnico.
- **Generador Automático de Requisiciones de Compra:** Detección instantánea de todas las piezas cuyo inventario actual está en o por debajo del punto mínimo de seguridad ($\le \text{min\_stock}$). El sistema calcula la cantidad sugerida de reposición:
  $$\text{Cantidad a Comprar} = (\text{Stock Mínimo} \times 2) - \text{Stock Actual}$$
- **Exportación Rápida:** Botón para copiar el pedido formateado al portapapeles (listo para WhatsApp o correo a proveedores) y botón para imprimir la **Requisición Oficial de Compra** con firmas autorizadas.

### 📅 4. Calendario Bimestral de Mantenimiento Preventivo
- **Tablero Visual de Ejecución:** Visualización continua de 2 meses calendario para planificar mantenimientos por frecuencia semanal, mensual, trimestral o semestral.
- **Semáforo Inteligente de Estado:** Marcadores de color dinámicos que indican tareas programadas, preventivos al día y alertas de vencimiento.

### 📶 5. Widget de Telemetría y Salud de Sincronización
- **Indicador Dinámico en Cabecera:**
  - 🟢 **Conectado (XX ms):** Latencia en tiempo real con la nube y base de datos local 100% al día.
  - 🟡 **Sincronizando (N pend):** Subida automática de registros pendientes en curso.
  - 🔴 **Offline:** Operación autónoma en modo local; no detiene ningún trabajo del personal.
- **Modal de Diagnóstico:** Acceso con 1 clic para auditar registros pendientes tabla por tabla y forzar sincronización manual inmediata.

### 🖥️ 6. Modo Kiosko con Cambio Rápido de Usuario (Fast Switching)
- **Diseñado para Terminales Compartidas en Planta:** Permite cambiar de turno o de técnico en menos de 1 segundo sin reiniciar el programa ni cerrar la máquina virtual.
- **Temporizador de Inactividad Inteligente:** Si un operario deja la sesión abierta, el sistema detecta la ausencia de teclado y mouse y cierra la sesión automáticamente para resguardar la seguridad.
- **Recuperación Automática de Borradores:** Si la sesión se cierra mientras se capturaba una orden, el texto y datos se guardan como borrador y se restauran al iniciar sesión de nuevo.

---

## 📥 Descarga e Instalación Rápida

### Paso 1: Descargar el Instalador
Dirígete a la pestaña oficial de **[Releases](https://github.com/CoriosMwRaw/Corios_CMMS-Releases/releases)** de este repositorio y descarga el instalador más reciente:
- Archivo: `Corios_CMMS_Setup_x64.exe` (o ejecutable empaquetado correspondiente).

### Paso 2: Instalación
1. Ejecuta el archivo descargado.
2. Sigue el asistente de instalación estándar de Windows.
3. El paquete ya incluye su propio entorno de ejecución pre-configurado y optimizado, por lo que **NO necesitas instalar Java, JDK ni drivers adicionales**.

### Paso 3: Primer Inicio y Activación
1. Al abrir la aplicación por primera vez, el sistema identificará la estación de trabajo mediante su huella de hardware (`Hardware UUID`).
2. Contacta al administrador de tu empresa o soporte técnico de Corios para autorizar la estación en el panel central.
3. ¡Listo! La terminal se conectará automáticamente y descargará la configuración de tu empresa.

---

## 🖨️ Compatibilidad de Hardware Industrial

**Corios CMMS** está optimizado de fábrica para interactuar con periféricos industriales estándar de cualquier marca:

| Dispositivo | Especificación / Modelo Soportado | Función en el Sistema |
| :--- | :--- | :--- |
| **Pistolas Lectoras de Códigos (Barcode / 2D)** | Lectores USB o Bluetooth compatibles con emulación de teclado **HID** (Honeywell, Zebra, Datalogic, Netum, Eyoyo, etc.). | Escaneo instantáneo de activos en chasis para abrir órdenes (`Ctrl + Q`) y búsqueda de refacciones. |
| **Impresoras Térmicas de Etiquetas** | Impresoras de transferencia térmica directa (Zebra ZD220/ZD420, Brother TD/QL series, TSC, Dymo) configuradas en **50x30 mm** o **2x1 pulgadas**. | Impresión de etiquetas adhesivas de alta resolución para maquinaria y gavetas de almacén. |
| **Impresoras de Oficina / Piso** | Cualquier impresora láser o inyección de tinta compatible con Windows (A4 o Carta). | Impresión de Fichas Técnicas de Orden de Trabajo, Requisiciones de Compra y Reportes de Kardex. |

---

## 💻 Requisitos del Sistema

### Requisitos Mínimos (Terminal de Planta / Kiosko)
- **Sistema Operativo:** Windows 10 (64-bit) o Windows 11.
- **Procesador:** Intel Core i3 (4ta Gen o superior) / AMD Ryzen 3 / Intel Celeron G4900 o equivalente.
- **Memoria RAM:** 4 GB.
- **Almacenamiento:** 500 MB de espacio disponible en disco sólido (SSD recomendado).
- **Resolución de Pantalla:** $1366 \times 768$ píxeles.
- **Red:** Conexión Ethernet o Wi-Fi para sincronización (funciona 100% offline).

### Requisitos Recomendados (Estación de Jefatura / Supervisor)
- **Sistema Operativo:** Windows 11 Pro (64-bit).
- **Procesador:** Intel Core i5 / AMD Ryzen 5 o superior.
- **Memoria RAM:** 8 GB o superior.
- **Almacenamiento:** SSD NVMe con 1 GB disponible.
- **Resolución de Pantalla:** $1920 \times 1080$ (Full HD) con soporte HiDPI.

---

## 🛡️ Seguridad, Privacidad y Confiabilidad

- **Aislamiento Multi-Tenant:** Cada empresa y sucursal opera en un espacio lógico blindado e impenetrable.
- **Encriptación en Tránsito:** Toda la sincronización hacia el clúster en la nube viaja cifrada bajo protocolos **TLS 1.3**.
- **Licenciamiento Seguro por Hardware:** Control riguroso de estaciones autorizadas para prevenir accesos no autorizados o copias fuera de la empresa.
- **Respaldos Automáticos:** La base de datos local almacena cada transacción en SQLite y el clúster en la nube mantiene respaldos automatizados.

---

## 📞 Soporte y Licenciamiento Empresarial

Para cotizaciones empresariales, adición de nuevas terminales de planta, solicitudes de personalización o soporte técnico prioritario:

- **Repositorio Oficial de Descargas:** [CoriosMwRaw/Corios_CMMS-Releases](https://github.com/CoriosMwRaw/Corios_CMMS-Releases)
- **Soporte Técnico & Activaciones:** Contacta a tu representante técnico asignado de Corios.

---

<div align="center">

**Corios CMMS** — *Potencia, control y continuidad operativa para la industria moderna.*  
© 2026 Corios. Todos los derechos reservados.

</div>
