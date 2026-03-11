# Alura-Telecom
# Telecom X — Análisis de Evasión de Clientes

Proyecto de análisis exploratorio de datos (EDA) para identificar los factores asociados a la cancelación de servicios en Telecom X, como parte del Challenge de Data Science LATAM.


## Objetivo

Comprender el perfil de los clientes que cancelan el servicio (churn) y extraer insights que permitan al equipo de Data Science desarrollar modelos predictivos y estrategias de retención.


## Flujo de trabajo

**Extracción** — Carga del archivo JSON y normalización de la estructura anidada con `pd.json_normalize()`.

**Transformación** — Corrección de tipos de datos, eliminación de duplicados y nulos, y creación de las variables `Cuentas_Diarias` y `Churn_bin`.

**Análisis exploratorio** — Estadísticas descriptivas, visualización de la distribución de churn, análisis por variables categóricas y numéricas, servicios adicionales y matriz de correlación.

**Informe** — Conclusiones e insights con recomendaciones estratégicas.

## Cómo ejecutar

```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/telecomx-churn.git
cd telecomx-churn

# 2. Instalar dependencias
pip install pandas numpy matplotlib seaborn

# 3. Abrir el notebook
jupyter notebook TelecomX_LATAM.ipynb
```

---

## Principales hallazgos

- La tasa de evasión global es del **26%**.
- Los contratos **Month-to-month** concentran la mayor tasa de abandono (~42%).
- Los primeros **12 meses** son el período de mayor riesgo de cancelación.
- El método de pago **Electronic check** está fuertemente asociado al churn.
- Los servicios adicionales como `OnlineSecurity` y `TechSupport` actúan como factores de retención.

---

## Autor

Challenge Data Science LATAM — Alura + Oracle Next Education
