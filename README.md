# examen2
INSTRUCCIONES
El objeto de la práctica es crear una virtual, y configurarla de forma automatizada, con la ayuda de Terraform y Ansible.

En este sentido se debe preparar una máquina virtual con sistema operativo Ubuntu Server 18.04 LTS https://ubuntu.com/download/server con las siguientes características:

              Memoria RAM 4G - 8G
              4 procesadores
              Almacenamiento 16 G - 32 G
              Una Tarjeta de Red
              Acceso a Internet
              
 En hyper-V se debe habilitar la virtualización anidada (de acuerdo a https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/user-guide/nested-virtualization )

En una consola de PowerShell (en modo administrador se debe correr) con la maquina virtual apagada:

Set-VMProcessor -VMName UbuntuServer -ExposeVirtualizationExtensions $true 
Donde UbuntuServer es el nombre de la maquina virtual
