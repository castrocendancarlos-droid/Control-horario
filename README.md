# Mi jornada · iPhone y GitHub Pages

Aplicación estática en español. No requiere Python ni un servidor de datos. Los cálculos se ejecutan en el dispositivo y los registros se guardan en IndexedDB, dentro del navegador.

## Publicar en GitHub

1. Crea un repositorio y sube **el contenido de esta carpeta** a la raíz: `index.html` debe quedar en la raíz del repositorio.
2. En GitHub abre Settings → Pages, selecciona despliegue desde una rama, `main` y `/ (root)`, y guarda.
3. Abre el enlace de Pages que muestra GitHub. Desde Safari en el iPhone puedes usar Compartir → Añadir a pantalla de inicio.
4. Abre la aplicación una vez con conexión. Los archivos necesarios se almacenan para usarla después sin conexión. Comprueba ese funcionamiento antes de depender de él.

No subas bases de datos, archivos Excel ni tus copias JSON al repositorio. Este paquete contiene únicamente el programa: empieza con un año vacío. La configuración de calendario y los fichajes se pueden trasladar con una copia JSON privada.

## Copias de seguridad

- **↓ Copia** descarga una copia JSON de todos los años y datos guardados. En iPhone guárdala en Archivos o iCloud Drive. Si Safari abre el documento en vez de descargarlo, usa Compartir → Guardar en Archivos.
- **↥ Importar** permite elegir una copia, comprobar sus años y registros y confirmar la importación. Las fechas y configuraciones coincidentes se toman del archivo; los datos de otros años y fechas se conservan.
- Antes de importar se conserva el estado anterior dentro del navegador. **Recuperar estado anterior** permite deshacer la última importación; también conserva el estado que había antes de recuperar.
- La copia incluye parámetros anuales, fechas de contrato, vacaciones, calendarios, turnos de Navidad, fichajes, ausencias, notas, ajustes y referencias originales de Excel. Los resúmenes se recalculan al importar.
- No hay sincronización automática entre el ordenador y el iPhone. Exporta una copia y trasládala manualmente cuando lo necesites.
- La versión Python del ordenador puede exportar este mismo formato. La importación a SQLite desde el móvil no forma parte de esta entrega.

Los datos pertenecen al navegador, dispositivo y dirección web utilizados. Borrar los datos de Safari, cambiar de dirección/repositorio o utilizar otro navegador puede dejar la aplicación sin tus registros. La copia JSON guardada fuera del navegador permite recuperarlos. Comprueba si Safari y la aplicación añadida a inicio comparten tus registros antes de alternar entre ambas; usa la copia JSON cuando sea necesario.

El archivo JSON no está cifrado. No lo publiques. La interfaz y el código pueden ser públicos: los registros no se envían a GitHub ni se incluyen en las peticiones del sitio. La descarga del programa sí utiliza la conexión normal a GitHub Pages.

## Criterios de cálculo

Se conserva el cálculo de la versión Python: café permitido incluido y descuento del exceso; T Teletrabajo solo tarde, D Teletrabajo día entero; bloques semanales por parte mensual con arrastre; ausencias por horas desglosadas sin duplicarlas; Defunción Familiar de día completo justificada y sin recuperación; horas del parte según calendario y temporada; vacaciones proporcionales; límites trimestrales de teletrabajo. Los avisos de datos pendientes de revisión se mantienen.

Se compara automáticamente el motor JavaScript con los registros y resultados de Python antes de empaquetar. El funcionamiento real de descarga y de instalación en un iPhone debe comprobarse en el dispositivo; la entrega se verifica en el navegador de escritorio con pantalla estrecha.

Para probar el paquete en un ordenador, utiliza un servidor HTTP estático; abrir `index.html` directamente desde el explorador de archivos no permite cargar los módulos y el modo sin conexión.
