# Configuración de DNS Master-Slave con Bind9

![Portada del proyecto](cover.png)

## Descripción del Proyecto
Proyecto personal de **Administración de Sistemas** enfocado en la configuración de un servidor DNS autoritativo con Bind9 en arquitectura master-slave para redundancia y alta disponibilidad.

Características principales:
- Zona directa con registros A (servidores, dns-master/slave), CNAME (www, ftp, cloud).
- Zona inversa con registros PTR para resolución reverse.
- Transferencias de zona permitidas entre master y slave (allow-transfer { 10.0.2.6; }).
- Visualización y gestión mediante Administrador de DNS en Windows.
- Pruebas con nslookup para resolución forward (A, CNAME) y reverse (PTR).

Entorno reproducible en red local con IPs 10.0.2.x.

## Tecnologías y Herramientas Utilizadas
- **Bind9** (master y slave)
- **Linux** para edición de archivos (/etc/bind/named.conf.local, db.olive.local, db.10.0.2)
- **Windows DNS Manager** para interfaz gráfica
- **nslookup** para verificaciones

## Objetivos Alcanzados
- Implementación master-slave con sincronización de zonas.
- Registros DNS variados para servicios (web, ftp, cloud).
- Resolución completa forward y reverse.
- Verificación desde múltiples servidores.

## Proceso Completo – Capturas Paso a Paso

<div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(320px, 1fr)); gap: 15px; margin: 30px 0;">

  <img src="screenshots/screenshots (1).png" alt="Paso 1: DNS Manager - Registros zona directa">
  <img src="screenshots/screenshots (2).png" alt="Paso 2: nslookup servidor2 y ftp">
  <img src="screenshots/screenshots (3).png" alt="Paso 3: nano db.10.0.2 (zona inversa)">
  <img src="screenshots/screenshots (4).png" alt="Paso 4: nano db.olive.local (zona directa)">
  <img src="screenshots/screenshots (5).png" alt="Paso 5: nano named.conf.local (zonas inversas)">
  <img src="screenshots/screenshots (6).png" alt="Paso 6: DNS Manager - Zonas inversas">
  <img src="screenshots/screenshots (7).png" alt="Paso 7: nslookup servidor1, www, reverse">
  <img src="screenshots/screenshots (8).png" alt="Paso 8: nano named.conf.local (zonas directas)">
  <img src="screenshots/screenshots (9).png" alt="Paso 9: DNS Manager - Zonas directas">
  <img src="screenshots/screenshots (10).png" alt="Paso 10: nslookup servidor2, ftp, reverse 2">
  <img src="screenshots/screenshots (11).png" alt="Paso 11: DNS Manager - Vista general">

</div>

## Aprendizajes Clave
- **Master-Slave en Bind**: Sincronización y transferencias seguras.
- **Zonas y Registros**: Directas (A, CNAME, NS, SOA), inversas (PTR).
- **Verificaciones**: nslookup para testing forward/reverse.
- Integración Windows-Linux para gestión DNS.

## Relevancia Profesional
Habilidades para:
- Redes empresariales (redundancia DNS).
- DevOps/Cloud (base para DNS gestionados).
- Ciberseguridad (configuraciones seguras).

## Conclusión
Proyecto funcional con DNS redundante, listo para escalar.

¡Gracias por visitar! Dale ⭐ si te gusta.

---
**Autor**: Pau Olivé Moreno  
**Fecha**: Principios de 2025