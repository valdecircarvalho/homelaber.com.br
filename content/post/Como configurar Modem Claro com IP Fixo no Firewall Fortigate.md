author = "Valdecir Carvalho"
title = "Firewall Fortinet Fortigate 60D no Home Lab"
date = "2020-10-06 07:00:00"
publishDate = "2020-10-06 07:00:00"
type = "post"
draft = "false"
url = "/firewall-fortigate-60d-no-home-lab"
image = "/imagens/2020/10/firewall-fortinet-fortigate-60d-homelab.jpg"
description = "Recentemente comprei um Firewall Fortinet Fortigate 60D para usar no meu lab. Nesse posts eu conto como e porque escolhi esse equipamento, suas caracteristicas técnicas e como estou usando esse firewall no meu home lab."
tags = [
    "Lab",
    "Homelab",
    "Fortigate",
    "Fortinet",
    "60D",
    "Fortigate 60D",
    "Firewall Fortigate 60D",
    "Blogtober2020",
    "Blogtober",
    "BlogtoberTech",
]
categories = ["Blog", "Homelab", "Lab", "Fortigate", "Blogtober"]

+++

Olá Homelabers!

Feliz 2021 para todos!

Estou para escrever esse post já tem um tempo, mas agora vai. 

Em agosto de 2020 eu resolvi contratar um novo link de internet, o principal motivador era ter um link com IP fixo para usar no lab para fechar VPN com algumas Clouds e fazer testes e estudos e também ter um backup, caso o meu link principal da Vivo (Fibra) tivesse algum problema técnico.

Pesquisei bastante sobre as operadoras que atendem o meu bairro aqui em Guarulhos e no final acabou sobrando apenas a Claro como opção.

Link contratado, instalado e tudo funcionando, chegou a hora de configurar o link no meu Firewall Fortigate 60D (veja esse post)

**Como configurar Modem Claro com IP Fixo no Firewall Fortigate**

Para que o o Firewall seja o gateway da rede e fique com o IP Fixo do Link, é preciso colocar o Modem em modo Bridge, ou seja, ele será responsável apenas pela conexão com o seu provedor.

O modem da que a Claro disponibilizou é um XXXXXXX

Aqui existem dois lugares, onde você deve informar (ou já deve vir configurado) as informações do seu IP Fixo - fornecido pela Claro.

O primeiro lugar, é no menu REDES >> CONFIGURAÇÕES BÁSICAS. E o segundo lugar é no menu REDES >> CONFIGURAÇÃO DE WAN.

Nas configurações básicas, você deve informar que o tipo de conexão WAN é Modo Bridge.

Antes de mudar as configurações, tome nota do IP, Subnet, Gateway, DNS, etc.

Feito isso, clique em Aplicar Ajustes.

Agora, vamos a configuração do Fortigate.

Eu estou usando a interface WAN1.

Na sessão Address, escolha Manual em Addressing Mode

Preencha o IP/Network Mask com as informações fornecidas pela Claro - ou que você tenha anotado das configurações do seu modem. Use o formato 000.000.000.00/000.000.000.000

Na sessão Administrative Access, escolha PING - caso você queira que o seu Firewall responda pings na internet.

Em Status, deixe o Interface State como Enabled.

O próximo passo, é configurar a rota. 

Faça as configurações como na imagem abaixo

Para validar a sua conexão, execute um simples teste de ping, se funcionar, está OK!

