


+++
author = "Valdecir Carvalho"
title = "Conheça o Oracle Cloud VMware Solution - OCVS"
date = "2020-09-16 07:00:00"
publishDate = "2020-09-16 07:00:00"
type = "post"
draft = "false"
url = "/conheca-o-oracle-cloud-vmware-solution-ocvs"
image = "/imagens/2020/MM/imagem.jpg"
description = "description"
tags = [
    "",
    "",
    "",
	"",
    "",
]
categories = ["Blog", ""]
+++

![image title](/imagens/2020/MM/imagem.jpg)

Olá Homelabers!

Acabei de perceber que já estou há 7 meses trabalhando na Oracle e 7 meses de pandemia. Comecei na Oracle, em uma quinta-feira, 12/03. Fui apenas dois dias ao escritório e na segunda-feira já estourou a pandemia e não voltei mais. Esse ano de 2020 além de estar uma loucura, passou voando. 

[https://homelaber.com.br/um-novo-comeco-oracle/](https://homelaber.com.br/um-novo-comeco-oracle/)

No post de hoje, vou falar sobre um "novo" produto da Oracle que estou conseguindo trabalhar bastante, o Oracle Cloud VMware Solution ou OCVS. A ideia desse post é aterrissar o assunto e depois, nos próximos posts aprofundar mais sobre o produto.

O OCVS foi anunciado pelo Mr. Oracle Larry Ellison em 2019 durante a Oracle Openworld e causou um grande furor na comunidade VMware, pois a parceria entre Oracle e VMware foi uma grande surpresa para muita gente - foi até chamado de O Milagre do Moscone

Eu me lembro que estava "namorando" com a Oracle na época e fiquei bastante animado com o anúncio e muito curioso para colocar minhas mãozinhas nesse produto.

O tempo passou e no último dia 06/08/2020 aconteceu o anúncio oficial e aqui estou eu para começar uma série sobre OCVS para vocês.

{{< target-blank title="" url="" >}}

## O que é o Oracle Cloud VMware Solution?
----
O Oracle Cloud VMware Solution ou OCVS é um produto da Oracle que permite executar o stack SDDC (VMware Cloud Foundation) da VMware em servidore Barel Metal na Oracle Cloud.

 - Um produto da Oracle que combina o Oracle Cloud Infrastructure e o
   software VMware
 - Uma solução certificada da plataforma VMware Cloud Foundation  
 - Vendido pela Oracle e por parceiros da Oracle

## Hardware & Software
 
O deploy de  um Cluster SDDC do Oracle Cloud VMware Solution inicia com um mínimo de 3 hosts Baremetal (oi vSan).

Cada host tem 52 oCPUs (Cores físicos), 768 GB RAM e 51 TB de Storage NVME SSD. O processador desse host Baremetal é um Intel Xeon Platinum 8167M de 2.0 GHz - ou seja, um senhor processador. 

No total, um cluster mínimo entrega 156 oCPUS (Cores Físicos), 2304 GB Memória RAM e 153 TB de Storage NVME SSD (raw). 

Falando de software, você pode escolher entre 2 versões do vSphere + NSX + vSAN:

vSphere 6.5 Update 3 ou vSphere 6.7 Update 3
NSX-T 2.5
vSAN 6.6 ou 6.7

## Principais Benefícios
----
It's JUST VMware!

Eu vejo vários benefícios do OCVS, principalmente se você tem workloads Oracle rodando On-Prem. 

1. Flexibilidade da Cloud - 
2. Controle
3. Gerenciamento
4. Localização - A Cloud Oracle hoje está presente em 18 localidades ao redor do mundo e no Brasil temos 1 DC operacional (em SP) e um próximo no roadmap para 2021. Você pode rodar o seu workload VMware no Brasil sem nenhum custo extra. Na Oracle Cloud, o custo é totalmente independe de onde o seu workload está - lindo isso não?

E lembrando que o cluster SDDC do OCVS roda dentro de uma VCN, ou seja, o seu VMware está ali do ladinho de todos os serviços OCI. 


## Casos de Uso
----

Os principais casos de uso para o OCVS na minha opinião são:

- Migração de Datacenter 
- Expansão de Capacidade
- DR
- 

## Mais informações
----
Video VMUG SP
https://youtu.be/8tmHQEJ_XcY

----
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzQ4NjYyODc1LC03MzQ1ODYwOTgsLTIzMD
QxNjMwNyw1MTc2NjUwODUsLTg4ODQ0NjkyMiwtMTk3ODg5MzE0
MSwxODg1NDkyNjc2LDQ1MDY2NDYxMl19
-->