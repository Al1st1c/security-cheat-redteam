
Criar um honeypot

Comando completo:
while true;do nc -vnlp 21 < 21.txt 1>> 21.log 2>> 21.log;echo $(date) >> 21.log;done

While true; do ________ ;done (Mantém a conexão ativa)

nc - netcat
-vnlp (opções do netcat)
-v = Verbose, assistir o background
-n = Resolver apenas IP
-l = Listen, escutar
-p = porta

< 21.txt = Diz que ao acessarem o ip/porta aberto pelo nc, quem acessou vai ver o conteudo desse arquivo


1>> 21.log = Salva o retorno de sucesso

2>> 21.log = Salva o retorno de erro

;echo $(date) = concatena e exibe uma data
