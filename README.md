**Institución:** Universidad de San Carlos de Guatemala 

**Curso:** Practicas Iniciales 

**Estudiante:** Luis Alejandro Pocón Sutuj  ``202403172``

**Hardware de Referencia:** Arquitectura Intel Celeron 4205U (8GB RAM / 240GB SSD)  

---

## 1. INTRODUCCIÓN Y DIAGNÓSTICO INICIAL

### 1.1 El Polvo como Aislante Térmico
El mantenimiento preventivo consiste en crear un ambiente favorable para el sistema informático y conservar limpias todas las partes que componen una computadora. El mayor porcentaje de fallas mecánicas y electrónicas en computadoras portátiles es causado por la **acumulación de polvo en los componentes internos**. El polvo actúa como un **aislante térmico**, atrapando el calor generado por los semiconductores e impidiendo su correcta dispersión hacia el ambiente. Al mezclarse con partículas de grasa presentes en el aire, se crea una capa espesa que reduce drásticamente la vida útil del procesador y puede provocar cortocircuitos debido a elementos conductores microscópicos.

### 1.2 Diagnóstico Operativo Previo
Antes de retirar un solo tornillo del chasis, es estrictamente obligatorio realizar una auditoría de software con el equipo encendido para detectar fallas preexistentes:
1. Verificar la integridad física y el funcionamiento de cada tecla del teclado.
2. Comprobar el desplazamiento y la respuesta de los botones del *touchpad*.
3. Validar los tiempos de arranque del Sistema Operativo Windows y el reconocimiento correcto del almacenamiento (~240 GB SSD) y la memoria RAM (8 GB) en la herramienta de Información del Sistema.
4. Anotar cualquier anomalía encontrada para deslindar responsabilidades técnicas antes de la intervención física.

---

## 2. COMPONENTES PRINCIPALES DE LA LAPTOP (HARDWARE DE REFERENCIA)

A diferencia de una computadora de escritorio (PC AT/ATX tradicional), una laptop integra la mayoría de sus interfaces directamente en una sola tarjeta de circuito impreso miniaturizada.

| Componente | Descripción Técnica | Especificación del Equipo |
| :--- | :--- | :--- |
| **Microprocesador (CPU)** | Unidad Central de Proceso encargada de analizar, ejecutar instrucciones y controlar el flujo de datos. Posee una Unidad de Control y una Unidad Aritmética Lógica (UAL). | **Intel Celeron 4205U** (Generación Whiskey Lake, 15W TDP, bajo consumo térmico). |
| **Tarjeta Madre (Motherboard)** | Circuito impreso principal que interconecta de forma compacta el procesador, los puertos y los zócalos de memoria. | Arquitectura integrada de bajo perfil (All-in-One portátil). |
| **Memoria RAM** | Memoria volátil de acceso rápido encargada de almacenar los datos de los programas en ejecución. | **8 GB DDR4** (Puede presentarse soldada a la placa o en formato de ranura SODIMM). |
| **Unidad de Almacenamiento** | Dispositivo magnético o de estado sólido para el resguardo permanente de la información. | **SSD de ~240 GB** (Interfaz M.2 SATA/NVMe o formato de 2.5 pulgadas de alta velocidad). |
| **Sistema de Enfriamiento** | Conjunto mecánico compuesto por un disipador de cobre acoplado al CPU y un ventilador extractor compacto de 5V. | Bloque térmico optimizado para procesadores móviles de bajo voltaje. |
| **Batería e Interfaz de Energía** | Celdas de Ion de Litio encargadas de suministrar voltajes continuos regulados para la movilidad del hardware. | Batería interna integrada no extraíble externamente. |

---

## 3. CUIDADOS Y MEDIDAS DE SEGURIDAD ANTES DE LA PRÁCTICA

El cumplimiento de las siguientes normas previene accidentes personales y daños catastróficos irreversibles en los microcomponentes electrónicos:

*   **Prevención de Descargas Electrostáticas (ESD):** Los circuitos integrados modernos son altamente susceptibles a la electricidad estática generada por el cuerpo humano. Es **obligatorio el uso de la pulsera antiestática**, ajustada firmemente a la muñeca y conectada a la toma de tierra del chasis metálico. 
*   **Aislamiento del Entorno:** La mesa de trabajo debe estar limpia, perfectamente iluminada y construida con materiales **no conductores** (madera, melamina o tapetes antiestáticos; nunca superficies de metal).
*   **Desconexión Eléctrica Absoluta:** Se debe apagar el equipo por completo, retirar el cargador de corriente y remover los cables exteriores antes de iniciar el desarme.
*   **Gestión de Tornillería:** Debido a que las laptops utilizan tornillos de diferentes longitudes en el chasis inferior y en la placa madre, se deben clasificar en recipientes independientes etiquetados con cinta adhesiva. Colocar un tornillo largo en una rosca corta puede perforar las pistas internas de la tarjeta madre.
*   **Regla de No Forzar:** Ningún componente electrónico ni conector debe introducirse a la fuerza. Si una tarjeta o cable no encaja con suavidad, se está insertando en la orientación o ranura incorrecta.

---

## 4. DESARROLLO PASO A PASO DE LA PRÁCTICA (PROTOCOLO INDUSTRIAL)

### Fase 1: Desarmado Seguro del Chasis Inferior
1. Coloque la laptop de cabeza sobre un paño suave para no rayar la cubierta superior.
2. Retire los tornillos visibles de la carcasa inferior con el destornillador de cruz adecuado. *Nota técnica: Verifique si hay tornillos ocultos debajo de las gomas antideslizantes de soporte.*
3. Utilice una púa de plástico de apertura (*spudger*) para separar con cuidado los pines plásticos a lo largo del perímetro del chasis. No use destornilladores planos de metal para hacer palanca, ya que deformarán el plástico o romperán componentes internos.
4. Levante la tapa con cuidado. **Paso crítico inmediato:** Localice el conector de la batería interna y desconéctelo de la placa madre antes de tocar cualquier otro circuito, eliminando la presencia de voltajes residuales en el sistema.

### Fase 2: Limpieza Técnica de la Placa Madre y Memoria RAM
1. Utilice una brocha de cerdas rígidas limpia para remover el polvo superficial adherido a la placa madre, acompañado de una aspiradora para capturar los residuos suspendidos.
2. **Advertencia de Seguridad con el Aire Comprimido:** Al aplicar aire comprimido, mantenga el bote en posición vertical (nunca invertido para evitar expulsar líquido congelado) y sostenga firmemente las aspas del ventilador con un dedo. Si permite que el aire haga girar el ventilador de forma libre, actuará como un dínamo y generará un voltaje inverso que puede quemar los circuitos integrados de la placa madre.
3. Desmonte el módulo de memoria RAM presionando los ganchos metálicos laterales. Sujete la tarjeta estrictamente por sus bordes plásticos para evitar daños por ESD.
4. Si las terminales doradas están sucias, **frótelas firmemente con una goma de lápiz suave**. Retire por completo los residuos de la goma e introduzca el módulo en su ranura aplicando una ligera presión hasta escuchar el chasquido de seguridad.

### Fase 3: Mantenimiento del Sistema Técnico (Procesador Intel Celeron 4205U)
1. Retire los tornillos que fijan el disipador de cobre sobre el procesador siguiendo el orden numérico impreso en el metal (1, 2, 3, 4) para evitar tensiones desiguales sobre el chip.
2. Limpie los restos secos de la pasta térmica antigua sobre el procesador y el bloque de cobre utilizando un lienzo libre de pelusa humedecido con **alcohol isopropílico**. La superficie debe quedar perfectamente brillante y libre de grasa.
3. Aplique una pequeña gota (tamaño de un grano de arroz) de pasta térmica de alta conductividad en el centro del procesador. No sature la superficie; el exceso de pasta actúa como aislante en lugar de conductor técnico.
4. Vuelva a colocar el disipador y ajuste los tornillos en forma de cruz respetando el orden numérico original.

### Fase 4: Reensamblado y Control de Calidad
1. Conecte nuevamente el cable de alimentación de la batería a la tarjeta madre.
2. Verifique la "Ley del Pin 1" o la alineación correcta en cualquier cable flexible (*flex*) que haya sido desconectado (teclado, touchpad, puertos USB laterales).
3. Coloque la tapa inferior del chasis y encaje a presión los pines plásticos del contorno.
4. Atornille la carcasa externa utilizando los tornillos correspondientes previamente organizados.
5. Conecte el cargador y proceda al encendido del equipo para validar el arranque exitoso del sistema y comprobar que las temperaturas del procesador Intel Celeron se mantengan estables en reposo.

---

## 5. CONCLUSIONES Y RECOMENDACIONES DE OPERACIÓN

*   **Periodicidad:** Se recomienda realizar este procedimiento de limpieza interna profunda como mínimo **una vez al año** en entornos domésticos limpios, o cada **seis meses** si la computadora portátil trabaja en ambientes expuestos a altas concentraciones de polvo o fibras textiles.
*   **Software Complementario:** Como complemento al mantenimiento físico, es mandatorio ejecutar las utilerías nativas del sistema operativo para la desfragmentación/optimización del disco sólido (SSD) y la revisión periódica del estado de salud de los bloques de almacenamiento.

---

## 6. REFERENCIAS BIBLIOGRÁFICAS

*   Gutiérrez Molina, A., Peñafiel Salinas, J., & Villarreal Azúa, I. G. (s.f.). *Mantenimiento preventivo y correctivo para PCs*. Dirección General de Servicios de Cómputo Académico, Universidad Nacional Autónoma de México (UNAM).


