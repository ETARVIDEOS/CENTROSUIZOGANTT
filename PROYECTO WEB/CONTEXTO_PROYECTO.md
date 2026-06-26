# Proyecto: Centro Suizo Joyas — Contexto Completo

> Última actualización: 26 junio 2026
> Preparado por: Krea & Cuenta SpA (Edgar Boyé)

---

## 1. PARTES INVOLUCRADAS

| Rol | Nombre | Contacto |
|---|---|---|
| Cliente | Jordan Bruna Opazo | ipr.jordan@gmail.com |
| Agencia | Krea & Cuenta SpA (Edgar) | kreaycuenta@gmail.com |

---

## 2. NEGOCIO DEL CLIENTE

- **Nombre:** Joyería Centro Suizo / Centro Suizo Joyas
- **Ubicación:** Iquique, Chile
- **Plataforma e-commerce:** Wix (plan gratuito actualmente)
- **URL Wix:** https://admin05151.wixsite.com/website-362
- **Dashboard Wix:** https://manage.wix.com/dashboard/ad8fe733-264e-494e-b3af-2261071556c1/home
- **Dominio a registrar:** joyeriacentrosuizo.cl (en NIC Chile, aún no registrado)
- **Productos en tienda:** 310 productos
- **Colecciones:** AROS DE BEBE, ANILLOS DE COMPROMISO, AROS ADULTO
- **CRM:** SuperSonics ONE — ya activo y logueado

---

## 3. ACCESO A SISTEMAS (CONFIGURACIÓN TÉCNICA)

### Wix
| Elemento | Detalle |
|---|---|
| Navegador | Google Chrome |
| Perfil Chrome | earguello.coapconsultores@gmail.com |
| Cuenta Wix | ipr.jordan@gmail.com (Jordan) |
| Extensión Claude | Instalada y funcional en ese perfil |
| Estado | **FUNCIONA** — Claude puede leer y controlar Wix |

**Nota:** Opera GX NO funciona con la extensión Claude (incompatibilidad Tab Groups API).

### SuperSonics ONE
| Elemento | Detalle |
|---|---|
| URL | https://app.supersonics.one/v2/location/BqC5uMyvdkyqZnX8W2vV/dashboard |
| Location ID | BqC5uMyvdkyqZnX8W2vV |
| Cuenta logueada | Joyería Centro Suizo |
| Acceso Claude | **NO puede navegar via extensión** (dominio bloqueado) — usar screenshots manuales |
| Form 1 existente | ID: Olr0hxVXrWqvv0C88Ykd (creado por Jordan Bruna, Jun 18 2026) |
| API formularios | https://api.supersonics.one/widget/form/{FORM_ID} |
| Script embed | https://api.supersonics.one/js/form_embed.js |

### GitHub + Cloudflare Pages
- Hosting de landing pages: GitHub (repos públicos) + Cloudflare Pages (deploy automático)
- Se eligió Cloudflare Pages sobre Netlify por **sin límite de ancho de banda** (crucial para Meta Ads)
- Ver manual detallado: `manual_cloudflare_pages.txt`

---

## 4. ARCHIVOS DEL PROYECTO

| Archivo | Ubicación | Descripción |
|---|---|---|
| `catalog_products (2).csv` | `C:\Proyectos\CENTROSUIZOJOYAS\` | CSV parcial (~80 de 310 productos, 52 cols Wix) |
| `PLAN JOYERIA CENTRO SUIZO 2.docx` | `C:\Proyectos\CENTROSUIZOJOYAS\` | Propuesta comercial en Word |
| `CONTEXTO_PROYECTO.md` | `C:\Proyectos\CENTROSUIZOJOYAS\` | Este archivo |
| `carta_gantt.html` | `C:\Proyectos\CENTROSUIZOJOYAS\` | Carta Gantt estática (para PDF/cliente) |
| `carta_gantt_interactiva.html` | `C:\Proyectos\CENTROSUIZOJOYAS\` | Carta Gantt interactiva con fechas editables, baseline y comentarios |
| `manual_cloudflare_pages.txt` | `C:\Proyectos\CENTROSUIZOJOYAS\` | Paso a paso para crear landings en Cloudflare Pages |
| `manual_supersonics.txt` | `C:\Proyectos\CENTROSUIZOJOYAS\` | Investigación completa de SuperSonics ONE |

**Para leer el PDF:** Poppler instalado.
`C:\Users\Boye Ingeniería\AppData\Local\Microsoft\WinGet\Packages\oschwartz10612.Poppler_Microsoft.Winget.Source_8wekyb3d8bbwe\poppler-25.07.0\Library\bin\pdftotext.exe`

**Server local:** `npx serve -l 3456 .` en la carpeta del proyecto

---

## 5. PROPUESTA COMERCIAL — FASE 1

**Total:** $945.000 neto (con descuento) / $1.124.550 con IVA
**Pago:** 50% anticipo / 50% contra entrega de entregables operativos

| # | Entregable | Con descuento |
|---|---|---|
| 1 | Levantamiento Wix + Pixel Meta Ads | $150.000 |
| 2 | Dominio joyeriacentrosuizo.cl (NIC Chile) | $30.000 |
| 3 | Guión de ventas emocional WhatsApp | $65.000 |
| 4 | Capacitación online 1 día (máx 4 dispositivos) | $150.000 |
| 5 | Campaña Meta Ads — Argollas matrimonio (~$600K pauta) | $200.000 |
| 6 | Campaña Meta Ads — Anillos de compromiso (~$250K pauta) | $200.000 |
| 7 | Campaña e-commerce — Aros bebé/cadenas (máx 4 productos) | $150.000 |

**Inversión en pauta sugerida:** mínimo $700.000 CLP/mes (pagada directamente por el cliente a Meta).

---

## 6. PLAN DE TRABAJO DETALLADO — FASE 1

### Objetivo Central
Determinar el **Costo de Adquisición de Lead (CAL)** usando la infraestructura web actual. El cliente registrará ventas de productos ofertados por formulario para medir el **ROAS**.

### Fase 1.1 — Quick Win Meta Ads (1 al 15 de Julio)

**Entregables:**
1. Landing page Argollas Matrimonio → GitHub + Cloudflare Pages
2. Landing page Anillos de Compromiso → GitHub + Cloudflare Pages
3. Formularios SuperSonics embed en ambas landings (crear form específico por campaña)
4. Meta Pixel instalado en ambas landings con evento `fbq('track', 'Lead')`
5. Guión emocional de ventas WhatsApp (entrega ~7 Julio)
6. Configuración campañas Meta Ads (segmentación Iquique)
7. Registro automático de leads en SuperSonics CRM

**Hitos:**
- **8 Julio:** Capacitación comercial WhatsApp + Marcador PC (5 horas, máx. 4 dispositivos, NO incluye CRM)
- **8 Julio:** Excel catálogo entregado a Jordan
- **10 Julio:** Feedback Excel recibido de Jordan (plazo límite — Fase 1.2 depende de esto)
- **15 Julio:** Campañas Meta Ads LIVE — Argollas + Anillos

### Fase 1.2 — Levantamiento Wix + Pixel Meta (10 al 30 de Julio)
*Inicio depende del feedback del Excel recibido el 10 de Julio*

**Entregables:**
1. Levantamiento Web Wix + instalación Pixel Meta Ads
2. Registro dominio joyeriacentrosuizo.cl en NIC Chile
3. Actualización catálogo 310 productos (Excel → CSV Wix)
4. Campaña e-commerce Aros Bebé / Cadenas (máx. 4 productos)

**Hito:**
- **30 Julio:** Wix operativo + dominio activo

### Fase 1.3 — Google Ads — BONUS INCLUIDO (30 Julio al 10 Agosto)
*Solo si Wix está operativo al 30 de Julio*

**Entregables:**
1. Configuración Google Ads + palabras clave Iquique
2. Primera campaña Google Ads activa

**Hito:**
- **10 Agosto:** Google Ads activo + Primera revisión de resultados Fase 1

---

## 7. SUPERSONICS ONE — HALLAZGOS CLAVE

### Funcionalidades confirmadas
- ✅ **Formularios embebibles** en páginas externas via iframe + script
- ✅ **Administrador de Anuncios** integrado (Facebook + Google + LinkedIn) — **REQUIERE ACTIVACIÓN**
- ✅ **Automatización / Flujos de trabajo** — ya tiene workflows de Facebook, Instagram, WhatsApp
- ✅ **Planificador redes sociales** — FB y IG conectados (necesitan reconexión)
- ✅ **WhatsApp API** integrado en conversaciones

### Cómo embeber formulario en una landing externa
```html
<div style="height:740px; width:100%">
  <iframe
    src="https://api.supersonics.one/widget/form/FORM_ID_AQUI"
    style="width:100%;height:100%;border:none;border-radius:8px"
    data-layout="{'id':'INLINE'}"
    data-trigger-type="alwaysShow"
    data-activation-type="alwaysActivated"
    data-deactivation-type="neverDeactivate"
    data-form-id="FORM_ID_AQUI"
    title="Nombre del formulario">
  </iframe>
</div>
<script src="https://api.supersonics.one/js/form_embed.js"></script>
```

### Conexión SuperSonics ↔ Meta Ads
- **Opción recomendada:** Activar "Administrador de Anuncios" en Marketing → última pestaña
- **Opción actual (Fase 1):** Landing page + form embed → leads caen al CRM automáticamente
- **Alternativa:** Zapier (Meta Lead Forms → SuperSonics)

### Workflows existentes en la cuenta de Jordan
- "Promocion Mensajes Masivos" — **Published**, 224 inscritos
- "Copy - Promocion Mensajes Masivos Argollas" — **Draft**, 677 inscritos (¡ya hay base de argollas!)

### Acción pendiente en SuperSonics
- [ ] Reconectar Facebook e Instagram (piden reconexión)
- [ ] Crear formulario "Landing Argollas Matrimonio" + copiar embed code
- [ ] Crear formulario "Landing Anillos Compromiso" + copiar embed code
- [ ] Activar "Administrador de Anuncios" (verificar costo adicional)
- [ ] Crear workflows post-lead por campaña
- [ ] Verificar ciudad en config (dice Arica, debería ser Iquique)

---

## 8. COMPROMISOS DEL CLIENTE (JORDAN)

El cliente debe entregar antes de comenzar:
- ✓ Directrices claras sobre contenidos de anuncios y precios
- ✓ Fotografías de catálogo disponibles en Wix
- ✓ Autorización para reutilizar videos e Instagram para pauta
- ✓ Accesos administrativos a todos los sistemas
- ✓ Facilidades para colaboradores en capacitación online
- ✓ **Registro de ventas** de productos ofertados por formulario (para medir ROAS)
- ✓ **Feedback del Excel catálogo antes del viernes 10 de Julio**

---

## 9. ESTADO DE TAREAS

### COMPLETADO ✅
- [x] Propuesta comercial leída y analizada
- [x] Catálogo CSV analizado (52 columnas, formato Wix — NUNCA modificar columnas)
- [x] Acceso Wix confirmado y funcionando via Chrome
- [x] SuperSonics investigado: formularios, embed code, Administrador de Anuncios
- [x] **Carta Gantt estática** creada (`carta_gantt.html`)
- [x] **Carta Gantt interactiva** creada (`carta_gantt_interactiva.html`) — fechas editables, baseline, comentarios, responsive
- [x] **Manual Cloudflare Pages** creado (`manual_cloudflare_pages.txt`) — con embed code real de SuperSonics
- [x] **Manual SuperSonics** creado (`manual_supersonics.txt`) — investigación completa

### PRÓXIMOS PASOS — EJECUCIÓN TÉCNICA (Fase 1.1)

**Semana 1 Julio (1-5 Jul):**
- [ ] Crear repo GitHub: `landing-argollas-matrimonio` (público)
- [ ] Crear repo GitHub: `landing-anillos-compromiso` (público)
- [ ] Crear HTML landing Argollas (copy emocional + Meta Pixel + form embed)
- [ ] Crear HTML landing Anillos (copy emocional + Meta Pixel + form embed)
- [ ] Conectar repos a Cloudflare Pages
- [ ] En SuperSonics: crear formularios específicos por campaña + obtener embed codes
- [ ] Activar Administrador de Anuncios en SuperSonics (verificar costo)

**Semana 2 Julio (5-8 Jul):**
- [ ] Instalar Meta Pixel en ambas landings + verificar con Pixel Helper
- [ ] Conectar formularios SuperSonics en landings
- [ ] Crear guión emocional WhatsApp (entrega 7 Julio)
- [ ] Preparar Excel catálogo para Jordan (entrega 8 Julio)
- [ ] Capacitación comercial WhatsApp (8 Julio, 5 horas, 9:00 AM)

**Semana 2-3 (8-15 Jul):**
- [ ] Configurar campañas Meta Ads (segmentación Iquique)
- [ ] Activar campañas → Live el 15 Julio

**Otras tareas Fase 1.2 (cuando llegue feedback Excel, máx. 10 Jul):**
- [ ] Instalar Pixel Meta en Wix (Marketing → Facebook Ads)
- [ ] Registrar dominio joyeriacentrosuizo.cl en NIC Chile
- [ ] Exportar CSV completo 310 productos desde Wix
- [ ] Actualizar catálogo con precios/fotos del equipo de Jordan

---

## 10. NOTAS TÉCNICAS IMPORTANTES

### CSV de Wix
- **NUNCA modificar las 52 columnas** — Wix rechaza imports con columnas faltantes o renombradas
- Solo editar: `price`, `inventory`, `visible`, `ribbon`, `name`, `description`
- El `handleId` es el identificador único — no tocar jamás

### Carta Gantt Interactiva
- Guardado automático en `localStorage` del navegador
- Función **Línea Base**: guarda fechas actuales, muestra barra fantasma al modificar
- Función **Restaurar**: vuelve a las fechas de la línea base
- Comentarios por hito: añadir, editar, eliminar (persisten en localStorage)
- Para compartir con Jordan: Ctrl+P → Guardar como PDF
- Para desplegar en Netlify: arrastrar el HTML a Netlify Drop o conectar GitHub

### Meta Pixel en Landings
- Obtener Pixel ID desde Meta Business Suite → Administrador de Eventos
- Pegar código en `<head>` del HTML
- Evento de conversión: `fbq('track', 'Lead')` al enviar el formulario

### Wix Plan Gratuito
- Limita funciones de marketing y SEO
- Para Meta Pixel avanzado puede necesitar plan de pago
- Dominio personalizado requiere plan de pago en Wix

---

## 11. FASES FUTURAS (no incluidas en propuesta actual)

### Fase 2
- Auditoría y migración CRM
- Campañas Google + Meta combinadas
- Capacitación CRM online 2 días

### Fase 3
- Agente de voz IA para leads automáticos
- Claude conectado a Meta Ads y Google Ads
- Dashboard datos en tiempo real desde CRM

### Fase 4
- Replicar modelo a otros negocios de Jordan

---

## 12. CÓMO USAR ESTE CONTEXTO EN UNA NUEVA CONVERSACIÓN

Al abrir una nueva conversación con Claude, comparte este archivo y di:

> "Lee el archivo CONTEXTO_PROYECTO.md y retoma el proyecto de Centro Suizo Joyas desde donde lo dejamos."

Claude tendrá todo el contexto para continuar sin repetir pasos.

**Archivos clave a mencionar si necesitas trabajar en algo específico:**
- Gantt interactivo: `carta_gantt_interactiva.html`
- Manual Cloudflare: `manual_cloudflare_pages.txt`
- Manual SuperSonics: `manual_supersonics.txt`
- Catálogo CSV: `catalog_products (2).csv`
