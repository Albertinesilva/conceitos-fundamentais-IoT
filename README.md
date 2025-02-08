<h1 align="center">🔗 Tópicos Avançado em Redes </h1>

<h2>Relatório Técnico: Conceitos Fundamentais de IoT</h2>

**Introdução**

A `Internet das Coisas (IoT)` tem sido uma das tecnologias mais significativas do tempo, conectando dispositivos físicos à internet para `coleta e troca de dados em tempo real.` Este relatório visa examinar os `conceitos básicos do IoT`, a partir de sua arquitetura básica para protocolo de comunicação, segurança, hardware computação e material abrangido distribuído com exemplos práticos relacionados à realidade.

**1. Conceitos Fundamentais de IoT**

A ideia por trás disso é empacotar um monte desses `dispositivos` que possam coletar informações do ambiente, eles mandam esses dados para um sistema central, que em geral é um na `nuvem`. Lá, os processa e toma medidas baseadas nisso, como ligar seu ar condicionado a casa, apertar o botão das luzes e coisas do tipo. A importância disso é que ela traz `eficiência`, `automação` e `inovação` para diversos setores da sociedade. Desde saúde, ao monitorar pacientes, à agricultura, ao otimizar a colheita e o uso de água, desde as cidades inteligentes, transporte a uso de energia. 

A arquitetura de um sistema desse tipo geralmente possui três partes: 

- Os `dispositivos` que são os sensores e atuadores. 

- Os `gateways` que fazem a ponte entre os dispositivos e a `nuvem` da aplicação. 

- A `cloud`, que é onde os dados são armazenados e processados. 

E por fim, mas não menos importante, os `aplicativos`, que são as `interfaces` com as quais interagimos, como o `app no celular` ou `painel de controle` de uma empresa ou dona de casa. 

Um exemplo de aplicação prática disso é a cidade sob monitoramento de trânsito. Sensores nas ruas coletam informações de quantos carros passam e quando e mandam isso pra nuvem. Lá, esses dados são processados, e atualizados em tempo real em um painel de controle para uma autoridade de trânsito decidir quem para onde e quando para evitar congestionamento.

**2. Protocolos de Comunicação para IoT**

Existem dois `protocolos` principais que são utilizados para permitir a comunicação entre dispositivos IoT. Esses protocolos são: `MQTT e CoAP`.  

- `MQTT` funciona através de um padrão de `publicação/assinatura` e é um `protocolo` perfeito em caso de redes em constante mudança e má largura de banda de `dispositivos`. 
- `CoAP` é um protocolo de `roteamento` baseado em `REST` criado especificamente para dispositivos com falta de energia e processamento.

**Casos de Uso:**

`MQTT` : monitoramento `remoto` de `equipamentos industriais`, já que a comunicação é essencialmente em tempo real e precisa ser confiável.
 CoAP` : automação residencial, para contornar problemas de uso de energia especialmente com a Internet das Coisas. Quando um interruptor inteligente liga ou desliga as luzes, é necessário que a rede capte instantaneamente o movimento. 

**Experimento simples:**

Configurar um `broker MQTT` (como o Mosquitto), para conduzir dados de temperatura de um sensor (como um NodeMCU), para ser exibido em um painel de controle dentro do `Node-RED`. Isso criará uma demonstração das capacidades de tempo real dos protocolos de IoT.

**AMQP e LoRaWAN**

Os protocolos `AMQP` e `LoRaWAN` são utilizados em cenários específicos de IoT:
- AMQP (Advanced Message Queuing Protocol) Utilizado em sistemas empresariais, oferece segurança e confiabilidade na troca de mensagens.
- LoRaWAN (Long Range Wide Area Network) é uma comunicação de longo alcance, tem baixo consumo de energia, ideal para aplicações agrícolas e monitoramento remoto

**Comparação e Aplicação**

O `AMQP` é mais robusto. Usado em ambientes corporativos em que a segurança da informação é importante. 
O `LoRaWAN`, por outro lado, permite que sensores em áreas rurais transmitam dados a distâncias de até 15 km, sem a necessidade de uma potência de transmissão alta, tornando-o mais flexível

**3. Segurança e Padronização em IoT**

A segurança é um dos maiores desafios da IoT, pois os dispositivos conectados podem se tornar vulneráveis a ataques cibernéticos. Os principais problemas da IoT em relação à segurança incluem:
- Falta de criptografia durante a transferência de dados.

- Dispositivos desatualizados acessíveis para ataques.

- Ataques DDoS que se aproveitam da rede dos dispositivos IoT.

**Boas práticas para prevenir**
- Implementação de criptografia de ponta a ponta.
- Atualizações frequentes de firmware e software dos dispositivos.
- Uso de autenticação forte para acesso aos dispositivos.

**Exemplo de Ataque Real**
Em 2016, o ataque Mirai Botnet explorou dispositivos IoT vulneráveis e criou uma botnet massiva para derrubar grandes servidores da internet.

**Interoperabilidade e Padrões API**
A interoperabilidade na IoT significa que diferentes dispositivos são capazes de se comunicar uns com os outros, independentemente do fabricante.

**APIs Padronizadas**
As APIs padronizadas é essencial para integrar entre dispositivos IoT e serviços que ficam na nuvem. Existem três APIs amplamente usadas:
- RESTful APIs – Baseado em HTTP e fácil de integrar e escaláveis.
- WebSockets – Permite a comunicação bidirecional em tempo real.
- OPC UA (Open Platform Communications Unified Architecture) é amplamente usada na indústria para padronizar a comunicação entre máquinas.

**4. Hardware e Computação Distribuída**

**Hardware IoT: Sensores e Atuadores**
   



