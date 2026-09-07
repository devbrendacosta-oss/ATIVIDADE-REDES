# ATIVIDADE-REDES
Atividade Prática: Configuração de Rede Local com Servidor DHCP (Topologia em Estrela)

 1. Objetivo da Atividade
Montar, configurar e validar uma rede local básica no Cisco Packet Tracer, implementando um servidor de endereçamento dinâmico (DHCP) para automação de IPs e testando a comunicação entre estações de trabalho e o servidor central.

 2. Materiais e Topologia
Cada aluno deverá abrir o Cisco Packet Tracer e montar a seguinte estrutura:

1x Switch (Modelo 2960)

1x Servidor (Server-PT)

5x Computadores (PC-PT)

Cabeamento: Cabos diretos (Copper Straight-Through) conectando cada dispositivo a uma porta livre do Switch central.

 3. Plano de Endereçamento e Configuração
Os alunos devem seguir rigorosamente a distribuição de endereços abaixo para evitar conflitos na rede:

Dispositivo	Função na Rede	Endereço IP (IPv4)	Máscara de Sub-rede	Tipo de Configuração
Servidor	Central / Servidor DHCP	192.168.1.10	255.255.255.0	Estático (Fixo)
PC 1	Estação de Trabalho	192.168.1.100 (Exemplo)	255.255.255.0	Dinâmico (Via DHCP)
PC 2	Estação de Trabalho	192.168.1.101 (Exemplo)	255.255.255.0	Dinâmico (Via DHCP)
PC 3	Estação de Trabalho	192.168.1.102 (Exemplo)	255.255.255.0	Dinâmico (Via DHCP)
PC 4	Estação de Trabalho	192.168.1.103 (Exemplo)	255.255.255.0	Dinâmico (Via DHCP)
PC 5	Estação de Trabalho	192.168.1.104 (Exemplo)	255.255.255.0	Dinâmico (Via DHCP)
Parâmetros do Serviço DHCP (Configurado no Servidor):
Status: On

Default Gateway: 0.0.0.0

Start IP Address: 192.168.1.100

Subnet Mask: 255.255.255.0

Maximum number of users: 50 (Não esquecer de clicar em Save/Add)

 4. Critérios de Avaliação e Testes
Para concluir o laboratório com sucesso, o aluno deve demonstrar o funcionamento executando:

Validação do DHCP: Alterar a configuração de IP de cada um dos 5 PCs de Static para DHCP e comprovar que receberam os endereços automaticamente a partir de 192.168.1.100.

Teste de Conectividade (Ping): Abrir o Command Prompt em pelo menos dois computadores e testar a comunicação com o servidor:

Bash

ping 192.168.1.10
(O retorno deve apresentar pacotes enviados com sucesso e 0% de perda).

Teste de Envio de PDU: Utilizar a ferramenta de simulação de pacotes (ícone de carta no Packet Tracer) enviando uma mensagem de um PC para o Servidor e verificando o status Successful.
