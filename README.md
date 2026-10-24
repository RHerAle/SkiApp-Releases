# SkiApp ⛷️📱 — El Navegador y Grabador GPS Definitivo para Esquiadores

[![Latest Release](https://img.shields.io/github/v/release/RHerAle/SkiApp-Releases?color=blue&label=Latest%20Release)](https://github.com/RHerAle/SkiApp-Releases/releases/latest)
[![Android](https://img.shields.io/badge/Platform-Android%208.0%2B%20(Oreo%20to%2015)-34D399?logo=android&logoColor=white)](https://developer.android.com)
[![Resorts](https://img.shields.io/badge/Ski%20Resorts-82%20Integrated-0284C7?logo=target&logoColor=white)](https://github.com/RHerAle/SkiApp-Releases#cat%C3%A1logo-completo-de-82-estaciones-de-esqu%C3%AD)
[![Offline Ready](https://img.shields.io/badge/Offline-100%25%20A*%20Pathfinding-F59E0B)](https://github.com/RHerAle/SkiNav)
[![OTA Updates](https://img.shields.io/badge/OTA%20Updates-GitHub%20Releases%20Feed-10B981)](https://api.github.com/repos/RHerAle/SkiApp-Releases/releases/latest)
[![License](https://img.shields.io/badge/Data%20License-ODbL--1.0-64748B)](https://opendatacommons.org/licenses/odbl/)

> **SkiApp** es la aplicación móvil definitiva para esquiadores y practicantes de snowboard. Combina un motor de navegación topológica de pistas y remontes en 2D/3D con cálculo de rutas óptimas mediante **A\***, telemetría meteorológica y de estado en vivo, horarios y tiempos de espera de **Ski Bus**, un grabador GPS GNSS de alta precisión con barómetro y cálculo metabólico de calorías, y un sistema de actualización automática Over-The-Air (**OTA**) integrado directamente con GitHub Releases.
>
> Diseñada para funcionar al 100% en alta montaña sin necesidad de cobertura ni consumo de datos móviles, integrando **82 estaciones de esquí** de España 🇪🇸, Italia 🇮🇹 y Francia 🇫🇷.

---

## 🌐 Idiomas / Languages
- [Español (Documentación Completa)](#-español)
- [English (Full Documentation)](#-english)

---

# 🇪🇸 Español

## 💡 ¿Qué es SkiApp y qué problema resuelve en la nieve?

Esquiar en grandes estaciones como Baqueira Beret, Les 3 Vallées, Val Gardena o Sierra Nevada suele presentar retos importantes:
1. **Pérdida de orientación y mapas en papel mojados o ilegibles:** Con decenas de kilómetros de pistas interconectadas y bifurcaciones a gran altitud, perderse o acabar en una pista de dificultad superior a tu nivel es habitual y peligroso.
2. **Cierres imprevistos de remontes por viento o aludes:** Un remonte cerrado en un collado puede dejarte atrapado en el valle equivocado sin saber cómo regresar antes de la hora de cierre.
3. **Falta de cobertura móvil:** Las apps comerciales basadas en la nube dejan de funcionar o agotan la batería cuando el smartphone pierde la señal en las cotas altas.
4. **Desconocimiento de los autobuses internos (`Ski Bus`):** En dominios extensos, conectar sectores mediante autobuses lanzadera suele requerir consultar horarios en paradas frías sin conocer los tiempos reales de espera.

**SkiApp resuelve todos estos problemas en una única aplicación Android nativa, ligera y 100% offline.**

---

## 📸 Galería Visual de Capturas de Pantalla

| 01. Mapa y Navegador Inteligente | 02. Estado en Vivo y Ski Bus |
| :---: | :---: |
| <img src="screenshots/01-mapa-navegador-baqueira.png" width="380" alt="Mapa y Navegador Baqueira Beret"/> | <img src="screenshots/02-estado-en-vivo-y-skibus.png" width="380" alt="Estado en Vivo y Ski Bus"/> |
| *Rutas A\* por nivel, pistas coloreadas, remontes, telemetría meteorológica en vivo y guiado paso a paso.* | *Diálogo interactivo de estado de remontes, tiempos de espera de Ski Bus y cierres manuales.* |

| 03. Grabador GPS & Telemetría | 04. Catálogo de 82 Estaciones | 05. Perfil & Actualizador OTA |
| :---: | :---: | :---: |
| <img src="screenshots/03-grabador-gps-telemetria.png" width="320" alt="Grabador GPS y Telemetría"/> | <img src="screenshots/04-catalogo-82-estaciones.png" width="320" alt="Catálogo 82 Estaciones"/> | <img src="screenshots/05-perfil-y-actualizador-ota.png" width="320" alt="Perfil y Actualizador OTA"/> |
| *Velocímetro en vivo (64.8 km/h), desnivel barométrico, detección automática de bajadas y exportación GPX.* | *Buscador y catálogo de 82 estaciones de España (31), Italia (48) y Francia (2).* | *Configuración biométrica de gasto calórico y actualizador automático in-app desde GitHub Releases.* |

---

## ⚡ Explicación Detallada de Pantallas y Funcionalidades

### 1. 🧭 Mapa Topográfico y Navegador A* de Pistas (`01-mapa-navegador-baqueira.png`)
- **Grafos Topológicos Reales:** Representación vectorizada de cada pista clasificada por su color oficial: verde (principiante), azul (fácil), roja (intermedia) y negra (experta). Los remontes se muestran en naranja con su trazado exacto.
- **Planificador de Rutas Inteligente:** Selecciona cualquier estación de origen (ej. *Baqueira 1500*) y destino (ej. *Beret Base*).
- **Filtro de Dificultad Máxima:** Si viajas con esquiadores principiantes o en familia, restringe el algoritmo para evitar pistas rojas o negras.
- **Alternativas de Ruta en un Toque:**
  - **Ruta Rápida:** Minimiza el tiempo total en remontes y bajadas.
  - **Ruta Fácil / Panorámica:** Prioriza pistas anchas y de baja pendiente.
  - **Ruta Ski-Only (sin bus):** Para quienes prefieren esquiar continuamente sin tomar vehículos de superficie.
- **Itinerario Paso a Paso:** Indicación detallada de cada remonte a tomar, pista a descender con distancia en kilómetros y estimación de tiempo.

### 2. 🌤️ Telemetría en Vivo, Horarios de Ski Bus y Cierres Manuales (`02-estado-en-vivo-y-skibus.png`)
- **Meteorología Alpina en Tiempo Real:** Integración con la API de Open-Meteo para obtener temperatura a diferentes cotas, velocidad y rachas de viento, espesor del manto nivoso y visibilidad.
- **Detección Automática de Cierres por Viento:** Algoritmo heurístico que advierte cuando rachas superiores a 50 km/h comprometen la apertura de telesillas y telecabinas.
- **Líneas de Ski Bus y Horarios Programados:** Muestra las líneas lanzadera internas (ej. *Gua-Gua Baqueira - Beret* o *Ski Bus Bonaigua*), su frecuencia de paso (cada 15 o 30 min) y calcula los minutos exactos de espera para la próxima salida en función de tu hora de llegada.
- **Gestión Interactiva de Cierres:** Si observas una pista balizada como cerrada o un remonte parado por avería técnica, puedes tocar sobre él o abrir el panel para marcarlo como `🔴 CERRADO`. El navegador recalculará inmediatamente una ruta alternativa que lo esquive. Puedes reabrirlo o restaurar los estados oficiales en cualquier momento.

### 3. ⛷️ Grabador GPS GNSS, Barómetro y Gasto Metabólico (`03-grabador-gps-telemetria.png`)
- **Frecuencia de Registro GNSS a 1 Hz:** Máxima precisión en curvas y virajes con filtrado de rebotes por efecto cañón o bosque.
- **Reconocimiento Automático de Actividad:** Detecta cuándo estás descendiendo esquiando (`⛷️ Descenso en pista`), subiendo en telesilla/telecabina (`🚡 Subida en remonte`), en autobús (`🚌 Desplazamiento en bus`) o en reposo (`⏸️ Estacionario`).
- **Velocímetro Digital:** Visualización de velocidad instantánea y registro de velocidad punta alcanzada.
- **Altímetro y Desnivel Barométrico:** Emplea el sensor de presión barométrica del teléfono para medir cotas exactas y registrar el desnivel vertical negativo acumulado.
- **Cálculo Metabólico de Calorías:** Emplea el estándar MET (Equivalente Metabólico de la Tarea) ajustado por la inclinación de la pendiente, la masa corporal y la altura del esquiador.
- **Exportación GPX Estándar:** Guarda tu sesión en formato GPX para compartirla o abrirla en Strava, Garmin Connect, Google Earth o Relive.

### 4. 🏔️ Catálogo Integrado de 82 Estaciones (`04-catalogo-82-estaciones.png`)
- Incluye las 82 estaciones más destacadas de la Península Ibérica, los Alpes y los Dolomitas:
  - **31 estaciones en España 🇪🇸:** Pirineo Aragonés y Catalán, Cordillera Cantábrica, Sistema Central, Sistema Ibérico y Sierra Nevada.
  - **48 estaciones en Italia 🇮🇹:** Cobertura de Dolomiti Superski, Valle d'Aosta, Lombardía, Piamonte, Trentino, Alto Adige, Friuli y Apeninos.
  - **2 mega-dominios en Francia 🇫🇷:** Les 3 Vallées (638 km esquiables) y Alpe d'Huez (182 km).
- **100% Precargadas Offline:** No requiere descargar megabytes adicionales mientras estás en viaje. Toda la topología viaja dentro de la aplicación.

### 5. 👤 Perfil y Actualizador Automático In-App OTA (`05-perfil-y-actualizador-ota.png`)
- **Perfil Biométrico:** Configuración de peso, altura, edad y nivel técnico para calibrar el algoritmo calórico.
- **Canal de Actualizaciones OTA GitHub Releases:**
  - Consulta directa a la API pública oficial de este repositorio (`RHerAle/SkiApp-Releases/releases/latest`).
  - Detección semántica de nuevas versiones (ej. de `v1.0.0` a `v2.0.0`).
  - Diálogo con notas de versión, barra de progreso en vivo y descarga del archivo APK.
  - Lanzamiento del instalador de paquetes de Android (`FileProvider`) con un solo toque.

---

## 🗺️ Catálogo Completo de 82 Estaciones de Esquí

<details>
<summary><b>🇪🇸 Ver las 31 Estaciones de Esquí de España (Desplegar)</b></summary>

| Estación de Esquí | Macizo / Región | Dominio Pistas | Remontes | Cota Mín - Máx | Desnivel |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Baqueira Beret** | Pirineo Catalán (Val d'Aran) | 152.3 km | 33 | 1.500m – 2.610m | 1.110 m |
| **Sierra Nevada** | Sistema Penibético (Granada) | 104.4 km | 20 | 2.100m – 3.300m | 1.200 m |
| **Formigal-Panticosa** | Pirineo Aragonés (Valle de Tena) | 128.2 km | 23 | 1.500m – 2.250m | 750 m |
| **Cerler** | Pirineo Aragonés (Valle de Benasque) | 126.5 km | 19 | 1.500m – 2.630m | 1.130 m |
| **Candanchú** | Pirineo Aragonés (Valle del Aragón) | 44.9 km | 37 | 1.530m – 2.400m | 870 m |
| **Astún** | Pirineo Aragonés (Valle del Aragón) | 30.9 km | 17 | 1.700m – 2.300m | 600 m |
| **La Molina** | Pirineo Catalán (La Cerdanya) | 91.4 km | 33 | 1.700m – 2.445m | 745 m |
| **Masella** | Pirineo Catalán (La Cerdanya) | 68.4 km | 23 | 1.600m – 2.535m | 935 m |
| **Boí Taüll** | Pirineo Catalán (Alta Ribagorça) | 33.9 km | 9 | 2.035m – 2.751m | 716 m |
| **Port Ainé** | Pirineo Catalán (Pallars Sobirà) | 20.5 km | 8 | 1.650m – 2.440m | 790 m |
| **Espot Esquí** | Pirineo Catalán (Pallars Sobirà) | 19.4 km | 6 | 1.500m – 2.500m | 1.000 m |
| **Port del Comte** | Prepirineo Catalán (Solsonès) | 30.5 km | 19 | 1.700m – 2.400m | 700 m |
| **Vallter 2000** | Pirineo Catalán (Ripollès) | 13.1 km | 10 | 1.910m – 2.535m | 625 m |
| **Vall de Núria** | Pirineo Catalán (Ripollès) | 5.9 km | 7 | 1.964m – 2.252m | 288 m |
| **Tavascan** | Pirineo Catalán (Pallars Sobirà) | 3.8 km | 3 | 1.750m – 2.250m | 500 m |
| **Alto Campoo** | Cordillera Cantábrica (Cantabria) | 19.7 km | 11 | 1.650m – 2.125m | 475 m |
| **San Isidro** | Cordillera Cantábrica (León) | 23.5 km | 14 | 1.500m – 2.100m | 600 m |
| **Fuentes de Invierno**| Cordillera Cantábrica (Asturias) | 10.2 km | 5 | 1.487m – 1.950m | 463 m |
| **Valgrande-Pajares** | Cordillera Cantábrica (Asturias) | 15.3 km | 6 | 1.450m – 1.890m | 440 m |
| **Valle Laciana - Leitariegos** | Cordillera Cantábrica (León) | 6.1 km | 6 | 1.513m – 1.800m | 287 m |
| **Cabeza de Manzaneda**| Macizo Galaico (Ourense) | 12.2 km | 6 | 1.500m – 1.778m | 278 m |
| **Valdesquí** | Sistema Central (Madrid / Segovia) | 36.0 km | 15 | 1.860m – 2.280m | 420 m |
| **Puerto de Navacerrada**| Sistema Central (Madrid / Segovia) | 2.9 km | 6 | 1.700m – 2.177m | 477 m |
| **La Pinilla** | Sistema Central (Segovia) | 11.2 km | 13 | 1.500m – 2.050m | 550 m |
| **Sierra de Béjar - La Covatilla** | Sistema Central (Salamanca) | 14.2 km | 4 | 1.990m – 2.368m | 378 m |
| **Valdezcaray** | Sistema Ibérico (La Rioja) | 15.7 km | 9 | 1.530m – 2.125m | 595 m |
| **Aramón Javalambre** | Sistema Ibérico (Teruel) | 8.7 km | 9 | 1.650m – 2.000m | 350 m |
| **Aramón Valdelinares** | Sistema Ibérico (Teruel) | 9.2 km | 12 | 1.700m – 2.024m | 324 m |
| **Punto de Nieve Santa Inés** | Sistema Ibérico (Soria) | 1.0 km | 2 | 1.753m – 1.832m | 79 m |
| **Panticosa (Sector Independiente)** | Pirineo Aragonés | 18.3 km | 15 | 1.145m – 2.220m | 1.075 m |
| **Lunada** | Cordillera Cantábrica (Burgos) | 6.1 km | 5 | 1.280m – 1.445m | 165 m |

</details>

<details>
<summary><b>🇮🇹 Ver las 48 Estaciones de Esquí de Italia (Desplegar)</b></summary>

| Estación de Esquí | Región / Dominio | Dominio Pistas | Remontes | Cota Mín - Máx | Desnivel |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Val Gardena - Alpe di Siusi** | Dolomiti Superski (Südtirol) | 239.6 km | 83 | 1.236m – 2.518m | 1.282 m |
| **Breuil-Cervinia Valtournenche** | Valle d'Aosta (Matterhorn) | 196.5 km | 35 | 1.524m – 3.883m | 2.359 m |
| **Alta Badia** | Dolomiti Superski (Südtirol) | 146.6 km | 54 | 1.324m – 2.778m | 1.454 m |
| **La Thuile (Espace San Bernardo)** | Valle d'Aosta | 147.2 km | 18 | 1.440m – 2.800m | 1.360 m |
| **Via Lattea (Sestriere - Sauze d'Oulx)** | Piemonte | 479.9 km | 80 | 1.350m – 2.823m | 1.473 m |
| **3 Zinnen Dolomites (Sexten)** | Dolomiti Superski | 129.9 km | 23 | 1.130m – 2.200m | 1.070 m |
| **Livigno** | Lombardia | 125.0 km | 31 | 1.816m – 2.798m | 982 m |
| **Courmayeur Mont Blanc** | Valle d'Aosta | 91.1 km | 22 | 1.210m – 2.755m | 1.545 m |
| **Cortina d'Ampezzo** | Dolomiti Superski (Veneto) | 90.0 km | 28 | 1.224m – 2.930m | 1.706 m |
| **Val di Fassa (Belvedere - Col Rodella)** | Dolomiti Superski (Trentino) | 89.2 km | 27 | 1.320m – 2.485m | 1.165 m |
| **Campiglio Dolomiti di Brenta** | Trentino | 88.5 km | 39 | 850m – 2.504m | 1.654 m |
| **Kronplatz - Plan de Corones** | Dolomiti Superski (Südtirol) | 88.2 km | 25 | 935m – 2.275m | 1.340 m |
| **Ski Center Latemar (Obereggen)** | Dolomiti Superski | 85.5 km | 20 | 1.540m – 2.388m | 848 m |
| **Bormio** | Lombardia | 72.2 km | 14 | 1.225m – 3.012m | 1.787 m |
| **Mondolè Ski (Prato Nevoso)** | Piemonte | 72.2 km | 24 | 1.300m – 2.085m | 785 m |
| **Alpe Lusia - San Pellegrino** | Dolomiti Superski | 68.4 km | 16 | 1.370m – 2.513m | 1.143 m |
| **Monterosa Ski** | Valle d'Aosta / Piemonte | 66.5 km | 26 | 1.212m – 3.275m | 2.063 m |
| **Alto Sangro - Roccaraso** | Abruzzo (Apeninos) | 63.8 km | 28 | 1.390m – 2.141m | 751 m |
| **Ski Civetta (Alleghe - Zoldo)** | Dolomiti Superski (Veneto) | 57.9 km | 26 | 1.000m – 2.100m | 1.100 m |
| **Arabba - Marmolada** | Dolomiti Superski (Veneto) | 57.0 km | 21 | 1.446m – 3.269m | 1.823 m |
| **Pontedilegno-Tonale** | Lombardia / Trentino | 55.1 km | 31 | 1.121m – 3.016m | 1.895 m |
| **Pila** | Valle d'Aosta | 55.0 km | 16 | 1.540m – 2.750m | 1.210 m |
| **Bardonecchia** | Piemonte | 52.8 km | 19 | 1.312m – 2.800m | 1.488 m |
| **San Martino di Castrozza** | Dolomiti Superski (Trentino) | 51.0 km | 19 | 1.404m – 2.357m | 953 m |
| **Chiesa in Valmalenco** | Lombardia | 49.8 km | 9 | 1.000m – 2.336m | 1.336 m |
| **Abetone - Val di Luce** | Toscana (Apeninos) | 49.7 km | 18 | 1.240m – 1.892m | 652 m |
| **Monte Cimone** | Emilia-Romagna (Apeninos) | 49.0 km | 21 | 900m – 2.165m | 1.265 m |
| **Alpe Cimbra (Folgaria)** | Trentino | 46.9 km | 31 | 1.166m – 1.850m | 684 m |
| **Foppolo - Carona (Brembo Ski)** | Lombardia | 46.0 km | 12 | 1.500m – 2.163m | 663 m |
| **Folgarida - Marilleva** | Trentino | 42.9 km | 26 | 1.300m – 2.180m | 880 m |
| **Limone Piemonte (Riserva Bianca)** | Piemonte | 40.5 km | 17 | 1.050m – 2.050m | 1.000 m |
| **Solda all'Ortles (Sulden)** | Südtirol | 35.6 km | 11 | 1.900m – 3.250m | 1.350 m |
| **Santa Caterina Valfurva** | Lombardia | 34.9 km | 6 | 1.738m – 2.880m | 1.142 m |
| **Madesimo Valchiavenna** | Lombardia | 34.7 km | 12 | 1.550m – 2.948m | 1.398 m |
| **Paganella Ski (Andalo)** | Trentino | 33.1 km | 14 | 1.030m – 2.125m | 1.095 m |
| **Val Senales (Schnalstal)** | Südtirol | 32.3 km | 12 | 2.011m – 3.212m | 1.201 m |
| **Belpiano - Passo Resia** | Südtirol | 26.5 km | 14 | 1.460m – 2.390m | 930 m |
| **Plose (Bressanone)** | Südtirol | 25.0 km | 7 | 1.067m – 2.505m | 1.438 m |
| **Speikboden & Klausberg** | Südtirol (Valle Aurina) | 24.9 km | 9 | 950m – 2.510m | 1.560 m |
| **Carezza Dolomites** | Dolomiti Superski | 24.2 km | 13 | 1.182m – 2.337m | 1.155 m |
| **Tarvisio - Monte Lussari** | Friuli-Venezia Giulia | 24.0 km | 17 | 754m – 1.760m | 1.006 m |
| **Racines-Giovo (Ratschings)** | Südtirol | 23.7 km | 11 | 1.300m – 2.150m | 850 m |
| **Monte Zoncolan** | Friuli-Venezia Giulia | 23.7 km | 17 | 950m – 1.970m | 1.020 m |
| **San Domenico di Varzo** | Piemonte | 19.9 km | 7 | 1.420m – 2.550m | 1.130 m |
| **Gitschberg Jochtal** | Südtirol | 17.2 km | 10 | 1.307m – 2.510m | 1.203 m |
| **Piani di Bobbio - Valtorta** | Lombardia | 17.0 km | 12 | 1.340m – 1.950m | 610 m |
| **Ovindoli & Campo Felice** | Abruzzo (Apeninos) | 15.4 km | 12 | 1.400m – 2.220m | 820 m |
| **Aprica** | Lombardia | 13.7 km | 7 | 1.180m – 2.300m | 1.120 m |

</details>

<details>
<summary><b>🇫🇷 Ver los Grandes Dominios de Francia (Desplegar)</b></summary>

| Estación / Dominio | Departamento / Macizo | Dominio Pistas | Remontes | Cota Mín - Máx | Desnivel |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Les 3 Vallées** (Val Thorens, Méribel, Courchevel, Les Menuires) | Savoie (Alpes Franceses) | 638.2 km | 102 | 1.300m – 3.230m | 1.930 m |
| **Alpe d'Huez** (Grand Domaine Ski) | Isère (Grandes Rousses) | 182.3 km | 61 | 1.100m – 3.330m | 2.230 m |

</details>

---

## 📥 Guía de Instalación y Funcionamiento del Botón "🔄 Actualizar App"

### Instalación Inicial (Paso a Paso)
1. **Descarga el APK:** Ve a la [página de Latest Release](https://github.com/RHerAle/SkiApp-Releases/releases/latest) y pulsa en `SkiApp-v2.0.0.apk`.
2. **Autoriza la instalación:** Al abrir el archivo en tu dispositivo Android, si el sistema te solicita *"Permitir desde esta fuente"* (instalación de aplicaciones desconocidas), actívalo en los ajustes de seguridad.
3. **Instala y Abre:** Completa la instalación y disfruta de SkiApp en cualquier rincón nevado.

### ¿Cómo funciona el botón "🔄 Actualizar App"?
- Tanto en la esquina superior derecha del planificador de rutas como en la pestaña de **Perfil**, encontrarás el botón **`🔄 Actualizar App`**.
- Al pulsarlo, SkiApp realiza una consulta HTTP asíncrona a la API pública de GitHub:
  ```text
  GET https://api.github.com/repos/RHerAle/SkiApp-Releases/releases/latest
  ```
- Compara la versión local del paquete (`BuildConfig.VERSION_NAME`) con el tag remoto mediante comparación semántica de versiones (`AppUpdateManager.isNewerVersion`).
- Si existe una versión superior, muestra una ventana modal con el resumen de cambios, descarga el APK con barra de progreso interactiva y abre el instalador oficial de Android de forma limpia y desatendida.

---
---

# 🇬🇧 English

## 💡 What is SkiApp and what problem does it solve in the snow?

Skiing in massive mountain resorts such as Baqueira Beret, Les 3 Vallées, Val Gardena, or Sierra Nevada presents major navigational hurdles:
1. **Disorientation & soggy paper trail maps:** With hundreds of interconnected pistes and high-altitude junctions, getting lost or inadvertently entering a trail beyond your technical ability is both stressful and hazardous.
2. **Unexpected lift closures due to wind or avalanche control:** When a key ridge lift closes, skiers can end up stranded in the wrong valley with no quick route back before lifts close for the day.
3. **Loss of cellular signal:** Commercial cloud-dependent apps fail to load or drain your battery searching for signal at high elevations.
4. **Internal Ski Bus schedules:** Connecting distant base areas by shuttle bus often requires guesswork at freezing stops without knowing actual wait times.

**SkiApp resolves all of these pain points in a single, lightweight, native Android app that runs 100% offline.**

---

## 📸 Visual Screenshot Gallery

| 01. Intelligent Trail Map & Router | 02. Live Mountain Status & Ski Bus |
| :---: | :---: |
| <img src="screenshots/01-mapa-navegador-baqueira.png" width="380" alt="Trail Map & Router Baqueira Beret"/> | <img src="screenshots/02-estado-en-vivo-y-skibus.png" width="380" alt="Live Status and Ski Bus"/> |
| *A\* routing by difficulty, color-coded pistes, lift lines, live weather telemetry and step-by-step turns.* | *Interactive operational status dialog, Ski Bus schedules, countdown timers, and manual closures.* |

| 03. GPS Logger & Telemetry | 04. 82 Ski Resorts Catalog | 05. Profile & In-App OTA Updater |
| :---: | :---: | :---: |
| <img src="screenshots/03-grabador-gps-telemetria.png" width="320" alt="GPS Tracker Telemetry"/> | <img src="screenshots/04-catalogo-82-estaciones.png" width="320" alt="82 Resorts Catalog"/> | <img src="screenshots/05-perfil-y-actualizador-ota.png" width="320" alt="Profile & OTA Updater"/> |
| *Live speedometer (64.8 km/h), barometric altitude, automatic run detection and GPX export.* | *Instant search and catalog of 82 ski resorts across Spain (31), Italy (48), and France (2).* | *Biometric calorie profile and direct in-app Over-The-Air APK updater from GitHub Releases.* |

---

## ⚡ Core Features & Technical Overview

### 1. 🧭 Topological Piste Map & A* Pathfinder (`01-mapa-navegador-baqueira.png`)
- **Real Vector Topologies:** Pistes color-coded by European difficulty standards: green (beginner), blue (intermediate), red (advanced), and black (expert). Lifts are rendered in high-contrast orange.
- **Smart Wayfinding:** Set any departure station (e.g. *Baqueira 1500*) and destination (e.g. *Beret Base*).
- **Max Difficulty Filter:** Tailor the pathfinder to restrict runs strictly within your comfort zone (e.g., green/blue only).
- **Instant Route Alternatives:**
  - **Fastest Route:** Minimizes cumulative lift and ski time.
  - **Easiest / Scenic Route:** Favors gentle gradients and wide cruising trails.
  - **Ski-Only (No Bus):** Avoids shuttle transfers for continuous ski descent.
- **Step-by-Step Directions:** Exact list of lifts, connecting trails, distances in kilometers, and estimated minutes.

### 2. 🌤️ Live Telemetry, Ski Bus Timetables & Manual Overrides (`02-estado-en-vivo-y-skibus.png`)
- **Real-Time Alpine Meteorology:** Queries Open-Meteo for multi-elevation temperatures, wind velocity, gusts, snow depth, and sky conditions.
- **Automated High-Wind Hold Detection:** Flags lifts susceptible to closure when wind gusts exceed 50 km/h.
- **Ski Bus Timetables & Wait Time Calculation:** Integrates resort shuttle lines with departure frequencies and computes remaining wait times relative to your departure hour.
- **Interactive Manual Overrides:** Tap any lift or slope on the map or in the dialog to toggle between `🟢 OPEN` and `🔴 CLOSED`. The routing engine recalculates optimal paths around closed infrastructure instantaneously.

### 3. ⛷️ GNSS GPS Tracker, Barometer & Calorie Engine (`03-grabador-gps-telemetria.png`)
- **1 Hz High-Precision Telemetry:** Accurately logs curves without mountain canyon multi-pathing artifacts.
- **Real-Time Activity Recognition:** Automatically distinguishes between skiing downhill (`⛷️ Downhill Skiing`), riding a chairlift or gondola (`🚡 Riding Lift`), taking a shuttle (`🚌 Ski Bus`), or staying stationary (`⏸️ Stationary`).
- **Real-Time Speedometer:** Large digital gauge with current speed and peak velocity tracker.
- **Barometric Altimeter:** Leverages device barometric hardware for vertical drop calculations.
- **MET Metabolic Calorie Calculation:** Calibrated to body mass, height, age, and slope incline.
- **Standard GPX Export:** One-tap export to share your sessions with Strava, Garmin Connect, Google Earth, or Relive.

### 4. 🏔️ Built-In Catalog of 82 Ski Resorts (`04-catalogo-82-estaciones.png`)
- Preloaded with the top 82 ski domains in Europe:
  - **31 resorts in Spain 🇪🇸:** Pyrenees, Cantabrian Range, Central System, Iberian System, and Sierra Nevada.
  - **48 resorts in Italy 🇮🇹:** Dolomiti Superski, Valle d'Aosta, Lombardy, Piedmont, Trentino, South Tyrol, and Apennines.
  - **2 mega-resorts in France 🇫🇷:** Les 3 Vallées (638 km) and Alpe d'Huez (182 km).
- **100% Offline Topology:** No map data downloads needed on the mountain. Everything is bundled directly into the app.

### 5. 👤 Profile & Over-The-Air (OTA) In-App Updater (`05-perfil-y-actualizador-ota.png`)
- **Biometric Calibration:** Store your physical specs to tune telemetry algorithms.
- **Direct GitHub Releases OTA Distribution:**
  - Queries `https://api.github.com/repos/RHerAle/SkiApp-Releases/releases/latest`.
  - Performs semantic version checks without requiring Google Play Store or third-party stores.
  - In-app download with visual progress bar and clean Android package installer launch.

---

## 📥 Installation & In-App Update Guide

### Initial Installation
1. **Download APK:** Open the [Latest Release Page](https://github.com/RHerAle/SkiApp-Releases/releases/latest) and tap `SkiApp-v2.0.0.apk`.
2. **Authorize Unknown Sources:** If prompted by Android, grant permission to install from your browser or file manager.
3. **Launch & Ski:** Open SkiApp and select your favorite resort.

### How the "🔄 Actualizar App" Button Works
- Located in the top-right corner of the route planner and inside the **Profile** screen.
- Clicking the button initiates an asynchronous check to the GitHub Releases API.
- If a newer version is published, SkiApp prompts you with release highlights, downloads the APK, and invokes Android's `FileProvider` package installer.

---

## 📄 License & Open-Source Attribution
- **Application Codebase:** [RHerAle/ski-app](https://github.com/RHerAle/ski-app)
- **Topological Routing Engine:** [RHerAle/SkiNav](https://github.com/RHerAle/SkiNav)
- **GPS Telemetry Engine:** [RHerAle/SkiTracker](https://github.com/RHerAle/SkiTracker)
- **Geographical & Resort Data:** OpenStreetMap & Open Database License ([ODbL-1.0](https://opendatacommons.org/licenses/odbl/)).
