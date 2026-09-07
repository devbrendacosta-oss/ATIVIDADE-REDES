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

3. Critérios de Avaliação e Testes
Para concluir o laboratório com sucesso, o aluno deve demonstrar o funcionamento executando:

3.1 Validação do DHCP: Alterar a configuração de IP de cada um dos 5 PCs de Static para DHCP e comprovar que receberam os endereços automaticamente a partir de 192.168.1.100

3.2 Teste de Conectividade (Ping): Abrir o Command Prompt em pelo menos dois computadores e testar a comunicação com o servidor:
Bash
ping 192.168.1.10
(O retorno deve apresentar pacotes enviados com sucesso e 0% de perda).

<img width="913" height="523" alt="Captura de tela 2026-09-07 185741" src="https://github.com/user-attachments/assets/6ae950e2-783a-4246-9e11-4f395e7622d7" />
<img width="909" height="534" alt="Captura de tela 2026-09-07 185700" src="https://github.com/user-attachments/assets/a6bc58d5-a1df-4115-b51c-5c5518ad6410" />

3.3 Teste de Envio de PDU: Utilizar a ferramenta de simulação de pacotes (ícone de carta no Packet Tracer) enviando uma mensagem de um PC para o Servidor e verificando o status Successful.

<img width="1365" height="711" alt="Captura de tela 2026-09-07 191359" src="https://github.com/user-attachments/assets/acaa540b-7739-46b9-b48c-28fc091d3fac" />

