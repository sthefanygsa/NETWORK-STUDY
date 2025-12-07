# CCNA: Introduction to Networks

## Módulo 1: As redes hoje

### 1.2. Componentes de Rede

#### 1.2.1 Funções do Host

Para participar de uma comunidade online, teu dispositivo precisa estar numa rede que esteja conectada à internet.

- **Hosts (dispositivos finais)**: 
    - são todos os dispositivos conectados à rede;
    - eles recebem um indereço IP, que é o número usado para identificar cada um na rede;
    - podem incluir computadores, celulares, tablets etc.
- **Servidores**: são computadores especiais com softwares que fornecem serviços, como:
    - e-mail;
    - páginas web;
    - arquivos.
- **Clientes**: também são hosts, mas com programas voltados para pedir e exibir informações vindas do servidor (navegador pedindo uma página da web).

- **Software cliente**: é o programa que pede informações ao servidor.
    Exemplo: navegador (Chrome, Firefox).
- **Um mesmo computador pode rodar vários clientes ao mesmo tempo, tipo:**
    - chechar e-mail;
    - abrir um site;
    - mandar mensagem;
    - ouvir música online.
- **Tipos de servidores**
    - **Servidor de e-mail**:
    - roda um software específico pra guardar e enviar e-mails;
    - o cliente usa um app de e-mail (tipo outlook) para acessar as mensagens.
- **Servidor Web**
    - Roda o software que entrega páginas web;
    - O cliente usa um navegador (Chrome, Firefox, Edge) para acessar os sites.
- **Servidor de Arquivos**
    - Guarda arquivos corporativos ou pessoais num único lugar;
    - Os clientes acessam usando programas como o Explorador de Arquivos do Windows.

#### 1.2.2 Ponto a Ponto

- Cliente e servidor normalmente estão em computadores diferentes, mas podem estar no mesmo também.
- Em casas e pequenas empresas, é comum um computador ser cliente e servidor ao mesmo tempo.
- Quando todos os dispositivos compartilham recursos entre si desse jeito, isso se chama rede ponto a ponto (P2P).

- **Vantagens**:
    - fácil de configurar;
    - simples de mexer;
    - barata (não precisa de servidor dedicado);
    - boa para tarefas básicas: compartilhar arquivos e impressoras.

- **Desvantagens**:
    - sem administração central;
    - menos segura;
    - não escala bem (ruim para redes grandes);
    - como todos podem ser cliente e servidor, o desempenho pode cair.

#### 1.2.3 Dispositivos Finais

- Os dispositivos finais (computadores, celulares, tablets, impressoras etc.) são os que a gente mais conhece numa rede.
- Cada dispositivo final tem um endereço próprio -> é assim que a rede sabe quem é quem.
- Quando um dispositivo quer enviar algo, ele usa o endereço do destino para dizer "entrega isso para esse aqui".
- Um dispositivo final pode ser:
    - Origem da mensagem (quem envia);
    - Destino da mensagem (quem recebe).

#### 1.2.4 Dispositivos Intermediários

- Dispositivos intermediários são os que ligam os dispositivos finais entre si e também conectam várias redes diferentes.
- Eles garantem que os dados circulem direitinho pela rede.
- Pra encaminhar as mensagens, eles usam:
    - o endereço do dispositivo final de destino
    - e as informações de como as redes estão conectadas
- Com isso, eles decidem qual caminho a mensagem vai seguir.

- **Exemplos comuns de dispositivos intermediários**:
    - Roteadores;
    - Switches;
    - Firewall;
    - Pontos de acesso (APs).

- **Funções dos dispositivos intermediários**:
    - Regenerar e retransmitir sinais (impedir que o sinal “morra” no caminho);
    - Manter informações de rotas pela rede e entre redes
    - Avisar outros dispositivos quando rola erro ou falha;
    - Escolher rotas alternativas quando um link cai;
    - Classificar e priorizar mensagens;
    - Permitir ou bloquear tráfego, seguindo regras de segurança.

- **Observação importante**:
    - Um hub Ethernet (mais antigo) é basicamente um repetidor multiporta;
    - Ele só regenera e repassa sinais, sem inteligência;
    - E sim:todos os dispositivos intermediários fazem pelo menos a função de repetidor.

#### 1.2.4 Dispositivos Intermediários

- **O que é mídia de rede?**:
    - É o meio físico (ou não físico, no caso do wireless) por onde a mensagem viaja do ponto A até o ponto B.

- **Tipo de mídia (os 3 principais)**:
    1. Cabos de metal (par trançado, coaxial...):
        - Dados viram impulsos elétricos;
        - É o tipo mais comum em casas e empresas.
    2. Fibra Óptica:
        - Dados viram pulsos de luz;
        - Mais rápida e resistente a interferências.
    3. Sem fio (Wi-Fi, rádio, celular):
        - Dados transmitidos por ondas eletromagnéticas;
        - Sem cabo, mais prático, mas mais sujeito a interferências.

### 1.3. Representações e topologias de rede

#### 1.3.1 Representações de Rede

- Arquitetos e admins de rede precisam planejar e visualizar como a rede vai ser.
- Eles têm que ver quais dispositivos se conectam, onde ficam e como são ligados.
- Pra isso se usam diagramas de rede, que representam tudo de forma clara.
- Esses diagramas usam símbolos específicos (roteador, switch, servidor, cabo, nuvem etc.) pra identificar cada tipo de dispositivo e conexão.

- **Meios de Rede**:
    - Meios sem fio;
    - Mídia LAN;
    - Mídia WAN.

- **Diagrama de topologia**:
    - É tipo uma foto da rede, mostrando como tudo está conectado.
    - Ajuda a entender a organização e o funcionamento da rede, mesmo quando é grande.
    - Saber interpretar esses desenhos é essencial pra quem trabalha com redes.

- **Termos importantes**:
    - NIC (Placa de Interface de Rede):
        - É a peça que liga fisicamente o dispositivo final à rede.
        - Tipo a plaquinha do PC que conecta o cabo de rede ou o Wi-Fi.
    - Porta física:
        - É o buraquinho onde você conecta o cabo (RJ-45, fibra, USB, etc).
        - Pode ser porta de um computador, switch, roteador…
    - Interface:
        - Em dispositivos de rede (principalmente roteadores), as portas são chamadas de interfaces de rede.
        - Cada interface conecta o roteador a uma rede diferente.

- **Obervação**:
    - Na prática, porta e interface são quase sempre usados como sinônimos.

#### 1.3.2 Diagramas de Topologia

- **Tipos de diagramas de topologia**:
    Os diagramas são obrigatórios pra quem trabalha com redes, porque mostram como tudo está conectado.

Existem dois tipos:

- **Topologia Física**:
    - Mostra onde cada dispositivo está fisicamente (salas, racks, prédio…).
    - Mostra os cabos, por onde passam, e como estão instalados.
    - É tipo um mapa real da infraestrutura.
- **Topologia Lógica**:
    - Mostra como a rede funciona, não onde os equipamentos estão fisicamente.
    - Foca em endereços IP, sub-redes, roteamento, fluxo de dados e como os dispositivos se comunicam.
    - É tipo a visão “mental” da rede, mostrando quem fala com quem e por quais caminhos.
- **Diagrama de topologia lógica**:
    - Mostra como a rede funciona, não onde os equipamentos estão no espaço.
    - Inclui:
        - Dispositivos (PCs, switches, roteadores…)
        - Portas/interfaces
        - Esquema de endereçamento (IPs, sub-redes)
        - Tipo de mídia usada (cabo, fibra, wireless)
    - Dá pra ver quem está conectado a quem e como os dados circulam.

- **Observação**:
    - Os diagramas de topologia lógica e física que você está vendo agora são versões simplificadas, perfeitas pro estágio do curso.
    - Se pesquisar “diagramas de topologia de rede” na internet, vai ver modelos bem mais complexos.
    - Se pesquisar “diagramas de topologia de rede cisco”, você encontra vários usando os mesmos ícones que aparecem no material.

### 1.4. Tipos comuns de redes

#### 1.4.1 Redes de Vários Tamanhos

- **Tipos de redes (visão geral)**:
    - As redes existem em todos os tamanhos, desde 2 computadores até milhões de dispositivos interligados.
- **Redes domésticas**:
    - Simples e pequenas;
    - Servem para compartilhar impressora, arquivos, fotos, músicas entre dispositivos da casa.
- **Redes SOHO (Small Office/Home Office)**:
    - Usadas em casas ou pequenos escritórios;
    - Permitem trabalhar de casa, vender produtos, pedir materiais e falar com clientes;
    - Muito usadas por autônomos/freelancers.
    - Se conectam a uma rede corporativa, ou acessam recursos compartilhados centralizados.
- **Redes de empresas/organizações (médias a grandes)**:
    - Ajudam a guardar e organizar informações em servidores;
    - Oferecem e-mail, chat, colaboração, sistemas internos, etc;
    - Usam a internet para entregar prosutos e serviços aos clientes.
- **Rede Mundial (Internet)**:
    - É a maior rede do mundo;
    - Chamados de "rede de redes" porque conecta milhares de redes públicas e privadas.
- **Rede ponto a ponto (P2P)**:
    - Comum em casas e pequenas empresas;
    - Cada computador pode ser cliente e servidor ao mesmo tempo;
    - Boa para coisas simples, como compartilhar arquivos.

#### 1.4.2 LANs e WANs

- **Como as infraestruturas de rede podem variar**:
    Elas mudam conforme:
        - Área coberta (pequena ou gigante);
        - Quantidade de usuários;
        - Quantidade/tipo de serviços (e-mail, arquivos, internet, sistemas...);
        - Quem é responsável pela rede (empresa, provedor, usuário).

- **Tipos principais de infraestrutura**:
    - LAN (Local Area Network)
        - Rede local, área pequena;
        - Usada em casas, pequenos escritórios, salas, departamentos, prédios, campus pequeno;
        - Normalmente administrada por uma pessoa ou organização;
        - Conecta dispositivos próximos com alta velocidade.

    - WAN (Wide Area Network)
        - Rede de longa distância, área bem maior;
        - Conecta várias LANs entre si - pode ligar cidades, estados, países;
        - Geralmente gerenciado por grandes empresas, provedores de internet ou telecom;
        - Normalmente oferece velocidade menor que a LAN por causa das grandes distâncias.
    Exemplo: Sua casa = LAN -> conecta ao provedor -> WAN (internet)

#### 1.4.3 A Internet

- **Internet - Visão Geral**:
    - A internet é uma coleção mundial de redes interconectadas;
    - Ela é formada por LANs + WANs todas ligadas entre si;
    - Uma LAN pode se conectar a outra através de uma WAN, e várias WANs também se conectam entre si;
    - Essas conexões podem usar:
        - cobre
        - fibra óptica
        - transmissões sem fio
- **Quem "possui" a Internet?**:
    - Ninguém. A Internet não tem dono;
    - Como ela é enorme e global, é preciso usar protocolos e tecnologia padronizadas para tudo funcionar direitinho.
- **Quem organiza e padroniza a Internet?**:
    - IETF — cria e mantém padrões técnicos (ex: protocolos).
    - ICANN — cuida de domínios, DNS e endereços IP.
    - IAB — supervisiona a arquitetura geral da Internet.

#### 1.4.4 Intranets e Extranets

- **Internet, Intranet e Extranet**:
    - A internet é um mundão de redes interligadas — várias LANs e WANs conectadas entre si.
    Nenhuma pessoa ou empresa “dona”; tudo funciona porque existem padrões e protocolos definidos por organizações como IETF, ICANN e IAB.
- **Intranet**:
    - É tipo uma “internet particular” de uma empresa.
    Conecta as LANs e WANs internas só pra quem trabalha lá ou tem permissão.
Ex: funcionários acessando sistemas internos, documentos, servidores da empresa.
- **Extranet**:
    - É uma parte da intranet que a empresa abre com segurança para pessoas de fora que precisam acessar algo.
Exemplos:
    - fornecedores acessando pedidos da empresa
    - médicos acessando o sistema do hospital
    - escolas vendo dados do órgão de educação

### 1.5. Conexões com a Internet

#### 1.5.1 Tecnologias de Acesso à Internet

- **Como as pessoas se conectam à Internet**:
    - Pra quem é usuário comum (casa, home office, escritório pequeno), normalmente precisa assinar um ISP (tipo Vivo, Claro, Tim, etc).
        - Cabo (banda larga): internet via cabo coaxial, bem comum;
        - DSL: internet que usa o fio do telefone fixo;
        - Wi-Fi de longa distância: aquelas antenas que o provedor coloca em lugares pequenos;
        - 4G/5G: celular roteando ou modemzinho com chip.

- **Como as empresas se conectam**:
    - Empresas precisam de algo mais rápido, mais estável e que aguente muita gente usando ao mesmo tempo.
    Por isso elas usam conexões “de nível empresarial”, tipo:
        - DSL empresarial (não é igual o doméstico, é mais robusto)
        - Linhas dedicadas (link exclusivo só pra empresa, muito estável)
        - Metro Ethernet (uma internet de alta velocidade usando fibra, comum em empresas grandes).
    - Essas conexões precisam suportar:
        - telefone IP
        - videoconferências
        - acesso a data center
        - sistemas internos

#### 1.5.2 Conexões com a Internet para Residências e Pequenos Escritórios

- **Tipos de conexão à internet (bem resumido)**:
    1. Cabo
        - Usa o mesmo cabo da TV a cabo.
        - Rápida, estável e fica conectada o tempo todo.

    2. DSL (ADSL)
        - Usa linha telefônica.
        - Também fica sempre conectada.
        - No ADSL: download > upload (por isso “assimétrico”).
        - Muito usada em casas e pequenos escritórios.
    
    3. Celular (4G/5G)
        - 