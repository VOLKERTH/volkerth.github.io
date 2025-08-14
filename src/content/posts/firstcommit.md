---
title: "First Commit, preparando el entorno"
slug: "color-psychology-branding"
description: "Mi primer post"
publicationDate: 2025-08-14
category: "Proxmox"
public: true
author: "Sergio Muñoz"
---

En esta primera entrada del blog, quiero usarlo para explicar el entorno en el que vamos a trabajar, mi homelab (los detalles del hardware en la pestaña "Homelab"), tengo instalado <b>Proxmox PVE 9.0</b>, recién publicada hace una semana de esta entrada.

Una vez instalado (pasos sencillos, crear el USB bootable con Rufus y seguir el asistente de instalación que es bastante sencillo y pocos pasos), lo primero que hice fue crear un grupo de <i>Administradores</i>, y un rol de permisos para el mismo, para no asignar permisos a usuarios sueltos.

Creo mi usuario en Linux, desde la terminal en el propio nodo

<code class="bash">useradd -m -s/bin/bash sysops</code>

Añado este usuario al grupo <i>Administradores</i>, y habilito MFA en <i>root</i> y <i>sysops</i>.

Otros ajustes que suelo hacer, son dos cambios en cuanto a almacenamiento:
    <ul class="list">
        <li>◦ Usar todo el tamaño del disco del sistema en una misma partición, del datastore <i>local-lvm</i>.</li>
        <li>◦ Asignar funciones a los datastores (que ambos alojen máquinas virtuales, imágenes de disco, contenedores...)</li>
    </ul>

Los pasos para eliminar <i>local-lvm</i> y tener así el disco en una sola partición:
<code class="bash">
<p>lvremove /dev/pve/data</p>
<p>lvresize -l +%100%FREE /dev/pve/root</p>
<p>resize2fs /dev/mapper/pve-root</p>
</code>

Con esto nos aparecerá dos datastores, y uno de ellos con interrogación, podemos borrarlo en <code>Datacenter -> Storage</code>:
<img src="/posts/images/datastores.jpg"/>

Para la segunda acción, desde la misma pantalla que hemos borrado el datastore, seleccionamos el datastore y en la parte <i>Content</i>, seleccionamos los permisos que deseamos.

<b>TIP</b>: En el caso de tener dos discos con la misma capacidad, te recomiendo crear un volumen ZFS, y hacer un RAID con ambos.
Se hace desde el <code>nodo/host -> Disks -> ZFS</code> y seleccionamos la opción que más se adapte a nosotros.