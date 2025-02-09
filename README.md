<h1 align="center">🌐 Tópicos Avançados em Redes de Computadores (IOT) </h1>

## 📌 Objetivo da Atividade:

Aprofundar o entendimento sobre os principais conceitos da `IoT`, desde sua arquitetura e `protocolos` de comunicação até questões de segurança, hardware e computação em borda.

<h2 align="center">📄 Relatório Técnico: Conceitos Fundamentais de IoT</h2>

📝**Introdução**

Nos últimos anos, a Internet das Coisas (IoT) se tornou uma das tecnologias mais importantes do século XXI. Agora, podemos conectar objetos do cotidiano — como eletrodomésticos, carros, termostatos e babás eletrônicas — à Internet por meio de dispositivos incorporados, possibilitando uma comunicação perfeita entre pessoas, processos e outras coisas. Por meio da computação de baixo custo, nuvem, big data, análise avançada e tecnologias móveis, coisas físicas podem compartilhar e coletar dados com o mínimo de intervenção humana. Nesse mundo hiperconectado, os sistemas digitais podem gravar, monitorar e ajustar cada interação entre itens conectados, unindo o mundo físico ao digital e fazendo-os trabalhar em conjunto [(ORACLE, 2025)](https://www.oracle.com/br/internet-of-things/).

Este relatório revela os fundamentos da IoT, desde a arquitetura básica até o protocolo de comunicação, segurança, desempenho e o conteúdo abordado, com exemplos práticos relacionados à realidade. a IoT não é apenas uma questão de tornar os dispositivos mais inteligentes. Acima de tudo, isso diz respeito ao processo onde ocorre permuta de informações, ocorrendo-a muito mais rapidamente. Além disso, isso muda completamente a maneira como interagimos com o mundo.

💡**1. Conceitos Fundamentais de IoT**

A Internet das Coisas (IoT) descreve a rede de objetos físicos incorporados a sensores, software e outras tecnologias com o objetivo de conectar e trocar dados com outros dispositivos e sistemas pela internet. Esses dispositivos variam de objetos domésticos comuns a ferramentas industriais sofisticadas [(ORACLE, 2025)](https://www.oracle.com/br/internet-of-things/).

A ideia por trás disso é empacotar um monte desses `dispositivos` que possam coletar informações do ambiente, eles mandam esses dados para um sistema central, que em geral é na `nuvem`. Lá, os processa e toma medidas baseadas nisso, como ligar seu ar condicionado a casa, apertar o botão das luzes e coisas do tipo. A importância disso é que ela traz `eficiência`, `automação` e `inovação` para diversos setores da sociedade. Desde saúde, ao monitorar pacientes, à agricultura, ao otimizar a colheita e o uso de água, desde as cidades inteligentes, transporte a uso de energia. 

A `arquitetura` de um sistema desse tipo geralmente possui três partes: 

- Os `dispositivos` que são os sensores e atuadores. 

- Os `gateways` que fazem a ponte entre os dispositivos e a `nuvem` da aplicação. 

- A `cloud`, que é onde os dados são armazenados e processados. 

E por fim, mas não menos importante, os `aplicativos`, que são as `interfaces` com as quais interagimos, como o `app no celular` ou `painel de controle` de uma empresa ou dona de casa. 

Um exemplo de aplicação prática disso é a cidade sob monitoramento de trânsito. `Sensores` nas ruas coletam informações de quantos carros passam e quando e mandam isso pra `nuvem`. Lá, esses dados são processados, e atualizados em tempo real em um painel de controle para uma autoridade de trânsito decidir quem para onde e quando para evitar congestionamento.

🔗**2. Protocolos de Comunicação para IoT**

Existem dois `protocolos` principais que são utilizados para permitir a comunicação entre dispositivos `IoT`. Esses protocolos são: `MQTT e CoAP`.  

- `MQTT` funciona através de um padrão de `publicação/assinatura` e é um `protocolo` perfeito em caso de redes em constante mudança e má largura de banda de `dispositivos`. 
- `CoAP` é um protocolo de `roteamento` baseado em `REST` criado especificamente para dispositivos com falta de energia e processamento.

📋**Casos de Uso:**

`MQTT` : monitoramento `remoto` de `equipamentos industriais`, já que a comunicação é essencialmente em tempo real e precisa ser confiável.
`CoAP` : automação residencial, para contornar problemas de uso de energia especialmente com a Internet das Coisas. Quando um interruptor inteligente liga ou desliga as luzes, é necessário que a rede capte instantaneamente o movimento. 

🔬**Experimento simples:**

Configurar um `broker MQTT` (como o Mosquitto), para conduzir dados de temperatura de um sensor (como um NodeMCU), para ser exibido em um painel de controle dentro do `Node-RED`. Isso criará uma demonstração das capacidades de tempo real dos protocolos de IoT.

📶**AMQP e LoRaWAN**

Os protocolos `AMQP` e `LoRaWAN` são utilizados em cenários específicos de IoT:

- `AMQP` (Advanced Message Queuing Protocol) Utilizado em sistemas empresariais, oferece segurança e confiabilidade na troca de mensagens.
 
- `LoRaWAN` (Long Range Wide Area Network) é uma comunicação de longo alcance, tem baixo consumo de energia, ideal para aplicações agrícolas e monitoramento remoto

⚖️**Comparação e Aplicação**

O `AMQP` é mais robusto. Usado em ambientes corporativos em que a `segurança da informação` é importante. 
O `LoRaWAN`, por outro lado, permite que `sensores` em áreas rurais transmitam dados a distâncias de até 15 km, sem a necessidade de uma potência de transmissão alta, tornando-o mais flexível

🔒**3. Segurança e Padronização em IoT**

A segurança é um dos maiores desafios da `IoT`, pois os dispositivos conectados podem se tornar vulneráveis a ataques `cibernéticos`. Os principais problemas da `IoT` em relação à segurança incluem:

- Falta de `criptografia` durante a transferência de dados.

- `Dispositivos` desatualizados acessíveis para ataques.

- Ataques `DDoS` que se aproveitam da rede dos dispositivos `IoT`.

👍**Boas práticas para prevenir**
- Implementação de `criptografia` de ponta a ponta.
- Atualizações frequentes de `firmware` e `software` dos dispositivos.
- Uso de `autenticação` forte para acesso aos dispositivos.

🧑‍💻**Exemplo de Ataque Real**
Em 2016, o ataque `Mirai Botnet` explorou dispositivos `IoT` vulneráveis e criou uma `botnet` massiva para derrubar grandes `servidores` da internet.

📡**Interoperabilidade e Padrões API**
A interoperabilidade na IoT significa que diferentes dispositivos são capazes de se comunicar uns com os outros, independentemente do fabricante.

📡**APIs Padronizadas**
As `APIs` padronizadas é essencial para integrar entre `dispositivos IoT` e serviços que ficam na `nuvem`. Existem três `APIs` amplamente usadas:
- `RESTful APIs` – Baseado em `HTTP` e fácil de integrar e escaláveis.
- `WebSockets` – Permite a comunicação `bidirecional` em `tempo real`.
- `OPC UA` (Open Platform Communications Unified Architecture) é amplamente usada na `indústria` para padronizar a comunicação entre `máquinas`.

💻**4. Hardware e Computação Distribuída**

**Hardware IoT: Sensores e Atuadores**

Os `sensores` e atuadores são componentes fundamentais da `IoT`:

- `Sensores` que adquirem dados do ambiente, como temperatura, umidade e sensores de movimento.
- `Atuadores` que realizam ações a partir dados dos sensores, como motores elétricos, relés de controle.

**Exemplo de Sensor**

O `DHT11` é um dos sensores mais utilizados e simples para medir temperatura e umidade em aplicações de `automação residencial` e `sistemas agrícolas`.

🌐**Redes de Sensores Sem Fio (WSN)**

- As `WSN` conectam vários sensores à rede para permitir monitoramento em grande escala.

🌾**Aplicação na Agricultura Inteligente**

- Os `sensores` colocados nas plantações medem a umidade do solo e o nível de nutrientes e enviam os dados para a `nuvem` para `análise` e automaticamente acionar o sistema de irrigação

🧗‍♂️**Desafios de Implementação**
- `Consumo de energia` – Dispositivos devem operar com bateria por períodos longos.
- `Interferência de transmissão` – os locais ao ar livre podem interferir na transmissão.
- `Segurança de dados` – as informações devem ser protegidas contra acessos não autorizados.

**Edge Computing e sua Relação com IoT**

O `Edge Computing` processa `dados` localmente, reduzindo a necessidade de enviar grandes quantidades de informações para a `nuvem`.

**Vantagens e Desvantagens**

✅ **Vantagens:**

- `Baixa latência` – Respostas mais rápidas em `aplicações` críticas.
- `Menor consumo` de largura de banda – Reduz o tráfego de dados para a `nuvem`.
- `Maior privacidade` – Dados sensíveis podem ser processados localmente.

❌ **Desvantagens:**

- `Capacidade limitada de processamento` – Dispositivos podem ter menos poder computacional.
- `Maior complexidade na manutenção` – Necessidade de atualizações locais frequentes.

**Edge Computing na Segurança e Eficiência da IoT**

- Em `aplicações industriais`, o `Edge Computing` pode processar dados de `sensores` localmente e acionar alertas imediatos em caso de falhas, sem depender da `nuvem`, aumentando a segurança operacional.

**Conclusão:**

Portanto, desde o setor `agrícola` até as cidades inteligentes, o `IoT` é uma tecnologia  impactante para os negócios e países. Para concluir, descrevi os quatro principais conceitos, a arquitetura do `IoT`, os protocolos de comunicação, os problemas de segurança e o hardware. E comparado com exemplos de aplicativos para informações detalhadas sobre como o IoT é usado. Por fim, todo o trabalho de implementação do IoT e sua falta de regulamentação.

#### 📌 Autor

👨‍💻 **Albert Silva**


   



