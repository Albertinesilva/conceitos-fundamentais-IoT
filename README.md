<h1 align="center">🔗 Tópicos Avançado em Redes </h1>

<h2>Relatório Técnico: Conceitos Fundamentais de IoT</h2>

**Introdução**

A `Internet das Coisas (IoT)` tem se tornado uma das tecnologias mais transformadoras da atualidade, conectando dispositivos físicos à internet para permitir a `coleta e troca de dados em tempo real.` Este relatório tem como objetivo explorar os `conceitos fundamentais da IoT,` desde sua arquitetura básica até os protocolos de comunicação, segurança, hardware e computação distribuída, com exemplos práticos que ilustram sua aplicação no mundo real.

**1. Conceitos Fundamentais de IoT**
   
A `Internet das Coisas (IoT)` é basicamente a conexão de um monte de dispositivos físicos que conseguem coletar e trocar dados entre si por meio de uma rede. Esses dispositivos podem ser desde `sensores industriais supercomplexos até aqueles` `gadgets` `domésticos` que a gente usa no dia a dia, como lâmpadas inteligentes ou assistentes virtuais (KRANZ, 2016).

A ideia central da IoT é que esses dispositivos coletam `informações do ambiente` (como temperatura, umidade, movimento, etc.) e mandam esses dados para um `sistema central`, que pode ser na `nuvem.` Lá, esses dados são processados e usados para tomar decisões ou até mesmo acionar `ações automáticas`, como ligar um ar-condicionado ou ajustar a iluminação de uma casa (BUYYA; DASTJERDI, 2016).

A importância da IoT hoje em dia é enorme, porque ela `traz eficiência, automação e inovação` pra vários setores. Por exemplo, na `saúde`, ela pode ajudar a monitorar pacientes remotamente; na `agricultura`, otimiza o uso de água e fertilizantes; e nas `cidades inteligentes`, melhora o trânsito e o uso de energia (KRANZ, 2016).

A arquitetura de um sistema IoT geralmente tem quatro partes principais: os `dispositivos` (como sensores e atuadores), os `gateways` (que fazem a ponte entre os dispositivos e a nuvem), a `nuvem` (onde os dados são armazenados e processados) e as `aplicações` (que são as interfaces que a gente usa, como apps ou painéis de controle) (BUYYA; DASTJERDI, 2016).

Um exemplo bem prático de IoT é o `monitoramento de tráfego em cidades` `inteligentes`. Sensores instalados nas ruas coletam informações sobre o fluxo de carros e mandam esses dados pra nuvem. Lá, eles são processados e exibidos em tempo real num `painel de controle`, permitindo que os gestores de trânsito tomem decisões rápidas pra evitar congestionamentos e melhorar o fluxo de veículos (KRANZ, 2016).

**2. Protocolos de Comunicação para IoT**
   
Os `protocolos de comunicação` são superimportantes pra garantir que os dispositivos IoT consigam trocar dados de forma eficiente. Dois dos mais famosos são o `MQTT` e o `CoAP.` O `MQTT` (Message Queuing Telemetry Transport) é baseado num modelo de `publicação/assinatura` (publish/subscribe), o que o torna leve e perfeito pra redes que não são muito estáveis. Já o `CoAP` (Constrained Application Protocol) é baseado no `REST` e foi feito pra dispositivos com poucos recursos, como sensores que funcionam com bateria e precisam economizar energia (BUYYA; DASTJERDI, 2016).

Um exemplo clássico de uso do `MQTT` é o `monitoramento remoto de equipamentos industriais`, onde a comunicação precisa ser rápida e confiável. Já o `CoAP` é mais usado em `automação residencial`, tipo aqueles sistemas de casa inteligente, onde os dispositivos precisam se comunicar sem gastar muita energia (KING, 2020).

Pra você ter uma ideia de como o `MQTT` funciona, dá pra fazer um experimento bem simples usando um `broker MQTT`, como o Mosquitto, pra enviar dados de temperatura de um sensor (tipo um NodeMCU) pra um `painel de controle no Node-RED`. Isso mostra como o MQTT é bom pra `comunicação em tempo real` entre dispositivos IoT (BUYYA; DASTJERDI, 2016).

Além desses dois, tem outros protocolos que também são bem importantes, como o `AMQP` (Advanced Message Queuing Protocol) e o `LoRaWAN` (Long Range Wide Area Network). O `AMQP` é mais robusto e é muito usado em `sistemas empresariais`, enquanto o `LoRaWAN` foi feito pra `comunicação de longo alcance` e `baixo consumo de energia`, o que é perfeito pra áreas rurais ou remotas. Por exemplo, o LoRaWAN permite que sensores em fazendas ou florestas se comuniquem a distâncias de até `15 km`, sem gastar muita energia (KING, 2020).


