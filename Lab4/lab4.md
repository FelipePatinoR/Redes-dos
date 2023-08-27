# Practica de laboratorio 04 - Enrutamiento Dinámico RIP

<p>Creado por:
    <ul>
        <li>Danitza Milena Taimbud Pistala</li>
        <li>Jhon Jairo Corodba Lopez</li>
        <li>Daniel Felipe Patiño Ruano</li>
    </ul>
</p>

## Objetivos

### Objetivo General

Proporcionar el conocimiento y generar las habilidades necesarias en la configuración y gestión de dispositivos de redes.

### Objetivos Específicos:

- Conocer configuraciones básicas de enrutamiento dinámico con MikroTik.

---

## 1. Parámetros:

Para todos los efectos:

- la letra G se reemplaza por el número de grupo de laboratorio.
- la letra C de se reemplaza por el ultimo número de cédula del estudiante..
  on validos en todo el laboratorio.

[1_2]: https://github.com/GiancarloBenavides

## 2. [Preguntas reflexivas de ambientación](#) ✔

<ol type="a">
<li>¿Como funcionan los servidores DHCP y DNS?</li>
<li>¿Que desventajas tienen las rutas estáticas frente a las dinámicas?.</li>
<li>¿Cual es el algoritmo y la métrica que implementa RIP?.</li>
<li>¿Que diferencias hay entre las versiones 1 y 2 de RIP?. (Ventajas y Desventajas)</li>
<li>¿Que diferencias hay entre una IP estática, una IP dinámica y una IP reservada?.</li>

</ol>

## 3. [Configuración básica MikroTik-03](#) ✔

1. Conecte los equipos a la red eléctrica.
2. [Reinicie][3_1] los dispositivos a la configuración de fabrica.
3. Conecte la ultima interfaz [RJ45][rj45] del router al PC de configuración.
4. [Acceder][3_2] al dispositivo por el puerto 8291 via Winbox.
5. Cambiar el nombre del dispositivo para [identificarlo][3_3] como <code>R3</code>.
   ![Arquitectura](../Lab4/img-config-microtik/Paso%205.png "Cambiar nombre de dispositivo")
6. Etiquetar las [interfaces][3_4] a utilizar (2 WAN y una LAN).
   ![Arquitectura](../Lab4/img-config-microtik/Paso%206.png "Etiquetar Interfaces")
7. Conecte las interfaces [Ethernet][3_5] etiquetadas a los equipos vecinos.
8. Agregar un [bridge][3_6] y sus interfaces para la red LAN.
   ![Arquitectura](../Lab4/img-config-microtik/Paso%208.png "Agregar Bridge")
9. Agregar el direccionamiento para las dos redes externas WAN y la red interna LAN.
   1. Agregar la [dirección][5_1] de la interfaz externa que conecta con RM en el segmento IP 10.1.1.0/24.
   2. Agregar la [dirección][5_1] de la interfaz externa que conectara redes futuras en el segmento IP 10.33.1.0/24.
   3. Agregar la [dirección][5_1] del bridge (interna) con una IP 192.168.33.1 privada, clase C.
      ![Arquitectura](../Lab4/img-config-microtik/Paso%209.png "Agregar direccionamiento")
10. Agregar un [Pool][5_2] en el segmento de la LAN que asigne direcciones entre 192.168.33.100-192.168.33.200.
    ![Arquitectura](../Lab4/img-config-microtik/Paso%2010.png "Agregar pool")
11. Agregar un servidor [DHCP][5_3] y la información de puerta de enlace y DNS que enviara a los PC conectados a la LAN.
    ![Arquitectura](../Lab4/img-config-microtik/Paso%2011.png "Agregar servidor DHCP")
12. Convertir a [estático][5_4] el arrendamiento DHCP para la MAC del PC de configuración.

13. Cambiar la ip estática del pc de configuración a 192.168.33.10.
    ![Arquitectura](../Lab4/img-config-microtik/Paso%2012%20y%2013.png "Cambair ip estatica")
14. Configurar la [WLAN][wlan] de nombre "REDES_42" para proveer conectividad inalámbrica.
    ![Arquitectura](../Lab4/img-config-microtik/Paso%2014.png "Configurar WLAN")
15. Crear una regla [source NAT][5_5] en el cortafuegos para enmascarar la ip de origen.
16. Agregar la [ruta por defecto][5_6] 0.0.0.0/0.
    ![Arquitectura](../Lab4/img-config-microtik/Paso%2016.png "Agregar ruta por defecto")

## 4. [Configurar enrutamiento MikroTik-03](#) ✔

1. Agregar [Rip][8_1] a las interfaces conectadas a los router vecinos.
   ![Arquitectura](../Lab4/img-config-microtik/Paso%201%20RIP.png "Agregar ruta por defecto")

1. Publicar las [redes][8_2] que las interfaces rip deben compartir para que los tres router conozcan la ruta a los otros dos y a sus redes LAN.
   ![Arquitectura](../Lab4/img-config-microtik/Paso%202%20RIP.png "Agregar ruta por defecto")

1. Realizar pruebas de diagnostico [PING][8_3] y [TRACEROUTE][8_4] desde el router a los otros router.
1. Realizar pruebas de diagnostico [PING][ping] y [TRACERTE][tracert] desde un computador conectado via UTP a los otros router.
1. Realizar un [backup][8_5] de la configuración del equipo.

## 5. [Preguntas de conocimiento](#) ✔

1. ¿Por qué no se puede llegar a 10.10.1.100 desde R3 y 10.33.1.1 desde R1?
1. ¿Que se necesitaría para lograr llegar a 10.10.1.100 desde R2?
1. ¿Que se necesitaría para lograr llegar a 10.33.1.1 desde todos los routers?
1. ¿Permite el protocolo RIP compartir rutas entre diferentes Sistemas Autónomos? (Justifique)

[psk]: https://es.wikipedia.org/wiki/Pre-shared_key
[dhcp]: https://es.wikipedia.org/wiki/Protocolo_de_configuraci%C3%B3n_din%C3%A1mica_de_host
[wlan]: https://es.wikipedia.org/wiki/Red_de_%C3%A1rea_local_inal%C3%A1mbrica
[rj45]: https://es.wikipedia.org/wiki/RJ-45
[ping]: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/ping
[tracert]: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/tracert
[3_1]: https://wiki.mikrotik.com/wiki/Manual:Reset
[3_2]: https://wiki.mikrotik.com/wiki/Manual:Winbox
[3_3]: https://wiki.mikrotik.com/wiki/Manual:System/identity
[3_4]: https://wiki.mikrotik.com/wiki/Manual:Interface
[3_5]: https://wiki.mikrotik.com/wiki/Manual:Interface/Ethernet
[3_6]: https://wiki.mikrotik.com/wiki/Manual:Interface/Bridge
[5_1]: https://wiki.mikrotik.com/wiki/Manual:IP/Address
[5_2]: https://wiki.mikrotik.com/wiki/Manual:IP/Pools
[5_3]: https://wiki.mikrotik.com/wiki/Manual:IP/DHCP_Server
[5_4]: https://wiki.mikrotik.com/wiki/Manual:IP/DHCP_Server#Menu_specific_commands_2
[5_5]: https://wiki.mikrotik.com/wiki/Manual:IP/Firewall/NAT#Source_NAT
[5_6]: https://wiki.mikrotik.com/wiki/Manual:IP/Route#Default_route
[8_1]: https://wiki.mikrotik.com/wiki/Manual:Routing/RIP#Interface
[8_2]: https://wiki.mikrotik.com/wiki/Manual:Routing/RIP#Network
[8_3]: https://wiki.mikrotik.com/wiki/Manual:Tools/Ping
[8_4]: https://wiki.mikrotik.com/wiki/Manual:Troubleshooting_tools
[8_5]: https://wiki.mikrotik.com/wiki/Manual:System/Backup

---

## Mas Recursos

- [Wiki Mikrotik](https://wiki.mikrotik.com/wiki/Main_Page) (MikroTik - Wiki)
- [Video-Curso Mikrotik](https://www.youtube.com/watch?v=SLAPzl-LSc0&list=PLf0g2cV4iCkH19_UhaVt0vDn1f9ObumjF) (Wiki)
- [Encaminamiento](https://es.wikipedia.org/wiki/Encaminamiento) (Wikipedia)
- [RIP](https://es.wikipedia.org/wiki/Routing_Information_Protocol) (Wikipedia)
- [Calculadora IP](https://www.calculator.net/ip-subnet-calculator.html) (Wikipedia)
