permitir apenas ip especifico no ncat:


comando completo:
ncat -vnlp 8443 --ssl-key xyz.pem --ssl-cert cert.pem --allow 192.168.0.2


--allow ip = permite apenas esse ip