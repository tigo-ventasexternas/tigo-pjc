# tigo-pjc

Landing interactiva para captar prospectos de Tigo Paraguay en Pedro Juan Caballero.

Incluye:

- Simulador de planes por zona urbana y rural.
- Internet urbano, TV, combos Internet + TV y TV satelital rural.
- Requisitos visibles antes del envío.
- Botón de WhatsApp a Isidro Cabrera.
- Registro automático de leads en Google Sheets mediante Google Apps Script.
- Diseño móvil para grupos de WhatsApp, Facebook Marketplace y publicaciones en redes.

## Datos configurados

Asesor: Isidro Cabrera  
Rol: Asesor de Ventas Externas Tigo Paraguay autorizado  
WhatsApp: 595984049651  
Correo operativo: tigo.ventasexternas@gmail.com  
Repositorio sugerido: tigo-pjc  

## Archivos

- `index.html`: landing completa para GitHub Pages.
- `apps-script/Code.gs`: código para conectar la landing con Google Sheets.

## Paso 1. Subir a GitHub Pages

1. Entra a GitHub.
2. Abre el repositorio `tigo-pjc`.
3. Sube el archivo `index.html` en la raíz del repositorio.
4. Ve a `Settings`.
5. Entra a `Pages`.
6. En `Build and deployment`, selecciona `Deploy from a branch`.
7. Selecciona rama `main` y carpeta `/root`.
8. Guarda.
9. GitHub te dará una URL similar a:

`https://TU_USUARIO.github.io/tigo-pjc/`

## Paso 2. Crear la hoja de Google Sheets

1. Entra a Google Sheets con el correo operativo.
2. Crea una hoja nueva.
3. Nómbrala: `Leads Tigo PJC`.
4. Ve a `Extensiones`.
5. Entra a `Apps Script`.
6. Borra el contenido inicial.
7. Pega el contenido de `apps-script/Code.gs`.
8. Guarda el proyecto.

## Paso 3. Desplegar Apps Script

1. Dentro de Apps Script, pulsa `Implementar`.
2. Elige `Nueva implementación`.
3. Tipo: `Aplicación web`.
4. Ejecutar como: `Yo`.
5. Quién tiene acceso: `Cualquier usuario`.
6. Pulsa `Implementar`.
7. Autoriza los permisos.
8. Copia la URL que termina en `/exec`.

## Paso 4. Conectar la landing con Google Sheets

1. Abre `index.html`.
2. Busca esta línea:

`appsScriptUrl: "PEGAR_AQUI_TU_URL_DE_APPS_SCRIPT"`

3. Reemplázala por tu URL real de Apps Script:

`appsScriptUrl: "https://script.google.com/macros/s/XXXXXXXX/exec"`

4. Guarda.
5. Sube nuevamente `index.html` al repositorio.

## Paso 5. Probar

1. Abre la URL pública de GitHub Pages.
2. Selecciona un plan.
3. Llena nombre, WhatsApp, barrio y dirección.
4. Marca la confirmación de requisitos.
5. Pulsa `Enviar solicitud y abrir WhatsApp`.
6. Debe pasar esto:

- Se guarda el lead en Google Sheets.
- Se abre WhatsApp con el resumen listo para enviar a Isidro.

## Importante operativo

La landing no promete mes gratis ni promociones por venir de otra compañía. El flujo está armado para venta con pago anticipado de la primera cuota.

El envío automático a WhatsApp sin que el cliente toque enviar requiere WhatsApp Business API o un proveedor externo. Esta versión usa el método correcto para venta rápida sin pagar API: guarda el lead en Sheet y abre WhatsApp con el mensaje armado.

## Copy recomendado para grupos de WhatsApp

```
¿Ya tenés listo internet y TV para ver los partidos?

Soy Isidro Cabrera, Asesor de Ventas Externas Tigo Paraguay autorizado.

Armá tu combo según tu zona:
Internet urbano
TV
Internet + TV
TV satelital para zona rural

Entrá acá, elegí tu plan, revisá requisitos y mandame tu solicitud por WhatsApp:
PEGAR_LINK_DE_GITHUB_PAGES
```

## Título recomendado para Facebook Marketplace

```
Internet y TV Tigo en PJC | Armá tu combo y consultá cobertura
```

## Descripción recomendada para Facebook Marketplace

```
Servicio Tigo Paraguay en Pedro Juan Caballero y alrededores.

Opciones disponibles:
Internet urbano
TV
Internet + TV
TV satelital para zona rural
Planes con fútbol y Tigo Sports según grilla disponible

Requisitos:
Cédula vigente
Ser mayor de edad
Pago anticipado de primera cuota
Validación de cobertura

Soy Isidro Cabrera, Asesor de Ventas Externas Tigo Paraguay autorizado.

Escribime por WhatsApp o armá tu combo aquí:
PEGAR_LINK_DE_GITHUB_PAGES
```
