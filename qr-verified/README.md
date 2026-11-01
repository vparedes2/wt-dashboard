# Verificador de certificados · Vaca Muerta Consulting

- Página pública: https://victorparedes.ar/qr-verified/?c=CODIGO
- Generador interno (no enlazado): https://victorparedes.ar/qr-verified/generar.html
- Ejemplo: https://victorparedes.ar/qr-verified/?c=VMC-DEMO-0001

## Emitir un certificado

1. Abrí `generar.html`, cargá los datos y tocá **Generar código y QR**.
2. Descargá el `.json` y subilo a `qr-verified/c/` (el nombre del archivo es el código, p. ej. `VMC-2026-K7P4QX.json`).
3. Descargá el QR y pegalo en el certificado, con el código escrito debajo.

## Revocar un certificado

Editá su `.json` y cambiá `"estado": "vigente"` por `"estado": "revocado"`.

## Datos que se publican

Nombre, últimos 3 dígitos del DNI, curso, horas, modalidad y fechas. El DNI completo nunca se sube.
Los códigos son aleatorios, para que no se puedan adivinar recorriendo números.
