![](https://raw.githubusercontent.com/gabrielfernando01/RetailSparkFlow/main/image/cover.png)

# 🛒 RetailSparkFlow.

Pipeline de datos de extremo a extremo con Apache Spark, Scala, S3/MinIO y Spring Boot.

💡 Objetivos

1. Procesar un conjunto de datos públicos de Kaggle con tráfico transaccional.
2. Realizar limpieza, validación y transformaciones con Spark en Scala.
3. Almacenar resultados en Parquet o JSON en un bucket S3 (o en local usando MinIO).
4. Exponer los resultados como endpoints JSON con una API REST en Spring Boot.

🚀 Requisitos previos

- Java 11+ y Scala 2.12+
- sbt o Maven
- Docker y Docker Compose (para MinIO)
- IDE (IntelliJ, VS Code…)
- Cuenta en AWS o uso local de MinIO

## ⚙️ 1. Preparar el entorno del repositorio.

🔗 Fuente de los datos

Utilizaremos el dataset “Online Retail II”, con más de 500 k transacciones reales de un comercio electrónico del Reino Unido entre diciembre 2009 y diciembre 2011. Es ideal para un proyecto de Big Data con Spark por su volumen y complejidad <code>kaggle.com</code>

Ubicación del dataset en Kaggle: <code>https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset</code>

![](https://raw.githubusercontent.com/gabrielfernando01/RetailSparkFlow/main/image/structure.png)

## 📥 2. Descargar y colocar el dataset.

- Accede al enlace de Kaggle y descarga online_retail_II.csv.
- Mueve el CSV a data/online_retail.csv.