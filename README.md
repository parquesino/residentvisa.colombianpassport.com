# residentvisacolombia.com — landing de Residente (ES)

Sitio estático en español (traspaso R + R por tiempo acumulado), estética azul propia. Sin build. Deploy = push a `main` → GitHub Pages.

> OJO repo: el remoto se llama **`parquesino/residentvisa.colombianpassport.com.git`** (distinto a la carpeta). Dominio vía `CNAME` (`residentvisa.colombianpassport.com`). La cuenta de deploy necesita acceso concedido a ese repo (pedirlo si el push da 403).

## Objetivos (iguales en todas las landings)

1. Generar leads por WhatsApp.
2. Vender consultas estratégicas de $80 (100% abonables al contratar).
3. Transmitir: (a) contratar un abogado es una decisión inteligente; (b) Camila Ocampo / Colombian Passport es la firma correcta para contratar.

## Estructura

- `index.html` — landing única (Residente $650 primera vez / $450 solo traspaso).
- `eligibility-result.html` — página de resultado del quiz.
- Sin CSS compartido: cada HTML lleva su propio `<style>` inline.

## Modelo de precio vigente (oct-2026)

- Precios oficiales en la web: **$650 USD** R primera vez / **$450 USD** solo traspaso (ex-Protegido / traspaso). Sin nombres de plan (Esencial/Protegido/Integral).
- Esencial (descuento) e Integral ($2.900) solo existen en consulta; ni mención en web.
- Garantía: reaplicaciones por inadmisión sin honorarios hasta la aprobación. Cada nuevo estudio oficial ($56) lo paga el cliente al Estado. No cubre el rechazo definitivo.
- Tabla a 2 columnas (Servicio | Precio fijo). Beneficiario a **$300** (unificado; el ex-Protegido local era $200).
- Tasas con doble vía propia: estudio $56 + traspaso $56 (si ya eres R) o expedición $408 (R primera vez) + cédula $294.000 COP.

## Reglas vigentes (oct-2026)

1. **Cero fugas**: badges a `#reviews` o `<span>` sin link; logo del footer sin enlace; flotante nativo de WhatsApp (verde `#22C55E`) en vez de Chaty (pixel eliminado).
2. **No inventar cifras**: fuentes válidas son la tarjeta Protegido original y lo que pida el dueño.
3. Push a `main` = deploy (si el remoto trae cambios, `pull --rebase` antes del push). Verificar en vivo con hard refresh.
4. No tocar `canonical` ni la sección de costos del gobierno (traspaso vs primera vez).
