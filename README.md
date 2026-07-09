# Landing Page — ICONIC Beauty Salon & Clinic

Informe de briefing para el desarrollador. Este documento reúne toda la información del negocio disponible y las directrices de diseño/desarrollo para construir la landing page. El desarrollador trabajará iterando con Claude a partir de una plantilla base en HTML que ya tiene por su cuenta (esa plantilla **no forma parte de este repositorio**); este README es el contexto de negocio y de producto que debe alimentar esa iteración.

---

## 1. Sobre el negocio

| Campo | Dato |
|---|---|
| **Nombre** | ICONIC Beauty Salon & Clinic |
| **Tagline / subtítulo de marca** | *Hair & Aesthetic Medicine* |
| **Categoría** | Salón de belleza + clínica de medicina estética (servicio completo: peluquería, estética facial/corporal y medicina estética) |
| **Ubicación** | Av. Munich 1911, Col. Jaripillo, Mazatlán, Sinaloa — Plaza Punto Munich, Local 37 |
| **Ciudad** | Mazatlán, Sinaloa, México |
| **Teléfono / WhatsApp** | +52 669 146 1126 |
| **Facebook** | https://www.facebook.com/profile.php?id=61590505378176 |
| **Instagram** | https://www.instagram.com/iconic_beauty_salon_and_spa |

## 2. Catálogo de servicios

Extraído directamente del material de marca del cliente (tarjeta digital). Usar esto como base para las secciones de servicios de la landing:

- **Corte de cabello profesional.**
- **Peinado de novias, quinceañeras y eventos sociales** — brushing, técnicas de secado (blower), alaciado, ondas, peinados de noche, alta peluquería, recogidos.
- **Colocación de extensiones** de cabello natural y clon — técnicas Tape/Adhesivas, Micro Ring/Nano Ring, Queratina (K-Tip), Cortinas/Weft (coser).
- **Tratamientos capilares** — hidratación, nutrición, reconstrucción.
- **Alaciados progresivos y termoactivos** — keratina, bótox capilar, plástica capilar/taninoplastia, células madre, japonés, americano, brasileño, nanoplastia, ácido hialurónico capilar.
- **Aplicación de tintes** — globales, retoque de raíz, cobertura de canas rebeldes, baños de color.
- **Efectos de luz y decoloración** — Balayage, Ombré, Babylights, mechas tradicionales, money piece, decoloraciones globales.
- **Maquillaje profesional** — novias, quinceañeras, fotografía y eventos día/noche, con técnica de visagismo (contouring e iluminación).
- **Manicura y pedicura spa** — esmaltado gelish, uñas acrílicas, nail art.
- **Depilación facial y corporal** — diseño y depilación de cejas, bozo y cuerpo (cera fría/caliente, epilación con roll-on).
- **Limpiezas faciales** — mascarillas y masajes relajantes.
- **Aplicación de botox y ácido hialurónico.**
- **Dermaplaning, peeling y dermapen** (facial, corporal, capilar), mesobotox, BB Glow, hidralips, hilos y velos de colágeno.

Esto posiciona a ICONIC como un negocio **premium de doble vertical**: peluquería de alto nivel + medicina estética. El copy y el diseño deben reflejar ambas cosas con la misma seriedad (no solo "salón de belleza" genérico).

---

## 3. Branding

### Logo
El logo actual es un monograma dorado con las iniciales **"ISC"** (Iconic Salon & Clinic) integrado con la silueta del perfil de un rostro femenino, en estilo elegante/caligráfico, sobre fondo crema.

- **El archivo de logo entregado tiene fondo** (no es transparente) → el desarrollador debe **quitarle el fondo** (remover el fondo crema/beige y dejarlo en PNG transparente) antes de usarlo en el header, favicon, loading screen, etc.
- Se recomienda regenerar/vectorizar si es necesario para que luzca nítido en distintos tamaños (favicon, spinner de carga, footer).

### Paleta de colores
Extraída visualmente del material de marca (tarjeta digital). Son aproximaciones — el desarrollador puede afinar tonos exactos con Claude durante la iteración:

| Uso | Color aproximado | Hex ref. |
|---|---|---|
| Fondo principal / crema | Beige-crema cálido | `#F3E9DC` |
| Dorado/bronce (acento de marca) | Dorado metálico | `#C6A664` |
| Dorado oscuro (detalles/bordes) | Bronce | `#B08D57` |
| Texto principal | Café oscuro / espresso | `#4A3728` |
| Fondo de tarjetas/secciones | Blanco cálido | `#FFFDF9` |

Paleta general: **crema + dorado + café oscuro**, sensación de spa de lujo, cálida pero sobria. Evitar colores saturados o "juveniles"; mantener la sofisticación del material original.

### Tipografía sugerida
- Encabezados: serif elegante (tipo la usada en "ICONIC" del logo) o una serif moderna tipo *Playfair Display*, *Cormorant*, o similar.
- Cuerpo de texto: sans-serif limpia y legible (tipo *Inter*, *Poppins* o *Montserrat*) para mantener el lado "high-tech/corporativo" sin perder calidez.

---

## 4. Dirección al desarrollador — estilo y flujo de trabajo

### Flujo de trabajo
- Ya tienes un **prompt inicial** para adaptar la plantilla base HTML a las necesidades de este negocio. Usa este README como el contexto de negocio/producto para ese prompt.
- **Puedes iterar libremente con Claude** dándole instrucciones sucesivas hasta lograr el resultado deseado — no es un proceso de una sola pasada. Ajusta, corrige y refina tantas veces como sea necesario (contenido, estilo, animaciones, responsive, performance, etc.) hasta que el resultado cumpla con todo lo especificado aquí.
- La plantilla base que vas a modificar la tienes tú por tu cuenta; no está incluida en este repositorio.

### Estilo visual (obligatorio)
El diseño debe sentirse **premium, corporativo, "high-tech" y minimalista a la vez** — nivel enterprise/marca de lujo, no un salón de belleza genérico. Referencias de tono: sitios de clínicas estéticas de alta gama, marcas de lujo, fintech premium. Limpio, con mucho espacio en blanco, tipografía cuidada y la paleta crema/dorado/café descrita arriba.

### Efectos y animaciones requeridos
1. **Pantalla de carga (loading screen)**: spinner de carga con el logo de ICONIC en el centro, antes de mostrar el contenido de la página.
2. **Animaciones on-scroll**: elementos que aparecen/se revelan (fade-in, slide-up, etc.) conforme el usuario baja por la página.
3. **Efectos en el título del Hero**:
   - Efecto tipo "máquina de escribir" (typewriter) en el texto principal del hero.
   - Efecto de cambio de color en las letras del título (animación de color, gradiente animado o similar) para reforzar la sensación premium/dinámica.
4. Mantener los efectos sutiles y fluidos — el objetivo es transmitir sofisticación, no saturar la página con animaciones excesivas.

### Assets
- Quitar el fondo del logo entregado antes de usarlo (ver sección Branding).
- Usar el logo resultante (transparente) en: header/navbar, favicon, pantalla de carga.

---

## 5. Checklist de entregables

- [ ] Fondo del logo removido (PNG transparente)
- [ ] Paleta de colores aplicada de forma consistente (crema / dorado / café)
- [ ] Loading screen con spinner + logo
- [ ] Animaciones on-scroll implementadas
- [ ] Hero con efecto typewriter + cambio de color en el título
- [ ] Sección de servicios con el catálogo completo (sección 2)
- [ ] Datos de contacto y ubicación correctos (dirección, teléfono/WhatsApp, Facebook e Instagram confirmados)
- [ ] Diseño responsive (mobile-first, ya que gran parte del tráfico de un negocio local vendrá de celular)
- [ ] Revisión final del estilo: ¿se siente premium/corporativo/high-tech/minimalista, o se ve genérico?
