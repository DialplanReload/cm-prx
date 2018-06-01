[![N|Solid](docs/images/img-opens-off.png)](https://opens.com.br)
# ZBX-PROXY

Modulo para monitoramento de ambientes. Criado pela Opens, baseado em Zabbix e usando métodos ágeis para Continuous Monitoring.

O uso do ZBX-PROXY NÃO __DISPENSA__ o uso do ZBX-AGENT.


# IMPORTANTE

O módulo PROXY deve ser instalado em apenas um dos servidores do cliente. Caso seja somente um SNEP, este deve possuir os dois módulo, proxy e agent. Caso seja mais de uma central ou algum outro modelo que o ambiente tenha mais de um servidor a ser monitorado, somente um deve possuir o proxy e agent.

A escolha é livre, porém a recomendação é ser feito sempre na matriz/dac.

## Composição do ZBX-PROXY

1. zabbix/__zabbix-proxy-mysql__ - Container rodando o proxy do Zabbix em mysql na versão ubuntu-3.4.7.

2. openstec/__mysql__ - Container rodando o banco de dados utilizado pelo proxy.

