# Práctica: Balanceo de carga con Nginx

(Aquí va la documentación: diagrama, tabla de IPs, configs y pasos)
                      Cliente (navegador)
                             |
                             v
                  +----------------------+
                  | Balanceador (Nginx)  |
                  | 192.168.139.143      |
                  +----------+-----------+
                             |
              +--------------+--------------+
              |                             |
              v                             v
   +---------------------+       +---------------------+
   | Página 1 (Nginx)    |       | Página 2 (Nginx)    |
   | 192.168.139.144     |       | 192.168.139.145     |
   +---------------------+       +---------------------+

   VM SSH (192.168.139.142): único punto de administración
   hacia el balanceador y las dos páginas.

SSH 192.168.139.142

   
