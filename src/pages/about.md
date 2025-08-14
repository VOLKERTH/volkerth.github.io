---
layout: ../layouts/PageLayout.astro
title: "Acerca de mí"
description: "Acerca de mí"
---

# Acerca de mí

---

Actualmente trabajo Administrador de sistemas dando soporte a nivel nacional de manera remota, dando soporte a compañeros y también haciendo de mentor. Llevo 11 años trabajando en el sector IT, desde microinformática, pasando por infraestructura on-premise, hasta entornos en nube y contenedores.

## Tecnologías que actualmente uso

Te clasifico por categorías las tecnologías, marcas que usamos en el día a día y acciones que llevamos a cabo:

<section id="Virtualización">
        <h2 class="solway-regular">Virtualización</h2>
          <ul class="pill-list">
              <li>VMware ESXi</li>
              <li>VMware vCenter</li>
              <li>Hyper-V (la solución que más se está vendiendo actualmente en la empresa actual)</li>
              <li>Proxmox (hay un cliente que está empezando con esta tecnología)</li>
          </ul>
        </section>


<section id="Ciberseguridad">
        <h2 class="solway-regular">Ciberseguridad</h2>
          <ul class="pill-list">
              <li>En su mayoría son acciones relacionadas con BlueTeam, y tareas que se repiten en cada sección de esta lista</li>
              <li>Despliegue e instalación de antivirus y automatización (Crowdstrike, Kaspersky, Sophos, ESET... )</li>
              <li>Configuración políticas EDR/XDR</li>
              <li>Analizar logs y configuración de los firewalls (conexiones activas, protocolos...)</li>
              <li>Análisis de los equipos afectados realizando tareas forenses (puertos en escucha, software instalado, ficheros sospechosos)</li>
              <li>Reporte incidente en colaboración con el equipo de cibeseguridad que realizaron previo análisis y auditoría (RedTeam en su mayoría el departamento)</li>
              <li>Aplicar políticas MFA, en su mayoría Azure</li>
          </ul>
        </section>


<section id="Cloud">
        <h2 class="solway-regular">Cloud</h2>
          <ul class="pill-list">
              <li>Azure (Entra ID, Entra Connect, Defender XDR, Purview, VPN, Office365, ...)</li>
              <li>AWS (Disaster Recovery con Veeam, EC2, S3)</li>
          </ul>
        </section>


<section id="Networking">
        <h2 class="solway-regular">Networking</h2>
          <ul class="pill-list">
              <li>Azure VNet</li> 
              <li>AWS VPC</li>
              <li>Fortinet</li>
              <li>Sophos</li>
              <li>SonicWall</li>
              <li>HPE Aruba</li>
              <li>VMware NSX</li>
              <li>CISCO</li>
              <li>Cyberoam</li>
          </ul>
        </section>


<section id="VDI">
        <h2 class="solway-regular">VDI (Infraestructura de escritorios virtuales)</h2>
          <ul class="pill-list">
              <li>VMware Horizon</li>
              <li>Citrix</li>
          </ul>
        </section>


<section id="Almacenamiento">
        <h2 class="solway-regular">Almacenamiento</h2>
          <ul class="pill-list">
              <li>Blob Storage</li>
              <li>AWS S3</li> 
              <li>NAS (Synology, QNAP)</li> 
              <li>HPE MSA</li>
              <li>HPE VSA</li>
              <li>HPE Nimble</li>
              <li>HPE StoreOnce</li>
              <li>TrueNAS</li>
              <li>OwnCloud</li>
          </ul>
        </section>


<section id="Backup">
        <h2 class="solway-regular">Copias de seguridad / Backup</h2>
          <ul class="pill-list">
              <li>Veeam Backup and restore</li>
              <li>Veeam VSPC</li>
              <li>Cobian</li>
              <li>Veeam VSPC</li>
          </ul>
        </section>



## Detrás de las cámaras (¡digo pantalla!)

Fuera de mi trabajo, tengo las siguiente aficiones:
- Me sigo formando en este mundillo y cacharreando con mi servidor ("homelab").
- Cuando se puede, me gusta  jugar a rol y a juegos de mesa.
- Apasionado del mundo de las motos.
- Y si no lo has deducido por mi avatar, también me gusta ver de vez en cuando anime.

## Contacta conmigo

Si quieres que participe o que montemos un proyecto, aunque no tenga conocimiento de ello tanto tú como yo, encantado de unirme y crear comunidad, pero la idea es descubrir nuevas metodologías, buenas prácticas, tecnologías, dialogar acerca de este mundillo, contáctame con plena confianza.
En la página principal tienes las distintas formas en las que puedes contactar conmigo.

  <style>
    .card {
      padding: 1rem;
      background: var(--color-card);
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(var(--color-border), 0.33);
      text-decoration: none;
      color: inherit;
      transition: transform 0.2s ease;
    }
    .card:hover {
      transform: translateY(-3px);
    }
    .card h3 {
      margin: 0;
    }
    .card:hover h3 {
      color: var(--color-link);
    }
    .card p {
      margin: 0.5rem 0 0;
    }

    .finds-box {
        padding: 1em;
    }

    .posts-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
        gap: 1rem;
        margin: 2rem 0;
    }

    /* ===== Hero Section ===== */
    #hero {
      padding-bottom: 1.5rem; 
      padding-top: 2rem; 
    }
    #hero .subtitle {
      margin: 0.5rem; 
      font-size: var(--step-1);
      line-height: 1.25rem; 
    }
    #hero-title {
      display: flex; 
      gap: 1rem; 
      align-items: center;  
    }
    #hero h1 {
      display: inline-block; 
      margin: 0; 
      font-size: var(--step-4);
      line-height: 2.25rem; 
      font-weight: 700; 

    }
    #hero img {
      border-radius: 9999px; 
      border: 4px solid var(--color-button-border); 
      width: 8rem; 
      height: 8rem;
    }

    #hero p {
      margin-top: 1rem;
      margin-bottom: 1rem; 
    }
    
    #action-links {
        display: flex; 
        margin: 0.25rem; 
        flex-wrap: wrap; 
        list-style-type: none
    }

    #action-links li a {
      display: block; 
      padding: 0.25rem; 
      margin-right: 0.5rem; 
      font-weight: 700; 
      border-color: var(--color-border);
    }

    .pill-list {
      display: flex; 
      margin-top: 2rem; 
      flex-wrap: wrap; 
      list-style-type: none
    }

    .pill-list li {
      padding: 0.25rem; 
      margin: 0.5rem; 
      border-radius: 0.25rem; 
      border: 1px solid var(--color-button-border); 
      font-size: var(--step--1);
      line-height: 1.25rem;
    }

    /* ===== Featured & Recent Posts Sections ===== */
   section {
      padding-bottom: 1.5rem; 
      padding-top: 1.5rem; 
    }

    section h2 {
      font-size: var(--step-2);
      line-height: 1rem; 
      font-weight: 600; 
      letter-spacing: 0.025em; 
    }
    .all-posts-btn-wrapper { 
      text-align: center; 
    }
  </style>