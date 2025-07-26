# 📊 Análisis de Evasión de Clientes – TelecomX LATAM

Este proyecto de análisis de datos tiene como objetivo identificar patrones relacionados con la **evasión de clientes (churn)** en la empresa ficticia de telecomunicaciones **TelecomX LATAM**. La evasión representa una pérdida importante en el sector, y anticiparse a ella es clave para la rentabilidad.

---

## 📌 Objetivo

Detectar factores que influyen en la baja de clientes mediante análisis exploratorio y proponer **estrategias de retención** con base en los datos disponibles.

---

## 📂 Fuente de Datos

Se utilizó un archivo en formato `.json` llamado `TelecomX_Data.json`, que contiene información de más de 7.200 clientes, incluyendo:

- Datos demográficos (edad, género, dependientes)
- Servicios contratados (internet, telefonía, seguridad)
- Información de cuenta (tipo de contrato, método de pago, cargos)
- Variable objetivo: `Churn` (indica si el cliente se dio de baja)

---

## 🧹 Limpieza y Preparación

- **Normalización** de campos anidados (`customer`, `phone`, `internet`, `account`).
- Conversión de columnas a **formato uniforme y tipado correcto**.
- Reemplazo de valores categóricos (`yes/no` → `1/0`) para análisis estadísticos.
- Creación de campo `Cuentas_Diarias` (cargos mensuales / 30).
- Imputación de valores nulos y control de duplicados.

---

## 📊 Análisis Exploratorio

Se realizaron gráficos y estadísticas para responder las siguientes preguntas:

- ¿Qué proporción de clientes se han dado de baja?
- ¿Influye el género o el tipo de contrato en la evasión?
- ¿Hay métodos de pago asociados a mayor churn?
- ¿Cuál es el perfil de gasto de los clientes evadidos?

### Visualizaciones clave:
- Pie chart de distribución de churn
- Gráfico de barras por género, tipo de contrato y tipo de pago
- Análisis del total gastado y gasto mensual según churn

---

## 🧠 Principales Hallazgos

- La mayoría de clientes evadidos tienen contrato **mes a mes**.
- El método **electronic check** está fuertemente asociado a la evasión.
- Clientes con menor permanencia (`tenure`) son más propensos a irse.
- La evasión ocurre incluso entre clientes de **alto valor económico**.

---

## ✅ Recomendaciones

- Fomentar contratos a largo plazo con incentivos.
- Mejorar experiencia de pago y seguridad en métodos digitales.
- Implementar modelos predictivos para **identificar churn anticipado**.
- Diseñar campañas proactivas para retener clientes de alto riesgo.

---

## 🛠 Tecnologías Utilizadas

- Python
- Pandas
- Matplotlib
- Google Colab

---

## 📎 Autor

Este análisis forma parte de un desafío práctico de ciencia de datos.
