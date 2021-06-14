---
title: 'No hello world allowed, this is another testing'
date: 2021-06-13 03:54:42
tags: 
- command
- linux
---
## Title 2

Esto es un post de prueba. Lo voy a borra en los proximos dias. 

Ahi, estaba hablando de las ventajas y desventajas de usar passwd como -l o -d en un servidor con acceso unico de SSH. lol

---

Cabe mencionar que este apartado consiste en solamente consejos y posibilidades, por lo que cada una de ellas debe de considerarse en un entorno de Produccion.

- Por lo que si la opcion esta seteada como `no` entonces el usuario no podra logearse de ninguna manera al servidor.
  - En el caso de las cuentas que estas en modo ((60be999b-3fdf-49cd-8d7d-b9b57e2884dd)) dependeran de la configuracion que se realice en el file `/etc/ssh/sshd_config/PermitEmptyPasswords` si esta seteado en `yes`
    - La ventaja de este metodo es que los usuarios no requeriran el password para poder logearse al servidor usando [[SSH]]. Incluso si sus cuentas tenian configurado el password para realizar `sudo` podran hacerlo sin requerir un password.
    - `$ sudo passwd -d user1`
  - **Delete**
    - Esto tambien implica que cuando se ocupe usar `sudo` tambien es necesario usar el password.
    - En el momento que usamos la opcion de bloquear el password, la ventaja es que los password sigue por ahi, por lo que se oueden descloquear y seguir utilizando el password.
    - `$ sudo passwd -l user1`
  - **Lock**
- **The difference between passwd -l and passwd -d** #article
  - URL: https://nts.strzibny.name/passwd-lock-vs-passwd-delete/
  - Existen varias maneras de poder cancelar el password en Linux.
    - Se puede eliminar el password del todo o bien se puede solamente bloquear. Incluso se pueden hacer ambos. _Pero que implicaciones puede traer esto_?