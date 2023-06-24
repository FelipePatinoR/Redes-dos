## Telematics
<p><code>Fundamentos de Telemática</code></p>
<p>Creado por <code>Daniel Felipe Patiño , Jhon Jairo Cordoba y Danitza Milena Taimbud</code> para realizar el desarrollo de la <code>guia de laboratorio 2 </code> en los cursos de telemática y redes de computadores.</p>

# Practica de laboratorio 02

## Objetivos 

### Objetivo General
Proporcionar el conocimiento y generar las habilidades necesarias en la configuración y gestión de dispositivos de redes.

### Objetivos Específicos:
- Conocer los números necesarios para configurar el direccionamiento de una red de area local. :+1: 

---

## Parámetros:
Para todos los efectos:
* la letra G  de se reemplaza por el número de grupo de laboratorio.
* la letra C  de se reemplaza por el ultimo número de cédula del estudiante.


## 1. [Configurar el entorno de trabajo](#) ✔
1. Cree si no existe el repositorio [__"REDES-2"__][1_2] en su cuenta de github.
1. Agregue un archivo llamado [__"laboratorio_2.md"__][1_2] a este repositorio.
1. Invite a los compañeros de grupo como colaboradores en este repositorio.
1. Documente cada uno de los items a continuación con capturas de pantalla y código .

>Nota: recuerde que los [parámetros](#parámetros) son validos en todo el laboratorio.

[1_2]:https://github.com/GiancarloBenavides

## 2. [Preguntas reflexivas de ambientación](#) ✔

<ol type="a">
<li>¿Como se llama la interfaz donde se conecta los cables UTP.?</li>

 __R/.__ *La interfaz donde se conectan los cables UTP en los enrutadores se llama puerto Ethernet.*


<li>¿Que significa POE IN y POE OUT en una interfaz?.</li>


__R/.__*POE IN (Power over Ethernet In) se refiere a una función que permite suministrar energía eléctrica a través del cable Ethernet a un dispositivo compatible, como una cámara de seguridad o un teléfono IP. Es decir, el enrutador está proporcionando energía al dispositivo conectado.*

*POE OUT (Power over Ethernet Out) se refiere a la capacidad de un enrutador para recibir energía a través de un cable Ethernet y suministrarla a otro dispositivo conectado a través de un puerto compatible con Power over Ethernet. En este caso, el enrutador actúa como una fuente de alimentación para el dispositivo conectado.*

<li>¿Que utilidad tiene la interfaz USB en los Enrutadores?.</li>

__R/.__ *La interfaz USB en los enrutadores tiene varias utilidades que pueden depender del modelo específico del enrutador y de las características que ofrece. Algunas de las funciones comunes de la interfaz USB en los enrutadores son las siguientes:*

*Compartir archivos: Algunos enrutadores permiten conectar dispositivos de almacenamiento USB, como unidades flash o discos duros externos, a través del puerto USB. Esto permite compartir archivos y medios de manera fácil y rápida en la red local.*

*Impresión en red: Al conectar una impresora USB al puerto USB del enrutador, es posible compartir la impresora en toda la red local. Esto permite que múltiples dispositivos puedan imprimir a través de la misma impresora sin tener que conectarla directamente a cada dispositivo.*

*Acceso a Internet móvil: Algunos enrutadores ofrecen la función de módem USB, lo que significa que puedes conectar un módem USB 3G/4G o un teléfono móvil al puerto USB para acceder a Internet utilizando una conexión móvil. Esto es especialmente útil en áreas donde no hay una conexión de banda ancha fija disponible.*

*Almacenamiento en red (NAS): Algunos enrutadores con puerto USB tienen la capacidad de funcionar como servidores de almacenamiento en red (NAS, por sus siglas en inglés). Puedes conectar un disco duro externo al puerto USB y configurar el enrutador para que actúe como un servidor de archivos, permitiendo el acceso remoto y compartiendo archivos en la red local.*

*Actualización de firmware: En algunos casos, el puerto USB también se puede utilizar para actualizar el firmware del enrutador. Esto puede ser útil para mantener el enrutador actualizado con las últimas características y mejoras de seguridad.*

*Es importante tener en cuenta que no todos los enrutadores tienen un puerto USB y que las funciones disponibles pueden variar según el modelo y el fabricante del enrutador. Si estás interesado en utilizar alguna de estas funciones, te recomendaría consultar la documentación del enrutador específico que estás utilizando para obtener más detalles sobre las capacidades de su puerto USB.*

<li>¿Que utilidad tiene la interfaz SFP en los Enrutadores?.</li>

__R/.__ *- La interfaz SFP (Small Form-Factor Pluggable) en los enrutadores tiene varias utilidades y beneficios. SFP es un formato estándar para módulos ópticos y de red que permite la conexión de distintos tipos de interfaces de red a través de un conector compatible.*

*- Conexión de fibra óptica: La interfaz SFP es ampliamente utilizada para la conexión de enrutadores a redes de fibra óptica. Los módulos SFP ópticos permiten transmitir datos a través de cables de fibra óptica, que ofrecen velocidades más altas y una mayor capacidad de transmisión a largas distancias en comparación con los cables de cobre tradicionales.*

*- Flexibilidad y modularidad: La interfaz SFP permite la flexibilidad y la modularidad en los enrutadores. Los módulos SFP son intercambiables en caliente, lo que significa que se pueden insertar o quitar sin apagar el enrutador. Esto permite una mayor flexibilidad para adaptarse a diferentes necesidades de conectividad, ya sea utilizando módulos ópticos SFP para conectividad de fibra o módulos SFP de cobre para conexiones Ethernet estándar.*

*- Distancias largas: Los módulos SFP ópticos ofrecen la capacidad de transmitir datos a distancias más largas en comparación con los cables de cobre. Esto es especialmente útil cuando se necesita conectar enrutadores a través de grandes áreas geográficas o en entornos donde las distancias de cableado son significativas.*

*- Velocidades de transmisión: Los módulos SFP ofrecen diferentes velocidades de transmisión, como 1 Gigabit Ethernet (1GbE), 10 Gigabit Ethernet (10GbE) o incluso velocidades más altas, dependiendo del tipo de módulo SFP utilizado. Esto permite una mayor capacidad de ancho de banda y velocidades de transferencia de datos más rápidas en comparación con las interfaces Ethernet estándar.*

*- Conectividad de redes específicas: Además de la conectividad de fibra óptica, los módulos SFP también pueden admitir otros tipos de redes, como conexiones de red inalámbrica (Wi-Fi), conexiones de línea telefónica (T1/E1) o conexiones de redes de área local virtuales (VLAN), entre otros.*


<li>¿Que tipos de interface Ethernet se pueden encontrar en los Enrutadores?.</li>

__R/.__*Los enrutadores pueden tener una variedad de interfaces Ethernet dependiendo del modelo y la funcionalidad específica del enrutador. Aquí hay algunos tipos comunes de interfaces Ethernet que se pueden encontrar en los enrutadores:*

*Ethernet 10/100: Esta es una interfaz Ethernet estándar que admite velocidades de 10 Mbps y 100 Mbps. Es ampliamente utilizada en enrutadores para conexiones Ethernet de baja velocidad.*

*Gigabit Ethernet (10/100/1000): Estas interfaces Ethernet admiten velocidades de 10 Mbps, 100 Mbps y 1 Gbps (1,000 Mbps). Son comunes en enrutadores de gama media y alta, y permiten una mayor capacidad de transmisión de datos.*

*10 Gigabit Ethernet: Estas interfaces Ethernet admiten velocidades de 10 Gbps (10,000 Mbps). Se utilizan en enrutadores de alto rendimiento y se utilizan en entornos donde se requiere una gran capacidad de ancho de banda, como centros de datos o redes empresariales de alta demanda.*

*Interfaces SFP/SFP+: Estas interfaces utilizan módulos SFP (Small Form-Factor Pluggable) o SFP+ para admitir conexiones ópticas o de cobre intercambiables en caliente. Los módulos SFP o SFP+ permiten la flexibilidad para adaptarse a diferentes tipos de cables y velocidades, como fibra óptica o cables Ethernet de cobre, y ofrecen velocidades de hasta 10 Gbps o incluso más altas.*

*Interfaces 40/100 Gigabit Ethernet: Estas interfaces Ethernet admiten velocidades de 40 Gbps y 100 Gbps. Son utilizadas en enrutadores de nivel empresarial y en entornos de alto rendimiento donde se requiere un ancho de banda extremadamente alto.*


</ol>

## 3. [Caracterizar el CPE TP-LINK](#) ✔
|Parámetro||Valor|
|--|:--:|--:|
|Marca|-->||
|Referencia|-->||
|Velocidad de la CPU|-->||
|Tamaño de la memoria RAM|-->||
|Sistema Operativo|-->||
|Tipo de WIFI|-->||
|Voltaje DC|-->||


## 4. [Configurar básica de CPE TP-LINK](#) ✔
1. Conecte los equipos a la red eléctrica.
1. [Reiniciar][4_1] el dispositivo a la configuración de fabrica.
1. Conectar el equipo mediante un patchcord (latiguillo) al equipo y a internet.
1. [Acceder][4_2] al dispositivo via protocolo http desde el navegador web.
1. Cambiar el nombre del dispositivo para identificarlo.
1. Configurar la direccionamiento WAN para lograr conectividad con la red externa.
1. Configurar la direccionamiento LAN con una IP privada, clase C para lograr conectividad con la red interna.
1. Configurar el [DHCP][dhcp] para que asigne 20 direcciones IP entre [G](#parámetros).200-[G](#parámetros).220.
1. Configurar la [WLAN][wlan] de nombre y [PSK](psk) "REDES_4[G](#parámetros)" para lograr conectividad inalámbrica.
1. Realizar pruebas [PING][4_3] a DNS Cloudflare desde el dispositivo.
1. Realizar pruebas [PING][4_3] a DNS Cloudflare desde el computador conectado por UTP.
1. Realizar pruebas [TRACEROUTE][4_4] a DNS Google desde el router.
1. Realizar pruebas [TRACEROUTE][4_4] a DNS Google desde el Computador conectado por UTP.
1. Realizar pruebas [TRACEROUTE][4_4] a DNS Google desde un dispositivo conectado por WIFI.
1. Habilitar la gestión remota del dispositivo desde cualquier IP.
1. Realizar un backup de la configuración del equipo.

>Router: [TP-LINK][4_5] -> reiniciar: [Con el Router encendido dejamos presionado el botón reset durante 10 segundos hasta  LED SYS/PWR parpadee rápidamente][4_1] acceder: [conectar con la cadena admin:admin@tplinkwifi.net][4_2]

## 5. [Caracterizar la ONT HUAWEI](#) ✔
|Parámetro||Valor|
|--|:--:|--:|
|Marca|-->|Huawei|
|Referencia|-->|HS8545M5|
|Velocidad de la CPU|-->||
|Tamaño de la memoria RAM|-->||
|Sistema Operativo|-->|HarmonyOS (HMOS)|
|Tipo de WIFI|-->||
|Voltaje DC|-->|12V, 1.5A|

## 6. [Configurar básica de ONT HUAWEI](#) ✔
1. Conecte los equipos a la red eléctrica.
    ![](/Lab2/Img_ONT/1.jpg)
1. [Reinicie][6_1] los dispositivos a la configuración de fabrica.
    ![](/Lab2/Img_ONT/2.jpg)
1. Conecte los equipo mediante un patchcord (latiguillo) al equipo y a internet.
    ![](/Lab2/Img_ONT/3.jpg)
    ![](/Lab2/Img_ONT/3.1.jpg)
1. [Acceder][6_2] al dispositivo via protocolo http desde el navegador web.
    ![](/Lab2/Img_ONT/4.png)
    ![](/Lab2/Img_ONT/4.1.png)
    ![](/Lab2/Img_ONT/4.2.png)
1. Configurar la direccionamiento LAN con una IP privada, clase B para lograr conectividad con la red interna.
    ![](/Lab2/Img_ONT/5.png)
1. Configurar el [DHCP][dhcp] para que asigne 50 direcciones IP entre [GG](#parámetros).150-[GG](#parámetros).200.
    ![](/Lab2/Img_ONT/6.png)
1. Reservar una IP fija en la red interna para la MAC del un computador (Servidor).
    ![](/Lab2/Img_ONT/7.png)
1. Configurar la [WLAN][wlan] de nombre y [PSK](psk) "REDES_4[G](#parámetros)" para lograr conectividad inalámbrica.
    ![](/Lab2/Img_ONT/8.png)
1. Realizar pruebas [PING][4_3] a la puerta de enlace desde el computador conectado por UTP (Servidor).
    ![](/Lab2/Img_ONT/9.png)
1. Realizar pruebas [PING][4_3] a la puerta de enlace desde el computador conectado por WIFI (Cliente).
    ![](/Lab2/Img_ONT/10.png)
1. Realizar pruebas [PING][6_3] a la puerta de enlace desde un teléfono Movil conectado por WIFI.
    ![](/Lab2/Img_ONT/11.jpg)
    ![](/Lab2/Img_ONT/11.1.jpg)
1. Listar los dispositivos por tipo que aparecen en "DHCP Information".
    ![](/Lab2/Img_ONT/12.png)
1. Mapear el puerto 80 del router para que redirija a un servicio [Python][6_4] en un computador.
    ![](/Lab2/Img_ONT/13.png)
1. Verificar que se puede acceder al servicio (pagina web) desde los dos clientes (móvil y PC).
    ![](/Lab2/Img_ONT/14.png)
    ![](/Lab2/Img_ONT/14.1.png)
1. Habilitar la gestión remota del dispositivo desde cualquier IP.
    ![](/Lab2/Img_ONT/15.png)
1. Realizar un backup de la configuración del equipo.
    ![](/Lab2/Img_ONT/16.png)

>ONT: [HUAWEI][6_5] -> reiniciar:[Con el Router encendido dejamos presionado el botón reset durante 2 segundos hasta  hasta que los LEDs se apaguen][6_1] acceder: [conectar con la cadena user:twtvu@192.168.1.1][6_2]

## 7. [Caracterizar el router MikroTik](#) ✔
|Parámetro||Valor|
|--|:--:|--:|
|Marca|-->|MikroTik Routerboard|
|Referencia|-->|RB931-2nD|
|Velocidad de la CPU|-->|CPU 650 MHz|
|Tamaño de la memoria RAM|-->|RAM 32 MB|
|Sistema Operativo|-->|kernel de Linux 2.6|
|Tipo de WIFI|-->|802.11b / g / n|
|Voltaje DC|-->|5-5 voltios|

## 8. [Configurar básica de router MikroTik](#) ✔
1. Conecte los equipos a la red eléctrica.
    ![](/Lab2/Img_MikroTik/1.png)
1. [Reinicie][8_1] los dispositivos a la configuración de fabrica.
    ![](/Lab2/Img_MikroTik/2.png)
1. Conecte los equipo mediante un patchcord (latiguillo) al equipo y a internet.
    ![](/Lab2/Img_MikroTik/3.png)
    ![](/Lab2/Img_MikroTik/3.1.png)
1. [Acceder][8_2] al dispositivo por el puerto 8291 via Winbox.
    ![](/Lab2/Img_MikroTik/4.png)
    ![](/Lab2/Img_MikroTik/4.1.png)
1. Cambiar el nombre del dispositivo para identificarlo.
    ![](/Lab2/Img_MikroTik/5.png)
    ![](/Lab2/Img_MikroTik/5.1.png)
1. Cambiar la contraseña del usuario "admin" a "Redes_2".
    ![](/Lab2/Img_MikroTik/6.png)
    ![](/Lab2/Img_MikroTik/6.1.png)
    ![](/Lab2/Img_MikroTik/6.2.png)
1. Configurar las [interfaces][8_3] y el [bridge][8_4] (conmutador) para dos redes (Interna y externa).
    ![](/Lab2/Img_MikroTik/7.png)
    ![](/Lab2/Img_MikroTik/7.1.png)
1. Agregar la [dirección][8_5] de la interfaz externa en el segmento necesario para acceder a internet.
    ![](/Lab2/Img_MikroTik/8.png)
    ![](/Lab2/Img_MikroTik/8.1.png)
    ![](/Lab2/Img_MikroTik/8.2.png)
1. Agregar la [dirección][8_5] del bridge (interna) con una IP privada, clase A.
    ![](/Lab2/Img_MikroTik/9.png)
1. Agregar un [Pool][8_6] en el segmento de la LAN que asigne direcciones entre [GG](#parámetros).100-[GG](#parámetros).200.
    ![](/Lab2/Img_MikroTik/10.png)
1. Configurar el [DHCP][dhcp] y las rutas estáticas necesarias para lograr conectividad de la red interna con internet.
    ![](/Lab2/Img_MikroTik/11.png)
    ![](/Lab2/Img_MikroTik/11.1png)
    ![](/Lab2/Img_MikroTik/11.2.png)
    ![](/Lab2/Img_MikroTik/11.3.png)
1. Configurar la [WLAN][wlan] de nombre y [PSK](psk) "REDES_4[G](#parámetros)" para lograr conectividad inalámbrica.
    ![](/Lab2/Img_MikroTik/12.png)
    ![](/Lab2/Img_MikroTik/12.1.png)
    ![](/Lab2/Img_MikroTik/12.3.png)
    ![](/Lab2/Img_MikroTik/12.4.png)
    ![](/Lab2/Img_MikroTik/12.5.png)
    ![](/Lab2/Img_MikroTik/12.6.png)
    ![](/Lab2/Img_MikroTik/12.7.png)
1. Realizar pruebas de diagnostico [PING][8_7] y [TRACEROUTE][4_4] desde el router.
    ![](/Lab2/Img_MikroTik/13.png)
    ![](/Lab2/Img_MikroTik/13.1.png)
    ![](/Lab2/Img_MikroTik/13.2.png)
1. Realizar pruebas de diagnostico [PING][4_3] y [TRACEROUTE][4_4] desde un computador conectado via UTP.
    ![](/Lab2/Img_MikroTik/14.png)
    ![](/Lab2/Img_MikroTik/14.1.png)
    ![](/Lab2/Img_MikroTik/14.2.png)
    ![](/Lab2/Img_MikroTik/14.3.png)
1. Realizar pruebas de diagnostico [PING][4_3] y [TRACEROUTE][4_4] desde un computador conectado via WIFI.
    ![](/Lab2/Img_MikroTik/15.png)
    ![](/Lab2/Img_MikroTik/15.1.png)
    ![](/Lab2/Img_MikroTik/15.2.png)
    ![](/Lab2/Img_MikroTik/15.3.png)
    ![](/Lab2/Img_MikroTik/15.4.png)
1. Realizar un backup de la configuración del equipo.
    ![](/Lab2/Img_MikroTik/16.png)
    ![](/Lab2/Img_MikroTik/16.1.png)
    ![](/Lab2/Img_MikroTik/16.2.png)
    ![](/Lab2/Img_MikroTik/16.3.png)
>ROUTER: [MikroTik][8_5] -> reiniciar:[Con el botón de reset presionado encendemos el equipo. Dejamos presionado el botón reset durante 2-3 segundos hasta que veamos parpadear alguno de los LEDs de servicio][8_1] Acceder:[instale winbox y acceda por la pestaña "Neighbors" Login:admin y Password:admin][8_2]

## 9. [Diagrama de Red](#) ✔
- Realice un diagrama topológico de cada uno de los casos de estudio.
- Incluya todos los detalles de la red de area local a la que se encuentra conectado.
- Incluya los saltos conocidos incluyendo el equipo de borde de su ISP.

## 10. [Preguntas de conocimiento](#) ✔
1. ¿Que diferencias hay entre cada una de las implementaciones? (Ventajas y Desventajas)

__R/.__**
1. ¿Que diferencias existe en el retardo via WIFI vs el retardo via UTP? (Justifique)

__R/.__*En una conexión Wi-Fi, los datos se transmiten a través del aire utilizando ondas de radio. Esto puede introducir mayor variabilidad en la señal debido a factores como la interferencia electromagnética, obstáculos físicos y la presencia de otros dispositivos inalámbricos en la misma banda de frecuencia. En cambio, una conexión por cable UTP utiliza cables de cobre para la transmisión de datos, lo que proporciona una conexión física directa y más estable.*

*Una conexión por cable UTP puede proporcionar un ancho de banda más alto en comparación con una conexión Wi-Fi. Esto significa que la conexión por cable tiene la capacidad de transmitir una mayor cantidad de datos en un período de tiempo determinado. Un mayor ancho de banda puede contribuir a una menor latencia, ya que los datos pueden transferirse más rápidamente a través del cable.*

*Los dispositivos Wi-Fi requieren un procesamiento adicional para recibir y enviar datos a través de las ondas de radio. Esto implica un tiempo de procesamiento adicional que puede contribuir a una mayor latencia en comparación con las conexiones por cable UTP, donde la transmisión es directa y no requiere procesamiento adicional.*

1. ¿Cual es la puerta de enlace a internet? ¿Cual es la ruta por defecto? En el punto (8)
1. ¿Existe diferencia en las trazas hacia los DNS en internet, para cada medio de transmisión y dispositivo? (Justifique)

[psk]:https://es.wikipedia.org/wiki/Pre-shared_key
[dhcp]:https://es.wikipedia.org/wiki/Protocolo_de_configuraci%C3%B3n_din%C3%A1mica_de_host
[wlan]:https://es.wikipedia.org/wiki/Red_de_%C3%A1rea_local_inal%C3%A1mbrica
[4_1]:https://www.tp-link.com/ar/support/faq/497/
[4_2]:https://static.tp-link.com/res/down/doc/TL-WR840N(ES)_V2_QIG.pdf
[4_3]:https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/ping
[4_4]:https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/tracert
[4_5]:https://www.tp-link.com/co/home-networking/wifi-router/tl-wr840n/
[6_1]:https://consumer.huawei.com/co/support/content/es-us15855743/
[6_2]:https://forum.huawei.com/enterprise/es/%C2%BFc%C3%B3mo-iniciar-sesi%C3%B3n-en-ont-de-huawei/thread/636939-100243
[6_3]:https://play.google.com/store/apps/details?id=com.lipinic.ping&hl=es_419&gl=US
[6_4]:https://docs.python.org/3.10/library/http.server.html
[6_5]:https://support.huawei.com/enterprise/es/access-network/echolife-hg8546m-pid-21465065
[8_1]:https://wiki.mikrotik.com/wiki/Manual:Reset
[8_2]:https://wiki.mikrotik.com/wiki/Manual:Winbox
[8_3]:https://wiki.mikrotik.com/wiki/Manual:Interface/Ethernet
[8_4]:https://wiki.mikrotik.com/wiki/Manual:Interface/Bridge
[8_5]:https://wiki.mikrotik.com/wiki/Manual:IP/Address
[8_6]:https://wiki.mikrotik.com/wiki/Manual:IP/Pools
[8_7]:https://wiki.mikrotik.com/wiki/Manual:Tools/Ping
[8_8]:https://wiki.mikrotik.com/wiki/Manual:Troubleshooting_tools

---
## Mas Recursos
- [Wiki Mikrotik](https://wiki.mikrotik.com/wiki/Main_Page) (Wiki)
- [Video-Curso Mikrotik](https://www.youtube.com/watch?v=SLAPzl-LSc0&list=PLf0g2cV4iCkH19_UhaVt0vDn1f9ObumjF) (Wiki)
- [Direccionamiento IP](https://es.wikipedia.org/wiki/Direcci%C3%B3n_IP) (Wikipedia)
- [Calculadora IP](https://www.calculator.net/ip-subnet-calculator.html) (Wikipedia)

---
## Evaluación y rúbrica
- Fecha máximo entrega: 05 de Mayo de 2023
- Hora de entrega: 11:59pm	
- Nota máxima: 5.0 
- Número de actividades: 10
- Valor de cada actividad: 0.5
- Ponderación: 20%
- $\color{#DD69DD}{\text{...Carpe Diem}}$
