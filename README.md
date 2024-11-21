# Proyecto-sobre-la-carretera-Tecomán-Cerro-de-Ortega
El conteo de baches totales sobre esta carretera y el como esto afecta a toda la comunidad
# Título del Proyecto
**Autores:**
Gómez Padilla Artemio Gabriel
y Magaña Anguiano Rocío Maribel

## Introducción
La carretera que conecta Cerro de Ortega con Tecomán constituye una vía esencial para la movilidad y el desarrollo socioeconómico de la región. Sin embargo, su actual estado de deterioro representa un grave desafío para la seguridad vial, la eficiencia del tránsito y la calidad de vida de los habitantes. Este tramo es utilizado diariamente por un volumen significativo de conductores, incluidos agricultores, transportistas y personas que dependen de él para sus actividades económicas, educativas y sociales. El deterioro de la vía, caracterizado por la presencia de baches profundos, fisuras y una deficiente señalización, ha generado numerosos accidentes, volcaduras y daños considerables a vehículos, afectando a particulares y sectores estratégicos como el transporte de productos agrícolas hacia mercados regionales y nacionales.  Frente a esta problemática, el proyecto tiene como objetivo principal la rehabilitación integral de esta carretera para garantizar la seguridad de los ciudadanos, mejorar el flujo vehicular y contribuir al desarrollo económico de la región. Las acciones propuestas incluyen la identificación y reparación de baches, la optimización del drenaje para prevenir acumulaciones de agua durante lluvias, y la mejora de la señalización vial para reducir accidentes. Además, se propone incorporar materiales sostenibles y técnicas innovadoras de construcción que no solo reduzcan costos, sino que también minimicen el impacto ambiental. 
El impacto positivo de este proyecto es amplio y tangible. Por un lado, mejorar la infraestructura vial reducirá significativamente los accidentes de tránsito, protegerá los vehículos de daños costosos y mejorará la experiencia de los conductores. Por otro lado, al optimizar esta vía estratégica, se fortalecerá la economía regional, permitiendo un transporte más eficiente de bienes agrícolas y comerciales, y potenciando la productividad de las comunidades circundantes. A largo plazo, la renovación de la carretera sentará las bases para un desarrollo sostenible, incrementando la conectividad y calidad de vida de miles de personas que dependen de esta vía diariamente.La necesidad de intervenir de manera urgente no solo responde a los crecientes reclamos de la población, que ha recurrido a manifestaciones y bloqueos en señal de protesta, sino también a la importancia estratégica de esta carretera para la actividad comercial e industrial de la región. Ignorar esta situación podría no solo aumentar la frecuencia de accidentes y el desgaste de los vehículos, sino también agravar los problemas de movilidad y afectar directamente la competitividad económica de la región.
En resumen, este proyecto de rehabilitación representa una oportunidad clave para transformar una vía en un motor de desarrollo. A través de una planificación detallada, la participación de la comunidad y la implementación de soluciones innovadoras, se busca no solo reparar una carretera, sino también fortalecer los cimientos del progreso económico y social de una región que depende profundamente de su infraestructura vial.


## Desarrollo
Explicación detallada del enfoque del proyecto, herramientas utilizadas y metodología.

## Manejo de Datos
![image](https://github.com/user-attachments/assets/46f1f3dc-a5c6-491b-9e1a-b486cc9f0dd6)
![image](https://github.com/user-attachments/assets/da302f57-9857-4417-afe9-e9d67f101a5d)

## Resultados
**CÓDIGOS USADOS**
# PRIMER CÓDIGO
#Código para calcular la fuerza en la carretera y prevenir baches
import numpy as np
#Parámetros del material de la carretera
modulo_elasticidad = 3e9  #en Pascales (ejemplo: asfalto)
espesor_carretera = 0.15  #en metros
limite_tension = 2.5e6    #tensión máxima permitida en Pascales (ejemplo)
#Parámetros de la carga
carga_aplicada = 10000    #en Newtons (peso del vehículo, por ejemplo)
area_contacto = 0.01      #en metros cuadrados (área de contacto de la rueda)
#Calcular presión en el área de contacto
presion_contacto = carga_aplicada / area_contacto  # en Pascales
#Calcular tensión en la carretera (simulación simplificada usando esfuerzo máximo)
tension_generada = presion_contacto * espesor_carretera / modulo_elasticidad
#Comparar con el límite de tensión
if tension_generada < limite_tension:
    print("La carretera soporta la carga sin generar baches.")
else:
    print("El material de la carretera está sometido a demasiada tensión. Se podrían generar baches.")
#Imprimir los resultados
print(f"Tensión generada: {tension_generada:.2e} Pa")
print(f"Límite de tensión: {limite_tension:.2e} Pa")

# SEGUNDO CÓDIGO
#Parámetros iniciales
costo_reparacion_por_bache = 1164  #Costo de reparar un bache (en dólares)
cantidad_baches = 100             #Cantidad total de baches en la carretera
presupuesto_total = 20000        #Presupuesto disponible (en dólares)
#Calcular el costo total de reparación
costo_total_reparacion = cantidad_baches * costo_reparacion_por_bache
#Comparar con el presupuesto disponible
if costo_total_reparacion <= presupuesto_total:
    sobrante = presupuesto_total - costo_total_reparacion
    print("El presupuesto es suficiente para reparar todos los baches.")
    print(f"Dinero sobrante después de las reparaciones: ${sobrante:.2f}")
else:
    print("El presupuesto no es suficiente para reparar todos los baches.")
    baches_reparables = presupuesto_total // costo_reparacion_por_bache
    print(f"Se pueden reparar aproximadamente {baches_reparables:.0f} baches con el presupuesto actual.")
#Imprimir resultados
print(f"Costo total de reparación: ${costo_total_reparacion:.2f}")
print(f"Presupuesto disponible: ${presupuesto_total:.2f}")

## Conclusiones
La carretera Cerro de Ortega - Tecomán desempeña un papel crucial en la conectividad y el desarrollo económico de la región, pero su deterioro actual representa un desafío significativo para la seguridad vial y la eficiencia del tránsito. Este proyecto tiene como meta abordar de manera integral los problemas detectados, como los baches, la falta de señalización adecuada y las deficiencias en el drenaje. A través de estrategias de planificación eficiente, el uso de materiales sostenibles y la participación activa de las comunidades afectadas, se busca no solo reparar la infraestructura existente, sino también sentar las bases para un desarrollo vial sostenible a largo plazo.
La implementación de este plan contribuirá directamente a mejorar la calidad de vida de los habitantes al reducir accidentes, facilitar el transporte de mercancías y promover una movilidad más segura y fluida. Además, al priorizar la inversión en infraestructura vial, se fortalecerá la economía regional, garantizando que la carretera sea una herramienta clave para el progreso local. Este proyecto destaca la importancia de una gestión eficiente de recursos, la colaboración entre actores gubernamentales y ciudadanos, y la adopción de soluciones innovadoras que aseguren el éxito del proyecto y sus beneficios a largo plazo.
