# Verificador de certificados · Vaca Muerta Consulting

- Página pública: https://victorparedes.ar/qr-verified/?c=CODIGO
- ABM interno (no enlazado, con clave): https://victorparedes.ar/qr-verified/generar.html
- Ejemplo: https://victorparedes.ar/qr-verified/?c=VMC-DEMO-0001

## Dónde están los datos

En la planilla **VMC · Certificados** de Google Drive. Una aplicación web de Apps Script
(el código se instala desde la planilla: Extensiones → Apps Script) hace de API:

- `GET ?codigo=…` devuelve los datos públicos de un certificado (el DNI solo con sus 3 últimos dígitos).
- `POST` con la clave permite listar, dar de alta, modificar, revocar, reactivar y eliminar.

La URL de esa aplicación (termina en `/exec`) va en `config.js`.
Los archivos de `c/` siguen funcionando como respaldo (por ejemplo, el certificado de demostración).

## Firma

La imagen de la firma se carga en el ABM y queda guardada solo en ese navegador. No se sube al repositorio ni a Drive.
