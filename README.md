# Rede Residencial no Cisco Packet Tracer

## O que é este projeto?

Neste laboratório, montei do zero uma **rede doméstica simples** (parecida com a que temos em casa). 

O objetivo foi conectar dois computadores; um de mesa (via cabo) e um notebook (via Wi-Fi); a um roteador e modem, garantindo que ambos conseguissem navegar na internet e acessar um site de teste.

---

## Como a rede ficou montada (Topologia)

Abaixo está o mapa visual da rede montada dentro do simulador:

<img width="1197" height="661" alt="Visão Geral" src="https://github.com/user-attachments/assets/1891b0e9-73a6-411b-8027-5fca7547e2f0" />



### Dispositivos e Conexões Utilizadas:
* **PC:** Conectado ao roteador usando um cabo de rede comum (cabo Ethernet).
* **Roteador Sem Fio:** Recebe o sinal e distribui a internet por cabo e por Wi-Fi.
* **Cable Modem:** Aparelho que converte o sinal de internet que vem da rua (cabo coaxial) para a nossa rede de casa.
* **Notebook:** Conectado à rede sem fio (Wi-Fi).

---

## Passo a Passo do que foi feito

### 1. Configurando o PC de Mesa (Conexão via Cabo)
Para o computador funcionar na rede, ele precisa de um "endereço" exclusivo, chamado **Endereço IP**. 

Ativei a opção **DHCP**, que faz com que o roteador entregue esse endereço automaticamente para o computador, sem precisarmos digitar nada manualmente.

<img width="702" height="670" alt="Configuração PC" src="https://github.com/user-attachments/assets/9b5aa8cd-b13c-4e5a-96e3-b3b694200b1f" />

---
* **Conferindo o IP recebido pelo PC:**

<img width="702" height="672" alt="IPConfig PC" src="https://github.com/user-attachments/assets/da3c568c-a23e-4eb0-946c-6cd60a2c514c" />


---

### 2. Configurando o Notebook (Conexão via Wi-Fi)
Os notebooks no simulador vêm de fábrica apenas com entrada para cabo. Para conectar via Wi-Fi, fiz a troca da placa de rede:

1. Desliguei o notebook virtual.
2. Removi a placa de cabo e encaixei a placa de Wi-Fi (**WPC300N**).
3. Religuei o notebook e conectei à rede sem fio chamada `HomeNetwork`.

* **Conferindo as configurações de rede do Notebook:**

<img width="692" height="671" alt="Configuração Laptop" src="https://github.com/user-attachments/assets/7a55863f-360a-4a16-8ed4-cf1ce5f2d7b0" />

---

<img width="696" height="673" alt="DHCP Laptop" src="https://github.com/user-attachments/assets/d775765f-60ce-474c-a6b7-d5c0b5caef02" />

--- 
* **Conferindo o IP recebido pelo PC:**

<img width="689" height="671" alt="Ipconfig laptop" src="https://github.com/user-attachments/assets/31aa54b7-7ac8-4d2b-b37f-4684d3e05abc" />

---

## Ferramentas e Conceitos Aprendidos

* **Cisco Packet Tracer:** Software de simulação de redes.
* **DHCP:** O "distribuidor" automático de endereços de internet da rede.
* **IP:** O "RG" de cada aparelho conectado na rede.
* **Cabo de Rede vs. Wi-Fi:** Como configurar e alternar entre conexões físicas e sem fio.
* **Comando `ipconfig`:** Usado no terminal para descobrir o endereço IP do próprio computador.

> **Nota de Isenção e Atribuição:**
> Este repositório contém resoluções pessoais, anotações e configurações desenvolvidas por mim para fins de estudo e demonstração prática de habilidades. 
> O exercício original faz parte do currículo da **Cisco Networking Academy (NetAcad)** (*Atividade: Criando uma Rede Simples*). 
> Todos os direitos sobre conceitos e marcas registradas pertencem à Cisco Systems, Inc. Nenhum material proprietário ou protegido por direitos autorais da plataforma é redistribuído aqui.
