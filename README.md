# LocApp v3

Aplicación de cliente (static) para generar contraseñas basadas en una frase. La versión `index_v3.html` incluye varias formas de generar contraseñas (v1 MD5, v2 SHA512 15 caracteres, v3 SHA512+PBKDF2 20 caracteres) y funciona 100% offline — sin almacenamiento.

## Archivos importantes
- `index_v3.html` — Interfaz principal (HTML + estilos + JS embebido).  
- `sha512.js` — Implementación / helper SHA-512 (referenciado por `index_v3.html`).
- `md5.js` — Implementación / helper MD5 (referenciado por `index_v3.html`).

## ¿Qué hay de nuevo?
- La tarjeta principal ahora usa un contenedor fluido y un ancho mayor para aprovechar más espacio horizontal (más parecido a la versión anterior del diseño). Esto aplica estilos CSS para una mejor visualización en pantallas grandes.

## Uso / pruebas rápidas
Puedes abrir `index_v3.html` directamente en el navegador o ejecutar un servidor local si quieres probarlo vía `http://localhost`.

## Notas de privacidad
La app se ejecuta íntegramente en el cliente (navegador). No envía ni almacena datos en servidores externos.

## Ideas / mejoras futuras
- Proveer una interfaz para configurar longitudes y combinaciones (más control sobre v2/v3).
- Añadir test unitarios para los métodos de hash y conversiones (si se separa el JS en módulos).
