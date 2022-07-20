Comando pra gerar uma key :

openssl req -x509 -newkey rsa:2048 -keyout chave.pem -out cert.pem -days 10



Comando pra escutar com a chave:
ncat -vnlp 8443 --ssl-key chave.pem --ssl-cert cert.pem


Para se conectar:
ncat -vn ip port --ssl