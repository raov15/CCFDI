# CCFDI

Equipo de trabajo:
•	Roberto Antonio Orozco Velázquez
•	Scarlet
•	Colaborador: Daniel
________________________________________
1. Descripción General del Proyecto
El proyecto consiste en el desarrollo de una aplicación web para la consulta, procesamiento y gestión de CFDI, la cual permitirá automatizar procesos relacionados con la validación y análisis de información fiscal.
El desarrollo se está abordando mediante dos vertientes principales, permitiendo avanzar de forma paralela en distintos componentes del sistema.
________________________________________
2. Enfoque de Desarrollo
El desarrollo del proyecto se ha dividido en dos vertientes principales. Aunque cada una tiene responsables definidos, ambas forman parte de un mismo esfuerzo colaborativo, donde el equipo trabaja de manera conjunta y coordinada, apoyándose mutuamente para lograr resultados en el menor tiempo posible.
________________________________________
Vertiente 1: Desarrollo de Plataforma Web
Responsables: Roberto y Daniel
•	Diseño y desarrollo de la interfaz web
•	Implementación de endpoints/API
•	Integración con servicios externos (SAT)
•	Visualización de datos (dashboard de facturas)
________________________________________
Vertiente 2: Transformación de Estructuras Excel a Python
Responsable: Scarlet
Esta vertiente se enfoca en la conversión de estructuras, fórmulas y lógica contenida en archivos Excel hacia código funcional en Python.
•	Interpretación de estructuras de Excel
•	Traducción de fórmulas a lógica Python
•	Estandarización de reglas de negocio
•	Preparación de la lógica para integración con el sistema CFDI
________________________________________
3. Avances Técnicos (Roberto)
3.1 Desarrollo de herramienta de conversión
Se ha iniciado el desarrollo de un módulo capaz de:
•	Leer archivos Excel estructurados
•	Interpretar fórmulas y lógica existente
•	Traducir operaciones a código Python
•	Preparar la lógica para integración directa en backend
________________________________________
3.2 Estructura del Proyecto
Se ha definido una arquitectura modular para facilitar escalabilidad y mantenimiento:
cfdi_system/
│
├── data/
│   └── CCFDI de p.m. 2026.xlsx
│
├── app/
│   ├── main.py        # Punto de entrada de la aplicación
│   ├── models.py      # Definición de modelos (ORM / estructuras)
│   ├── database.py    # Conexión a base de datos
│   ├── logic.py       # Procesamiento y reglas de negocio
│   └── loader.py      # Lectura y transformación de Excel
│
├── requirements.txt   # Dependencias del proyecto
└── Dockerfile         # Contenerización del sistema
________________________________________
3.3 Componentes Implementados
•	✔ Lectura inicial de archivos Excel
•	X Definición de estructura base del proyecto
•	X Separación de lógica por módulos
•	X Preparación del entorno en Docker
________________________________________
3.4 Componentes en Desarrollo
•	Traducción automática de fórmulas Excel → Python
•	Normalización de datos provenientes del Excel
•	Integración con base de datos (Apollo de Scarlet)
•	Validación de reglas fiscales (Validación Isrrael)
________________________________________
4. Uso de Contenedores (Docker)
Se plantea el uso de Docker para:
•	Asegurar portabilidad del sistema
•	Facilitar despliegue en servidores
•	Mantener consistencia de entorno
•	Integrar servicios (API + base de datos)
________________________________________
5. Próximos Pasos
Corto Plazo (1 Semanas)
•	Finalizar el módulo loader.py
•	Completar conversión de fórmulas críticas
•	Integrar lógica con base de datos
Mediano Plazo(15 dias)
•	Conectar motor de procesamiento con API web
•	Implementar validaciones CFDI
•	Pruebas con datos reales
Largo Plazo (1 mes)
•	Dashboard completo
•	Automatización total del flujo CFDI
•	Optimización de rendimiento
________________________________________
6. Conclusión
El proyecto presenta un avance sólido en la definición de arquitectura y en el desarrollo del motor de procesamiento de datos.
La estrategia de dividir el desarrollo en dos vertientes permite avanzar de manera eficiente tanto en la capa visual como en la lógica del sistema.
El componente desarrollado representa una pieza clave, ya que permitirá automatizar la conversión de lógica empresarial existente en Excel hacia un sistema escalable en Python.
________________________________________
7. Observaciones
•	Se mantendrá control de versiones (https://github.com/raov15/CCFDI)
•	Las fórmulas serán basadas en DB y Python
•	Documentar reglas de negocio provenientes Isrrael.
________________________________________
