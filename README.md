## Projeto semestral

**Grupo:** 
<br>Vinicius Moura RA 2219204443 <br>
Getulio Vilanova dos Santos RA 2219202701<br>
Pedro Henrique RA 2219205952<br>
Murilo Alexandre Araújo RA 2219200153<br>

Repositório criado para o projeto do 5º semestre do curso de Tecnologia em Análise e Desenvolvimento de Sistemas.

Site do Blog -> 54.94.31.63

#Para acesso ao sistema
1- Abra um cliente SSH.
2- Localize o arquivo de chave privada. A chave usada para executar esta instância é debianCloud.pem
3- Execute este comando, se necessário, para garantir que sua chave não fique visível publicamente.
`chmod 400 debianCloud.pem`
4- Conecte-se à sua instância usando sua DNS pública:
`ec2-54-94-31-63.sa-east-1.compute.amazonaws.com`
Exemplo:
`ssh -i "debianCloud.pem" admin@ec2-54-94-31-63.sa-east-1.compute.amazonaws.com -p 22`

#CronJob
O sistema tem um script .sh, que a cada 1 minuto ele executa o comando git pull, e atualiza os arquivos na pasta raiz do sistema WEB, mantendo o site atualizado com a ultima versão disponivel no repositorio.
