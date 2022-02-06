layout: page
title: "Prueba"
permalink: /prueba/

# SecNotes
Empezamos haciendo el escaneo con masscan que en principio, nos saca más información que nmap.

![[Pasted image 20220126093617.png]]
Ahora podemos lanzar un escaneo específico contra estos puertos usando Nmap.

``nmap -sV -p80,8808,445 10.10.10.97``

![[Pasted image 20220126094402.png]]

### Puerto 80
![[Pasted image 20220126094739.png]]
Analizamos con gobuster nuestro puerto 80 y lo que parece es que podemos registrarnos sin problema para acceder al panel, este panel tiene pinta de que la utilidad de cambiar contraseña, lo podemos usar para cambiar la pass de otro user tal vez.

![[Pasted image 20220126101604.png]]


### Puerto 8808
![[Pasted image 20220126100814.png]]
