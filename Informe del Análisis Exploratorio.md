# 📄Informe Análisis Exploratorio

##  🔍 1. Introducción

Este análisis busca identificar los patrones que explican el abandono de clientes (churn) en el sector de telecomunicaciones.
El churn representa una amenaza clave para la retención, al reflejar la pérdida de usuarios activos.
Detectar los factores asociados permite tomar decisiones informadas.
Esto facilita mejorar la experiencia del cliente y reducir la rotación.

## 🧹 2. Limpieza y Tratamiento de Datos

Se cargaron los datos desde un archivo .json (TelecomX_Data.json) usando pandas. Las variables incluyen información demográfica, servicios contratados, duración del contrato y cargos mensuales y totales entre otros.

🧺 Pasos de limpieza realizados:

- Se Aplanó cada columna del diccionrio.
- Se convirtieron variables categóricas a tipo category.
- Se creó una variable binaria llamada "cols_a_binarias"  para facilitar cálculos posteriores ('Yes' → 1, 'No' → 0).
- Se verificó la ausencia de valores nulos.
- Se trató datos duplicados.

## 📈 Variables numéricas procesadas:

- tenure: Meses con la compañía.
- charges_monthly: Cargo mensual.
- charges_total: Total acumulado pagado.
- tenure_days: Tiempo en días (derivado).
- cuentas_diarias: Para calcular el valor diario.

## 📊 3. Análisis Exploratorio de Datos

### 📌 Distribución general del Churn

<img width="1046" height="494" alt="image" src="https://github.com/user-attachments/assets/6c38f994-b244-45b6-b65c-248464755233" />

### 📃📈 **Análisis:** Un 26.6% de los clientes analizados han abandonado el servicio.

### 📌📌 Por tipo de contrato:

<img width="567" height="425" alt="image" src="https://github.com/user-attachments/assets/bc5598fa-160e-451a-bd10-50ea92364ec3" />

### 📃📈 Análisis:  Los clientes con contrato mensual tienen una tasa de abandono mucho mayor que quienes tienen contratos anuales o bienales.

---

## 📝 4. 📌 Principales hallazgos:

### 1. Los contratos mensuales tienen mayor churn.
- Indican menor compromiso por parte del cliente.
- Representa un grupo prioritario para acciones de fidelización.

### 2. Clientes nuevos tienden a irse antes.
- Baja tenure está correlacionada con abandono temprano.
- Requiere atención durante las primeras semanas/meses.

### 3. Altos cargos mensuales sin valor percibido aumentan el riesgo de churn.
- Puede ser un síntoma de mala percepción del servicio o falta de personalización.

### 4. Método de pago automático reduce el abandono.
- Facilita la continuidad del servicio.
- Puede usarse como incentivo para fidelizar.


## 🚀 5. Recomendaciones

### 1. Ofrecer descuentos por contratos anuales o bienales
- Incentivar el cambio de contrato mensual a largo plazo.
- Ejemplo: regalo de meses adicionales o bonificaciones.

### 2. Programa de onboarding para nuevos clientes
- Mejorar la primera experiencia para reducir abandono temprano.
- Ofrecer guías, soporte técnico inicial o beneficios iniciales.

### 3. Segmentación por gasto mensual
- Ofrecer planes alternativos o paquetes premium a clientes de alto valor.
- Personalizar ofertas para evitar que clientes de alto costo se vayan.

### 4. Promoción de pago automático
- Beneficios exclusivos para clientes con pago automático (ej. descuentos, acceso a contenido adicional).

### 5. Monitoreo proactivo de clientes de alto riesgo
- Implementar modelos predictivos para identificar clientes con alta probabilidad de abandonar.
- Contactarlos antes de que tomen la decisión final.

## ✅ Conclusión

  Este análisis exploratorio ha permitido identificar patrones claros que explican el comportamiento de los clientes frente al abandono. Con esta información, se pueden diseñar estrategias efectivas para disminuir el churn , incrementar la retención y mejorar la rentabilidad a largo plazo.

---


