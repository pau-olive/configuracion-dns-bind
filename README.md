# Configuración de Servidor DNS con Bind

![Portada del proyecto](cover.png)

## Descripción del Proyecto
Proyecto personal de **Administración de Sistemas** enfocado en la configuración de un servidor DNS utilizando Bind en entornos Linux, incluyendo zonas directas e inversas, registros A, CNAME, PTR y comprobaciones con nslookup. Se incluye también la clonación de equipos para replicar el setup en múltiples máquinas virtuales.

Se implementan escenarios reales:
1. **Configuración básica de Bind**: Creación de archivos de zona y configuración local.
2. **Comprobaciones y resolución**: Verificación de registros DNS con herramientas como nslookup.
3. **Clonación opcional**: Replicación del servidor DNS mediante Clonezilla para despliegue masivo.

Todo en un entorno virtualizado con VirtualBox, reproducible y escalable.

## Tecnologías y Herramientas Utilizadas
- **Bind9** como servidor DNS
- **Linux** (Ubuntu o similar) para el servidor
- **VirtualBox** para virtualización
- **Clonezilla** para clonación de imágenes (opcional)
- Herramientas de verificación: nslookup, dig

## Objetivos Alcanzados
- Configuración completa de un servidor DNS autoritativo con zonas directas e inversas.
- Creación de registros DNS variados (A, CNAME, PTR) para servicios como web, FTP, etc.
- Verificación de resolución DNS en red local.
- Buenas prácticas en seguridad y replicabilidad del setup DNS.

## Proceso Completo – Capturas Paso a Paso

<div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(320px, 1fr)); gap: 15px; margin: 30px 0;">

  <img src="screenshots/screenshots (1).png" alt="Paso 1">
  <img src="screenshots/screenshots (2).png" alt="Paso 2">
  <img src="screenshots/screenshots (3).png" alt="Paso 3">
  <img src="screenshots/screenshots (4).png" alt="Paso 4">
  <img src="screenshots/screenshots (5).png" alt="Paso 5">
  <img src="screenshots/screenshots (6).png" alt="Paso 6">
  <img src="screenshots/screenshots (7).png" alt="Paso 7">
  <img src="screenshots/screenshots (8).png" alt="Paso 8">
  <img src="screenshots/screenshots (9).png" alt="Paso 9">
  <img src="screenshots/screenshots (10).png" alt="Paso 10">
  <img src="screenshots/screenshots (11).png" alt="Paso 11">

</div>

> Las capturas muestran el flujo completo: edición de archivos /etc/bind/named.conf.local, zonas directas/inversas, configuraciones en VirtualBox/Clonezilla y pruebas con nslookup para registros A, CNAME, PTR.

## Aprendizajes Clave
- **Gestión de DNS con Bind**: Configuración de zonas y registros para resolución de nombres en redes locales.
- **Verificación y troubleshooting**: Uso de nslookup para comprobar la correcta resolución DNS.
- **Replicabilidad**: Clonación de servidores DNS para entornos de producción o testing.
- Aplicación práctica de conceptos de **networking**, **resolución de nombres** y **alta disponibilidad**.

## Relevancia Profesional
Este tipo de habilidades son altamente demandadas en:
- **Administración de redes** (configuración de DNS en empresas, ISPs o data centers).
- **Cloud & DevOps** (base para DNS en AWS Route 53, Azure DNS, etc.).
- **Ciberseguridad** (configuraciones seguras de DNS para evitar DNS spoofing o cache poisoning).

## Conclusión
Proyecto 100% funcional, documentado visualmente paso a paso y preparado para integrar en entornos reales con múltiples servidores.

¡Gracias por visitar mi repositorio! Si te interesa la administración de sistemas, cloud o ciberseguridad, dale una ⭐

---
**Autor**: Pau Olivé Moreno  
**Fecha**: Principios de 2025