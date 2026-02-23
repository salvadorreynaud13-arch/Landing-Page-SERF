# **Identidad Visual y Guía de Estilos**

Para transmitir un aura de "Estrategia del Futuro" (IA, automatización, alto rendimiento), la marca se apoya en una estética "Dark Mode" elegante. Los tonos azules denotan profesionalismo y estructura, mientras que los toques de morado eléctrico aportan innovación y flujo (flow).

**Tipografía (Google Fonts)**

* **Títulos (Headings):** Plus Jakarta Sans. Geométrica, moderna, transmite tecnología y vanguardia.  
* **Cuerpo (Body):** Inter. Limpia, máxima legibilidad en interfaces digitales y altamente profesional.

**Variables CSS Base (:root)**

Puedes entregar este fragmento directamente al desarrollador o a la herramienta de generación para asegurar la consistencia visual:

:root {  
  /\* \=========================================  
     PALETA DE COLORES \- TEMA OSCURO (Default)  
     \========================================= \*/  
    
  /\* Fondos (Azules extremadamente oscuros, casi negros) \*/  
  \--bg-main: \#0B0F19;      /\* Fondo principal de la web \*/  
  \--bg-surface: \#111827;   /\* Fondo para tarjetas (cards) y secciones destacadas \*/  
  \--bg-surface-elevated: \#1F2937; /\* Efectos hover y elementos flotantes \*/

  /\* Colores de Marca Principales (Azul y Morado) \*/  
  \--brand-blue-primary: \#2563EB;   /\* Azul fuerte corporativo (Botones principales) \*/  
  \--brand-blue-glow: \#3B82F6;      /\* Azul brillante para efectos hover o bordes \*/  
    
  \--brand-purple-accent: \#7C3AED;  /\* Morado IA/Flow (Detalles, iconos, subrayados) \*/  
  \--brand-purple-glow: \#8B5CF6;    /\* Morado brillante (Glow effects o gradientes) \*/

  /\* Gradiente Oficial SERF (Para textos destacados o fondos de botones premium) \*/  
  \--brand-gradient: linear-gradient(135deg, \#2563EB 0%, \#7C3AED 100%);

  /\* Texto y Tipografía \*/  
  \--text-primary: \#F8FAFC;    /\* Blanco casi puro para títulos (H1, H2, H3) \*/  
  \--text-secondary: \#94A3B8;  /\* Gris azulado para párrafos y subtítulos \*/  
  \--text-muted: \#64748B;      /\* Textos legales o menos importantes \*/

  /\* \=========================================  
     TIPOGRAFÍA  
     \========================================= \*/  
  \--font-heading: 'Plus Jakarta Sans', system-ui, sans-serif;  
  \--font-body: 'Inter', system-ui, sans-serif;

  /\* \=========================================  
     ESPACIADO Y BORDES (Estilo CorosDev)  
     \========================================= \*/  
  \--border-radius-sm: 0.375rem; /\* Botones pequeños, inputs \*/  
  \--border-radius-md: 0.75rem;  /\* Tarjetas (Cards) de servicios \*/  
  \--border-radius-lg: 1.5rem;   /\* Contenedores grandes \*/  
    
  \--border-subtle: 1px solid rgba(255, 255, 255, 0.05); /\* Bordes casi invisibles para separar secciones \*/  
}

/\* Ejemplo de aplicación para botones \*/  
.btn-primary {  
  background: var(--brand-gradient);  
  color: var(--text-primary);  
  font-family: var(--font-heading);  
  font-weight: 600;  
  border-radius: var(--border-radius-sm);  
  transition: all 0.3s ease;  
  box-shadow: 0 4px 14px 0 rgba(124, 58, 237, 0.39);  
}

.btn-primary:hover {  
  box-shadow: 0 6px 20px rgba(124, 58, 237, 0.6);  
  transform: translateY(-2px);  
}  
