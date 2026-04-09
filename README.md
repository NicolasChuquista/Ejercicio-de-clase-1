# AquaBalde 🪣💧
> [cite_start]Sistema Inteligente de Monitoreo de Calidad de Agua para Comunidades Rurales y Periurbanas[cite: 3].

## ⚠️ El Problema
[cite_start]En numerosas comunidades rurales y periurbanas, miles de familias recurren a la recolección de agua proveniente de fuentes naturales (ríos, lagos, pozos y manantiales) y la almacenan en recipientes domésticos sin ningún tipo de control de calidad[cite: 18, 19]. [cite_start]La imposibilidad de conocer en tiempo real si esta agua es segura expone a la población a severos riesgos sanitarios y enfermedades de transmisión hídrica (ETH)[cite: 20, 21, 29]. 

Esta realidad refleja una brecha crítica en el cumplimiento de los lineamientos de la OMS y los estándares nacionales, como el **DS N° 031-2010-SA (Reglamento de la Calidad del Agua para Consumo Humano)** en Perú.

## 💡 La Solución
[cite_start]**AquaBalde** es un sistema integrado de monitoreo de calidad de agua diseñado para funcionar directamente en un balde de doble pared estándar fabricado en HDPE virgen, grado alimentario[cite: 48, 144]. [cite_start]El dispositivo combina hardware de bajo consumo con sensores electroquímicos y ópticos para evaluar el agua almacenada[cite: 49].

[cite_start]El usuario final no requiere conocimientos técnicos: tras llenar el recipiente, el sistema evalúa la muestra y en menos de 60 segundos indica si el agua es **APTA** o **NO APTA** para consumo humano[cite: 50].

### ⚙️ Características Principales
* [cite_start]**Interfaz Intuitiva:** Resultados mostrados mediante una pantalla OLED 1.3" y un código de colores semafórico (LEDs RGB)[cite: 64, 112].
* [cite_start]**Prevención de Contaminación Cruzada:** Diseño con cierre hermético y componentes encapsulados (IP67) entre las capas del balde[cite: 49, 146, 152].
* [cite_start]**Bajo Costo y Autonomía:** Funciona con una batería LiPo de 3000mAh (recargable vía solar o micro-USB), eliminando suscripciones y utilizando únicamente un biosensor de recarga anual[cite: 63, 67, 112].

## 📊 Parámetros Monitoreados
[cite_start]El sistema implementa una lógica de decisión basada en umbrales normativos[cite: 55]. [cite_start]El agua se clasifica como APTA solo si todos los parámetros están dentro del rango seguro[cite: 57]:

* [cite_start]**pH:** Medido vía electrodo ISFET/vidrio (Rango seguro: 6.5 - 8.5)[cite: 53, 115].
* [cite_start]**Turbidez:** Medido con sensor óptico infrarrojo de 880nm (Límite: < 5 NTU)[cite: 53, 120].
* [cite_start]**Conductividad Eléctrica:** Medido mediante electrodo de acero 316L de 2 puntas (Límite: < 400 µS/cm)[cite: 53, 126].
* [cite_start]**Coliformes Termotolerantes:** Detección cualitativa mediante biosensor enzimático (Límite: 0 UFC/100mL)[cite: 53, 131].

## 🌍 Impacto y ODS (Objetivos de Desarrollo Sostenible)
[cite_start]AquaBalde tiene un alineamiento directo con la Agenda 2030 de Naciones Unidas[cite: 198]:
* [cite_start]**ODS 6 (Agua Limpia y Saneamiento):** Contribuye a la Meta 6.1 al democratizar la verificación de la aptitud del agua en comunidades sin infraestructura hídrica[cite: 199].
* [cite_start]**ODS 3 (Salud y Bienestar):** Actúa como herramienta preventiva para reducir la mortalidad infantil y las enfermedades transmisibles al alertar sobre agua contaminada antes de su consumo[cite: 199].

## 🛠️ Stack Tecnológico (Hardware & Firmware)
* [cite_start]**Microcontrolador:** ESP32-S3 WROOM (Xtensa LX7 Dual Core 240MHz)[cite: 112, 217].
* [cite_start]**Firmware:** Desarrollo en C/C++ utilizando FreeRTOS + ESP-IDF[cite: 157].
* [cite_start]**Conectividad:** WiFi 2.4GHz y Bluetooth LE 5.0 integrados para transmisión opcional de datos[cite: 112].
* [cite_start]**ADC:** Conversor Analógico-Digital de 12-bit integrado para adquisición de datos de sensores[cite: 112].
