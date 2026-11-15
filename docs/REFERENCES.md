# Referencias · Pasillo Seguro

Documentación externa que se usó para entender el hardware, los protocolos y las
libertades del proyecto. No es una bibliografía decorativa: cada enlace apunta a
la fuente que explica una decisión concreta.

## Fuentes técnicas

| Fuente | Para qué se consultó |
|---|---|
| [Arduino UNO Q](https://docs.arduino.cc/hardware/uno-q/) | Hardware, Linux y microcontroller de la UNO Q. |
| [IP Webcam](https://play.google.com/store/apps/details?id=com.pas.webcam) | App Android que publica la cámara como MJPEG y JPEG por HTTP. |
| [libjpeg / libjpeg-turbo](https://libjpeg-turbo.org/) | Decodificación JPEG en C, usada para leer el stream de la cámara. |
| [Python 3](https://docs.python.org/3/) | Lenguaje, librería estándar y venv. |

## Versiones de este repositorio

`pasillo-seguro-unoq`

Cada carpeta puede tener dependencias y versiones distintas. Cuando el código
depende de una versión específica, esa versión está declarada en el README o en
el archivo de configuración de la carpeta, no en este documento.

## Criterio de preservación

- El código y los documentos se copiaron desde la carpeta original de trabajo.
- Se excluyeron `.git`, dependencias instaladas, compilados, registros y bases
  de datos locales.
- Se redactaron tokens, claves privadas y contraseñas detectadas en texto.
- Las plantillas `.example`, `.sample` y los valores de demostración se
  conservan porque documentan la configuración esperada.

## Limitaciones conocidas

Un detector en Python resuelve el problema, pero en una placa con poca CPU cada milisegundo cuenta y el intérprete se lleva una parte del presupuesto.

La documentación de cada versión describe el alcance real. Si una función no
está implementada, se dice; si un hardware no fue probado, también.
