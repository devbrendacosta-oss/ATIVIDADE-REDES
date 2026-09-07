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


<img width="905" height="573" alt="Captura de tela 2026-09-07 193408" src="https://github.com/user-attachments/assets/a56eec14-1da0-4f18-9678-f50764a80fe9" />


3.2 Teste de Conectividade (Ping): Abrir o Command Prompt em pelo menos dois computadores e testar a comunicação com o servidor:
Bash
ping 192.168.1.10
(O retorno deve apresentar pacotes enviados com sucesso e 0% de perda).


<img width="565" height="653" alt="Captura de tela 2026-09-07 193551" src="https://github.com/user-attachments/assets/4892c202-a894-4a45-9045-92a93505211e" />


3.3 Teste de Envio de PDU: Utilizar a ferramenta de simulação de pacotes (ícone de carta no Packet Tracer) enviando uma mensagem de um PC para o Servidor e verificando o status Successful.


<img width="1365" height="711" alt="Captura de tela 2026-09-07 191359" src="https://github.com/user-attachments/assets/acaa540b-7739-46b9-b48c-28fc091d3fac" />

