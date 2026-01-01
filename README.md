# 📊 Data Engineering Project – Databricks ETL Pipeline

## 📌 Project Overview
Este proyecto muestra el desarrollo de un **pipeline de datos end-to-end en Databricks**, utilizando una arquitectura **Medallion (Bronze → Silver → Gold)**.  
El objetivo es simular un flujo real de procesamiento de datos, desde la ingesta hasta la preparación de datos listos para análisis.

---

## 🎯 Objetivo del proyecto
- Simular un **Data Lake** mediante volúmenes en Databricks  
- Diseñar un pipeline ETL escalable y ordenado  
- Aplicar validaciones y transformaciones sobre los datos  
- Preparar información estructurada para consumo analítico  

---

## 🧰 Tecnologías utilizadas
- **Databricks**
- **Apache Spark (PySpark)**
- **Delta Lake**
- **Unity Catalog**
- **SQL**
- **Git / GitHub**

---

## 🧱 Arquitectura del proyecto

### **Bronze Layer**
- Creación de volúmenes para simular un Data Lake  
- Carga de archivos crudos (raw data)  

### **Silver Layer**
- Ingesta de datos:
  - Ventas  
  - Productos  
  - Clientes  
  - Sucursales  
- Validaciones:
  - Eliminación de duplicados  
  - Eliminación de valores nulos  
- Casteo de tipos de datos  
- Filtrado de registros innecesarios  
- Optimización de joins  
- Creación de tablas Silver  

### **Gold Layer**
- Creación de tablas finales optimizadas para análisis  

### **Orquestación**
- Configuración de un **Databricks Job** para automatizar el proceso ETL de ventas  

---

## 📂 Estructura del repositorio

📁 project-root
│
├── 📁 notebooks
│ ├── bronze/
│ ├── silver/
│ └── gold/
│
├── 📁 data
│ └── (archivos utilizados en la ingesta)
│
├── 📁 jobs
│ └── etl_ventas_job.json
│
└── README.md


📌 **Nota:**  
Los archivos utilizados para la ingesta de datos se encuentran dentro de la carpeta **`/data`** del repositorio.
