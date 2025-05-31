# Funciones-HASH
#### Actividad de Laboratorio: Cálculo y verificación de funciones HASH
## Objetivo: 
Comprender el funcionamiento de las funciones HASH mediante la generación y comparación de valores HASH usando herramientas de línea de comandos en Kali Linux y herramientas online.

## 📋Requisitos
- Kali Linux (virtual o físico)
- Conexión a internet
- Navegador web
- Archivo de texto simple (.txt) para pruebas

## ☑Actividades a realizar en el Laboratorio
### Parte 1: Generación de HASH en Kali Linux
Paso 1: Crear un archivo de prueba

`echo "Hola mundo desde ciberseguridad" > mensaje.txt`

Paso 2: Calcular el HASH usando diferentes algoritmos

a. MD5

`md5sum mensaje.txt`

b. SHA-1

`sha1sum mensaje.txt`

c. SHA-256

`sha256sum mensaje.txt`

¿Qué observas respecto a la longitud y formato de los valores HASH?

Paso 3: Simular una modificación y volver a calcular el HASH

`echo " " >> mensaje.txt`

Repite los comandos anteriores y compara los resultados.

### Parte 2: Uso de herramientas online

Paso 4: Ir a una herramienta de cálculo HASH online

Puedes usar:
*https://emn178.github.io/online-tools/*

Paso 5: Sube el archivo a la plataforma y genera el HASH

- Elije el algoritmo para generar el HASH
![image](https://github.com/user-attachments/assets/68fb3eb2-c2c3-4764-9510-fe07c12ee5b5)

- Luego sube el archivo y genera el HASH
- Compara con los resultados de la terminal de Kali.
- Verifica si los valores HASH coinciden.

### Parte 3: Verificación de integridad

Paso 6: Descargar un archivo desde internet con checksum

Por ejemplo, puedes descargar un archivo de prueba desde:

`wget https://ash-speed.hetzner.com/100MB.bin`

Una ves descargado, subelo al portal indicado en el paso anterior y obten el HASH

Supón que el valor esperado de SHA-256 fuera:

`29c1b58304c8a9064b747e3f313304a75b88fbebfedafb3275006367fe202df8`

Verifica el valor, revisando en la linea de comando en Kali:

`sha256sum 100MB.bin`

¿El valor HASH coincide? ¿Qué significaría si no coincidiera?

## Cierre y reflexión

- ¿Qué aprendiste sobre la sensibilidad de las funciones HASH?
- ¿Por qué son fundamentales para verificar integridad en ciberseguridad?

