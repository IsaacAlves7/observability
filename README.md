# It's a repository of Observability from scratch 🔍
<img src="https://img.shields.io/badge/Grafana_Stack-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white"> <img src="https://img.shields.io/badge/Datadog-25.3.2-632CA6?style=flat&logo=Datadog&logoColor=white"> <img src="https://img.shields.io/badge/Elastic_Stack-25.3.2-005571?style=flat&logo=Elastic&logoColor=white"> <img src="https://img.shields.io/badge/Graylog-25.3.2-FF3633?style=flat&logo=Graylog&logoColor=white"> <img src="https://img.shields.io/badge/NewRelic-25.3.2-1CE783?style=flat&logo=NewRelic&logoColor=white"> 

<img src="https://em-content.zobj.net/source/microsoft-teams/400/magnifying-glass-tilted-left_1f50d.png" align="right" height="77">

A **observabilidade** (observability) é um conceito fundamental em engenharia de sistemas e DevOps, que se refere à capacidade de entender o que está acontecendo dentro de um sistema complexo através da coleta, agregação e análise de seus dados de desempenho e operação. A ideia central é fornecer visibilidade e insights sobre o estado interno do sistema com base nas saídas externas. 

Observabilidade refere-se à capacidade de monitorar, mensurar e entender o estado de um sistema ou aplicação por meio da análise de seus resultados, logs e métricas de desempenho. Em sistemas de software modernos e na cloud computing, a observabilidade desempenha um papel de extrema importância, por garantir confiabilidade, desempenho e segurança a aplicações e a infraestrutura.

Essa maior importância da observabilidade hoje pode ser atribuída a fatores como: o aumento da complexidade dos sistemas de software, a adoção difundida dos microsserviços e a crescente dependência das arquiteturas distribuídas.

A observabilidade absorve e estende os sistemas de monitoramento clássicos e ajuda as equipes a identificarem a causa raiz dos problemas. Por ela, os stakeholders também esclarecem dúvidas sobre suas aplicações e negócios, como, por exemplo, previsões sobre possíveis erros. Um conjunto diversificado de ferramentas e tecnologias usadas hoje leva a uma grande matriz de possibilidades de implantação. Isso traz consequências arquitetônicas, portanto as equipes precisam saber configurar seus sistemas de observabilidade de maneira que sejam funcionais para elas. 

Observabilidade e monitoramento são conceitos relacionados, mas têm algumas diferenças importantes. A observabilidade refere-se à capacidade de fazer perguntas sobre seu sistema examinando seu comportamento de fora.

À medida que mais organizações adotam a infraestrutura nativa da nuvem, é provável que a necessidade de ferramentas de observabilidade projetadas especificamente para esses ambientes cresça. As ferramentas de observabilidade nativas em nuvem são projetadas para coletar e analisar dados de microsserviços, contêineres e outras tecnologias nativas em nuvem e fornecer insights sobre o desempenho do sistema nesses ambientes.

Em poucas palavras, a observabilidade nativa da nuvem é uma prática de monitoramento, análise e solução de problemas de aplicativos modernos e nativos da nuvem criados usando arquitetura de microsserviços e implantados em contêineres ou ambientes sem servidor. 

A observabilidade baseia-se em três pilares principais:

<img src="https://user-images.githubusercontent.com/61624336/172407209-627822a2-0a5f-4778-b58e-954481ee788b.gif" align="right" height="77">

1. **Logs** (Diagnósticos): Registros detalhados de eventos que ocorrem dentro do sistema. Logs fornecem um histórico cronológico das atividades do sistema e são úteis para diagnosticar problemas específicos, entender a sequência de eventos e rastrear bugs. É todo o diagnóstico preciso dentro do sistema.

2. **Métricas** (Detectar): Dados numéricos que representam o desempenho do sistema. Métricas podem incluir o uso de CPU, memória, taxa de erros, latência de solicitações, entre outros. Elas ajudam a monitorar a saúde do sistema e a identificar tendências ou anomalias. É tudo aquilo que foi detectado no sistema.

3. **Traços** (Isolar e melhorar): Informações sobre a execução de solicitações e transações através de diferentes componentes do sistema. Traços mostram como as solicitações se propagam pelo sistema, permitindo a identificação de gargalos, pontos de falha e a compreensão do fluxo de trabalho completo. Os Traços (Traces) são rastreamentos distribuídos que seguem o caminho de uma solicitação através de vários serviços e componentes de um sistema, ajudam a isolar e melhorar problemas em sistemas distribuídos, permitindo identificar gargalos de desempenho e falhas em componentes específicos. O rastreamento é focado na coleta de dados sobre a execução de solicitações ou transações em seu ambiente e aplicativos Kubernetes. Os rastreamentos podem ajudá-lo a entender como as solicitações ou transações são processadas por seus aplicativos, identificar problemas de desempenho e otimizar o desempenho do aplicativo.

> Além desses três pilares principais, temos os **Eventos** que é focado na coleta de dados sobre eventos importantes que ocorrem em seu ambiente Kubernetes, como implantações de aplicativos, eventos de dimensionamento e erros. Os eventos podem ajudá-lo a monitorar a integridade do seu ambiente Kubernetes e responder rapidamente aos problemas à medida que eles surgem.

Entrando mais a fundo no terceiro pilar da observabilidade, o **rastreamento distribuído** (distributed tracing) é um método usado para criar o perfil ou monitorar o resultado de uma solicitação executada em um sistema distribuído. Monitorar um sistema distribuído pode ser desafiador porque cada ponto central individual tem seu próprio fluxo de logs e de métricas. 

Para obter uma visão precisa de um sistema distribuído, essas métricas de pontos centrais diferentes precisam ser agregadas em uma visão abrangente. As solicitações para sistemas distribuídos, em geral, não acessam todo o conjunto de pontos centrais dentro do sistema, mas acessam um conjunto parcial ou um caminho através dos pontos centrais. O <a href="https://youtu.be/CqLB-tBYB2Q">rastreamento distribuído</a> ilumina os caminhos acessados com frequência por meio de um sistema distribuído e permite que as equipes analisem e monitorem esses caminhos. O rastreamento distribuído é instalado em cada ponto central do sistema e, em seguida, permite que as equipes consultem o sistema para obter informações sobre a integridade do ponto central e o desempenho da solicitação.

- **Revela dependências de serviço**: A decisão estratégica foi tomada: sua empresa começou a migrar para uma arquitetura distribuída, o número de componentes começou a aumentar e a capacidade de entender a arquitetura da organização diminuiu; aplicando o rastreamento distribuído, você pode rastrear o caminho de uma requisição à medida que ela passa por um sistema complexo. Algumas ferramentas até calculam e desenham um grafo de dependência completo. Pode ser útil ter uma visão geral de sua arquitetura e mergulhar profundamente para entender melhor as dependências.

- **Descubra a latência dos componentes ao longo do caminho**: Você pode descobrir a latência monitorando requisições de **serviços de borda** (edge services) usando sistemas de monitoramento. OK, você recebeu o alerta, mas agora precisa descobrir qual componente faz com que a solicitação específica exceda o **Service Level Objective** (SLO). É exatamente por isso que o rastreamento distribuído existe: para localizar componentes no caminho que são gargalos ou passíveis de causar falhas.

- **Análise de causa raiz**: Imagine o seguinte cenário – você acorda com um alerta, são 2h da manhã e uma requisição envolvendo 5 microsserviços diferentes está falhando repetidamente. Você procura desesperadamente nos logs, ainda tentando abrir os olhos contra a tela ultra iluminada, em busca de erros na hora do alerta, mas o fluxo de dados é gigantesco demais para descobrir com precisão e rapidez o que aconteceu. Está demorando demais. Pois bem: usando o rastreio distribuído, é possível encontrar o primeiro serviço que falhou, obter os logs dessa falha e algumas outras coisas mais (a depender da implementação de rastreio feita no sistema).

- **Colete eventos durante a requisição**: Para ajudar no processo de debug, é possível adicionar elementos ao rastreamento. Por exemplo, você pode adicionar todas as feature flags avaliadas ao rastreamento para que, em caso de falha, possa saber exatamente quais flags foram avaliadas em cada um dos serviços no caminho da requisição.

Vamos começar com o básico, de onde todas as soluções de rastreamento distribuídas se originaram. Embora antes houvesse algumas soluções de rastreamento distribuído, o artigo entitulado <a href="https://static.googleusercontent.com/media/research.google.com/en//archive/papers/dapper-2010-1.pdf">Google Dapper (2010)</a>, de 14 páginas, é a pedra angular do rastreamento distribuído, por assim dizer. O documento trata de explicar como o Google desenvolveu uma ferramenta de rastreamento em nível de produção, tendo em vista 3 objetivos principais:

A observabilidade permite às equipes de engenharia de software detectar, diagnosticar e resolver problemas mais rapidamente, melhorar a estabilidade e o desempenho do sistema, e fornecer uma base para melhorias contínuas. **Plataformas/Ferramentas de observabilidade**, como Prometheus, Grafana, Jaeger e Splunk, são um conjunto de sistemas que podem coletar, processar, analisar e visualizar sinais de telemetria, incluindo métricas, logs e rastreamentos. As plataformas de observabilidade incluem New Relic, Splunk, Datadog, Grafana Stack, e Apache JMeter. Essas ferramentas de observabilidade de código aberto, como Grafana, Jaeger, Kafka, OpenTelemetry e Prometheus, tornaram-se cada vez mais populares nos últimos anos, e essa tendência provavelmente continuará. Isso é parcialmente impulsionado pelo desejo de reduzir os custos associados às ferramentas proprietárias de observabilidade e às opções de flexibilidade e personalização oferecidas pelas ferramentas de código aberto.

Portanto, são comumente usadas para implementar essas práticas. Em resumo, a observabilidade é crucial para a manutenção e operação eficiente de sistemas modernos, especialmente em arquiteturas distribuídas e baseadas em microsserviços. Então, logging, monitoring e observabilidade são partes essenciais do ciclo de vida de desenvolvimento, implantação e operação de software. Eles estão relacionados à fase de operação contínua (ou operação) e monitoramento no ciclo de vida do DevOps e CI/CD. 

Continuous Integration (CI):

<img height="177" align="right" src="https://github.com/user-attachments/assets/7682458c-7491-445a-962e-0e8ec050f957" />

  - Logging: Durante a fase de integração contínua, logs são gerados para registrar o progresso da construção, testes e integração do código. Eles ajudam a identificar e resolver problemas de build e erros de integração.

  - Monitoring: Nesta fase, o monitoramento pode ser usado para acompanhar o desempenho das builds, uso de recursos do CI server, e saúde dos serviços de CI.

  - Observabilidade: Não é um foco principal nesta fase, mas alguns aspectos podem ser monitorados para melhorar a eficiência e detectar problemas nos pipelines de CI.

Continuous Delivery/Deployment (CD):

<img height="177" align="right" src="https://github.com/user-attachments/assets/77fefcf5-4e9f-4bfa-ad2c-1cdd85c92456" />

  - Logging: Logs são cruciais durante a fase de deployment para registrar as atividades de implementação, mudanças de configuração e qualquer problema que ocorra durante o processo. Eles permitem o rastreamento de quem fez o que e quando.

  - Monitoring: O monitoramento é intensificado para garantir que as novas versões sejam implementadas sem causar interrupções ou degradação de desempenho. Ferramentas de monitoramento verificam a disponibilidade dos serviços, tempos de resposta e outros indicadores de desempenho.

  - Observabilidade: A observabilidade começa a ter um papel mais importante, ajudando a entender o comportamento do sistema pós-deployment, identificar possíveis regressões e garantir que todas as partes do sistema estejam funcionando conforme esperado.

Nas etapas/fases de Operações e Monitoramento:

<img height="177" align="right" src="https://github.com/user-attachments/assets/48b293ce-e582-4d58-8536-8ce6cdaeb03b" />

  - Monitoring: O monitoramento contínuo do sistema em produção garante que o serviço esteja funcionando corretamente e permite a detecção proativa de problemas. Isso inclui a monitorização de métricas como uso de CPU, memória, latência, taxas de erro, etc.

  - Observabilidade: A observabilidade aqui é fundamental para obter uma visão abrangente do estado do sistema. Utiliza logs, métricas e traços para proporcionar uma compreensão profunda de como o sistema está operando, identificar anomalias, realizar análises de causa raiz e otimizar o desempenho.

Em resumo, enquanto logging e monitoring são utilizados em todas as fases do CI/CD, a observabilidade se torna especialmente crítica na fase de operações e monitoramento, onde a complexidade e a necessidade de insights detalhados sobre o sistema são maiores.

No contexto do DevOps, a observabilidade geralmente é considerada uma prática que abrange várias etapas do ciclo de vida do software. Ela envolve a capacidade de compreender o comportamento interno de um sistema com base em suas saídas externas. Isso inclui métricas, registros (logging), rastreamentos (traces) e outras formas de dados que fornecem insights sobre o funcionamento de um sistema. Portanto, logging, monitoring e observabilidade estão presentes em várias etapas do processo de desenvolvimento e implantação de software:

1. **Desenvolvimento**: Durante o desenvolvimento de software, é crucial considerar os requisitos de logging para entender como o código está se comportando durante o desenvolvimento e testes. Isso pode ajudar os desenvolvedores a depurar problemas e entender o comportamento do sistema.

2. **Implantação (Deploy)**: Durante a implantação, é importante configurar sistemas de monitoramento para acompanhar o desempenho e a integridade do software em produção. Isso pode incluir monitoramento de métricas de desempenho, uso de recursos, erros e outras métricas relevantes.

3. **Operações contínuas**: Após a implantação, a monitoração contínua e a observabilidade são fundamentais para garantir que o software esteja funcionando conforme o esperado e para identificar e resolver problemas o mais rápido possível. Isso inclui a análise de logs, métricas e outros dados para identificar problemas de desempenho, bugs e outras questões operacionais.

Portanto, logging, monitoring e observabilidade são práticas contínuas que permeiam todo o ciclo de vida do software, desde o desenvolvimento até a operação contínua. 

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/c95b4eb3-6929-4fae-a3b6-a3a96a922e57" align="right" height="177">

Vamos imaginar a seguinte situação: Calculadora online

Você tem a sua aplicação e os usuários que estão utilizando a sua aplicação. Vamos supor que um usuário tomou um erro, e esse usuário pode mandar um feedback, enviar um email alertando ao time de suporte sobre o ocorrido. Pensando em um exemplo mais simples de aplicação para esse caso, vamos supor que sua aplicação é uma calculadora online, onde as operações de adição, subtração e multiplicação são atendidas com sucesso, mas a falha ocorre na divisão para aquele usuário específico. Daí você faz um teste e revisa as possíveis causas e não encontra nada assim como nos outros últimos usuários. Daí, logo aparecem mais casos de erros semelhantes em outros usuários, e novamente, podem te avisar ou não te avisar sobre o que está acontecendo esse erro. Uma possível explicação para esse erro é que o número de usuários aumentou e seu servidor não está conseguindo dar vazão a esse total de usuários, o erro mais comum é conhecido como "erro de sobrecarga". Pode ser o banco de dados que não consegue suportar esses milhões de acessos ou o próprio servidor. 

Então, o que você faz para analisar esse erro? Você põe log na sua aplicação, onde até então você não utilizava nenhum monitoramento, então você escreve um pequeno arquivo de texto `.TXT` que é a forma mais simples de verificar um erro da aplicação. E você coloca que deu uma `exception` (tratamentos de erros e excessões) onde houve divisão por zero e que deu erro por acesso ao banco do volume de transações que estão acontecendo.

> Há muitos casos de aplicações onde são desenvolvidas sem haver nenhuma aplicação/registro de logs, o que é um absurdo, porque se houver alguma falha, a detecção dos erros será falha também.

**Logging**: Então, você começa a profissionalizar mais esse cenário e utilizar bibliotecas de Logs ao invés de escrever em seus arquivos de texto, como:

<img src="" align="right" height="77">

- <a href="">NLog</a>: é uma biblioteca para C-Sharp.

- <a href="">Serilog</a>: é uma biblioteca para .NET.

- <a href="">Apache Log4J</a>: é uma biblioteca de logging de código aberto muito popular em sistemas Java. Ele é usado para registrar informações de eventos em aplicativos, ajudando os desenvolvedores a rastrear problemas, entender o fluxo de execução do código e monitorar o comportamento do sistema em tempo real.

- <a href="">Winston</a>: é uma biblioteca de log para Node.js.

- <a href="">Monolog</a>: É uma biblioteca de log para PHP.

- <a href="">Graylog</a>: é uma plataforma de gerenciamento de logs de código aberto que ajuda na coleta, armazenamento, análise e visualização de registros de diferentes fontes. Ele oferece uma solução integrada para lidar com logs de várias fontes, permitindo que as equipes de operações e desenvolvimento monitorem e analisem informações cruciais dos sistemas.

**Monitoring**: Pode ser que aconteça outros casos também, vamos supor que seu servidor vai ficar sem internet ou desligado ou ficar travado e você não vai estar tomando nenhum erro, mas os usuários não vão conseguir acessar, o que você pode fazer pra entender esse tipo de situação é utilizar um serviço de **health check** (checagem de saúde), ele pode não só ver se sua URL do site está em pé, mas também fazer uma consulta no banco. Veja as soluções abaixo:

- <a href="">UptimeRobot</a>: é um serviço online grátis que monitora a disponibilidade e o desempenho de sites, servidores, serviços web e outros recursos online. Ele verifica regularmente os recursos cadastrados e notifica os usuários caso haja qualquer interrupção ou queda de disponibilidade.

- <a href="">Site 24x7</a>: é uma plataforma de monitoramento e gerenciamento de TI baseada em nuvem que fornece uma gama abrangente de ferramentas para monitorar o desempenho de sites, servidores, aplicações e infraestruturas de rede.

- <a href="">Pingdom</a>: é um serviço de monitoramento de desempenho e disponibilidade de sites e aplicações web. Ele ajuda as empresas a garantir que seus sites e serviços estejam sempre disponíveis e operando com desempenho ideal.

Às vezes sua aplicação de site fica lento, podendo ser o CPU, memória ou I/O de disco. Ou seu banco de dados demorar com transações/segundo e o tempo de resposta das queries. Vamos supor que você tenha uma loja online onde para fazer os pagamentos você utiliza um gateway de pagamentos onde o tempo de resposta e a taxa de erros. Outro erro muito comum dentro de um e-commerce é que e se o botão de finalizar compra sumir? Alguém fez um commit em que há remoções acidentais das features. Daí o cenário fica algo bem complexo de monitoramento.

Outro ponto bastante importante é sua métrica de negócios sendo monitorada, ou seja, no caso de um ecommerce a quantidade de vendas sendo feitas. O ideal é você ter um monte de gráficos em tempo real e receber alertas sobre os acontecimentos de erros, sendo alertado pelo email ou pelo canal de chat. Um exemplo: Quando eu tiver um volume de compras abaixo de 100 compras/h você vai receber um alerta. Ou seja, você vai definir parâmetros e o que sair desses parâmetros você vai ser notificado.

<img src="https://github.com/IsaacAlves7/DevSecOps/assets/61624336/0c0da762-d301-4499-8b33-ca3debe1d01f" align="right" height="177">

Pensando em um melhor cenário de mundo perfeito que é o continuous deployment (implantação contínua). Podemos imaginar nossa aplicação rodando em vários containers Docker, vamos imaginar em 8 containers no total, dai todos eles estão mantidos na versão 1 da aplicação (`v1`), e o checksinho verde significa que todas as métricas obtiveram sucesso, o uso de CPU, rede, banco de dados, integração com gateway de pagamento e também o volume de vendas todos rodaram com êxito. E, com isso, você atualiza um dos seus containers para a versão 2 (`v2`). 

E qual a melhor plataforma para monitoramento e visualização de logs em aplicações ou sistemas? Depende muito da necessidade, do custo e do tipo de monitoramento desejado, os mais famosos, incluem:

<img src="https://i0.wp.com/invisibl.io/wp-content/uploads/2021/06/image.png?resize=750%2C412&ssl=1" height="277" align="right">

- Zabbix: é uma plataforma de monitoramento de rede e sistemas de código aberto. Ele é usado para monitorar a saúde e o desempenho de redes, servidores, máquinas virtuais e serviços diversos em tempo real. O Zabbix coleta dados de dispositivos e aplicativos usando várias técnicas, como SNMP, IPMI, agentes nativos e protocolos personalizados, e exibe essas informações de maneira visual em gráficos e relatórios. Além disso, ele permite configurar alertas para notificar quando ocorrem problemas ou anomalias, ajudando a garantir que os sistemas estejam funcionando de maneira eficiente e confiável.

- New Relic: é uma plataforma de monitoramento de desempenho de aplicativos (APM) e infraestrutura em nuvem. Ela é projetada para ajudar empresas a entenderem e otimizarem o desempenho de seus aplicativos, oferecendo insights detalhados sobre como os aplicativos estão funcionando em tempo real. Através de sua ferramenta, os desenvolvedores e as equipes de operações podem monitorar o desempenho de aplicativos web, móveis e de outras plataformas. Isso inclui métricas de desempenho, análise de transações, rastreamento de código, detecção de erros e falhas, entre outros recursos.

- Sentry.io: é uma plataforma de monitoramento de erros e falhas em tempo real, usada principalmente por desenvolvedores e equipes de operações para identificar, diagnosticar e corrigir problemas em aplicativos. Essencialmente, o Sentry.io ajuda a rastrear e registrar erros que ocorrem em aplicativos, fornecendo informações detalhadas sobre onde, quando e por que um erro aconteceu. Ele captura exceções, mensagens de erro, rastreamentos de pilha e outros dados relevantes para ajudar os desenvolvedores a entender e resolver problemas rapidamente.

- <a href="">Grafana stack</a>: é uma plataforma open-source usada para visualização e análise de dados. Ela permite criar painéis dinâmicos e altamente interativos para monitorar, analisar e entender métricas de sistemas complexos. O Grafana é amplamente utilizado em operações de TI, monitoramento de sistemas, análise de dados de IoT, DevOps, e em praticamente qualquer cenário em que a visualização e análise de dados são cruciais para entender o desempenho e o comportamento dos sistemas.

- Dynatrace: é uma plataforma de inteligência de software que oferece monitoramento completo e automatizado de desempenho, fornecendo insights precisos sobre ambientes complexos de nuvem, aplicativos, microservices, containers e infraestrutura.

- Datadog: é uma plataforma de monitoramento e análise em nuvem que oferece visibilidade abrangente dos ambientes de TI, infraestrutura, aplicativos e serviços. Ele permite às equipes de operações, desenvolvimento e segurança monitorar o desempenho de sistemas, identificar problemas, rastrear métricas-chave e entender o comportamento de aplicativos e infraestrutura.

- <a href="">Elastic stack (ELK stack)</a>: Dentro do ELK Stack, o serviço que fornece principalmente recursos para logging (registro de logs) é o Logstash, enquanto o serviço mais voltado para monitoring (monitoramento de métricas e eventos) é o Elasticsearch, juntamente com o Kibana para visualização e análise.

- Nagios: O Nagios é uma das ferramentas mais conhecidas e utilizadas para monitoramento de sistemas, redes e infraestrutura. Ele oferece recursos abrangentes para monitorar a disponibilidade de serviços, a integridade dos dispositivos, o desempenho de redes e outros aspectos críticos de sistemas de TI.

# 🟥 Zabbix
<img src="https://img.shields.io/badge/Grafana_Stack-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white">

<a href=""><img src="https://www.vectorlogo.zone/logos/zabbix/zabbix-ar21.svg" align="right" height="77"></a>

**Zabbix** é uma plataforma de monitoramento de código aberto usada para acompanhar o desempenho e a disponibilidade de servidores, redes, aplicações, serviços em nuvem e outros componentes de infraestrutura de TI. Ele permite coletar, armazenar, analisar e visualizar métricas em tempo real, alertando administradores quando algo foge do comportamento esperado, como aumento de uso de CPU, queda de serviços, problemas de disco, falhas de conectividade ou qualquer outro evento que comprometa a operação de sistemas. Por ser altamente configurável e escalável, o Zabbix é amplamente utilizado por empresas de diversos tamanhos, desde pequenos negócios até grandes corporações e instituições públicas.

A arquitetura do Zabbix é baseada em agentes instalados nos dispositivos a serem monitorados, que coletam os dados e enviam para o servidor Zabbix central. No entanto, ele também suporta coleta de dados sem agente, usando protocolos como SNMP, IPMI, SSH, Telnet, HTTP, entre outros, o que o torna extremamente flexível. Esses dados são armazenados em um banco de dados relacional (geralmente MySQL, PostgreSQL ou Oracle), permitindo análises históricas e geração de gráficos detalhados. O sistema de alertas é poderoso e pode ser integrado com e-mails, SMS, mensagens em aplicativos como Telegram, Slack ou via Webhook com qualquer sistema externo, permitindo ações automatizadas em resposta a incidentes.

A interface web do Zabbix oferece dashboards personalizáveis, gráficos, mapas de rede, relatórios e outras ferramentas de visualização, ajudando as equipes de operações a entenderem rapidamente o que está acontecendo em seus sistemas. Um dos seus pontos fortes é a detecção proativa de problemas baseada em gatilhos definidos pelo usuário, com suporte a expressões condicionais e templates prontos para facilitar a configuração de novos hosts. Ele também permite a descoberta automática de novos dispositivos ou serviços, o que reduz o esforço manual e mantém o ambiente sempre atualizado. Tudo isso contribui para a observabilidade e resiliência da infraestrutura, tornando o Zabbix uma peça fundamental na estratégia de monitoramento de ambientes modernos.

Além disso, o Zabbix é gratuito sob licença GPL, o que atrai a comunidade de software livre e permite personalizações sem custo de licença. No entanto, também existem serviços comerciais e suporte oferecidos pela empresa Zabbix SIA para empresas que desejam assistência profissional ou hospedagem gerenciada. O Zabbix é uma solução madura, ativa desde os anos 2000, com uma base sólida de usuários e ampla documentação. Em um mundo onde manter a disponibilidade e o desempenho dos sistemas é essencial para os negócios, o Zabbix se consolida como uma ferramenta completa e confiável para garantir que tudo esteja funcionando como deveria.

# 🟩 New Relic
<a href=""><img src="" align="right" height="77"></a>

**New Relic** é uma plataforma de observabilidade e monitoramento de desempenho de aplicações (APM — Application Performance Monitoring) que permite a desenvolvedores, engenheiros de software, operadores de infraestrutura e equipes de negócios acompanharem em tempo real o comportamento de seus sistemas digitais. Assim como o Datadog, ela centraliza uma ampla variedade de dados — como métricas, logs, rastreamentos distribuídos (traces), eventos e informações do navegador do usuário — para que os times possam diagnosticar problemas, melhorar a performance e tomar decisões baseadas em dados concretos. A filosofia do New Relic é oferecer uma visão unificada da saúde e do desempenho de toda a stack tecnológica, desde o frontend até os bancos de dados e serviços externos.

A plataforma funciona a partir da instalação de agentes em linguagens como Java, .NET, Node.js, Python, Ruby, PHP e Go, além de integrar com serviços de nuvem como AWS, Azure e Google Cloud. Esses agentes coletam dados automaticamente sobre tempo de resposta, throughput, uso de recursos, erros, gargalos e chamadas externas, e enviam tudo para o console da New Relic, que exibe os resultados por meio de dashboards interativos. Um de seus pontos fortes é a capacidade de traçar a jornada de uma requisição em múltiplos serviços, o que facilita a detecção de falhas em arquiteturas baseadas em microserviços ou contêineres, como os orquestrados por Kubernetes.

Além do monitoramento de backend, o New Relic também oferece funcionalidades para rastrear a experiência do usuário final, como o RUM (Real User Monitoring), que mostra como os visitantes de um site interagem com páginas e qual o impacto do desempenho do frontend sobre sua experiência. Há ainda recursos de testes sintéticos, que simulam acessos programados para detectar quedas ou lentidão antes que usuários reais sejam impactados. Com a evolução da plataforma, o New Relic expandiu suas capacidades para incluir logs centralizados, monitoramento de infraestrutura, alertas baseados em regras e inteligência artificial para detectar anomalias automaticamente.

A interface da ferramenta, chamada New Relic One, é baseada em uma abordagem "tudo-em-um", permitindo a correlação direta entre logs, métricas e traces em um só lugar, o que facilita a análise de causa raiz. A ferramenta também é extensível via APIs e suporta dashboards customizados com sua linguagem de consulta própria, a NRQL (New Relic Query Language), usada para criar visualizações específicas a partir dos dados coletados. Empresas de todos os tamanhos utilizam a New Relic tanto para manter seus sistemas disponíveis e eficientes quanto para otimizar suas aplicações com base em dados de uso reais. Embora seja uma solução comercial, a New Relic possui planos gratuitos com limites mensais, o que facilita sua adoção inicial.

Com o avanço da inteligência artificial e a crescente complexidade das aplicações modernas, ferramentas como o New Relic tornaram-se essenciais para dar visibilidade e controle sobre ambientes distribuídos e dinâmicos. Mais do que apenas um sistema de alerta, ele se posiciona como um verdadeiro copiloto técnico para times de engenharia, capaz de reduzir o tempo de resposta a incidentes e orientar melhorias contínuas com base em dados objetivos.

# 🟢 UptimeRobot
<a href=""><img src="" align="right" height="77"></a>

**UptimeRobot** é um serviço online que tem como principal função monitorar a disponibilidade (uptime) e o tempo de resposta de websites, servidores e serviços web em geral. Ele realiza verificações periódicas — geralmente a cada cinco minutos, no plano gratuito, e em intervalos menores em planos pagos — para assegurar que o serviço monitorado esteja acessível e funcionando corretamente. Quando detecta uma falha, como um site fora do ar (downtime) ou um tempo de resposta excessivo, o UptimeRobot imediatamente envia alertas por e-mail, SMS, chamadas de voz, ou integrações como Slack, Telegram, Discord, Webhooks e outras plataformas, permitindo que os responsáveis tomem providências rápidas para corrigir o problema.

A forma como ele realiza as checagens varia conforme o tipo de monitoramento configurado. Ele pode simplesmente fazer uma requisição HTTP ou HTTPS e verificar se o status code retornado indica sucesso, ou ainda usar métodos como monitoramento por ping, portas específicas (como SMTP, FTP, MySQL), além de verificar palavras-chave específicas dentro do conteúdo retornado por uma página para garantir que ela não só esteja online, mas também exiba a informação esperada. Isso é útil, por exemplo, quando o servidor responde com código 200, mas exibe uma página de erro no conteúdo HTML.

Além da sua simplicidade e facilidade de uso, o UptimeRobot também oferece dashboards e históricos de disponibilidade, permitindo que equipes acompanhem métricas como percentual de uptime mensal ou anual, tempo médio de resposta e momentos em que ocorreram falhas. Esses dados podem ser exibidos em painéis públicos, que são úteis para mostrar transparência ao cliente, ou privados, apenas para os administradores. Como ele possui servidores espalhados pelo mundo, consegue monitorar a disponibilidade de um site a partir de diferentes regiões geográficas, o que ajuda a identificar problemas de acessibilidade regional ou bloqueios por CDN e firewalls.

Empresas de todos os tamanhos usam o UptimeRobot como uma primeira camada de detecção de problemas, especialmente em sistemas que exigem alta disponibilidade, como e-commerces, APIs públicas, serviços financeiros e plataformas SaaS. Embora não ofereça a mesma profundidade de uma ferramenta de observabilidade como o New Relic ou o Datadog, o UptimeRobot é uma excelente escolha para monitoramento simples, direto e com baixo custo, sendo frequentemente usado em conjunto com outras ferramentas. Ele se tornou popular entre desenvolvedores independentes, startups e equipes de DevOps que precisam de alertas confiáveis sem a complexidade de configurar soluções mais robustas. Seu modelo freemium com plano gratuito atrai muitos usuários que desejam garantir que seus sistemas estejam sempre no ar, o que faz dele uma peça útil em qualquer stack de monitoramento.

# Nagios

# Splunk

# Voice search

# 🐶 Datadog
<a href=""><img src="" align="right" height="77"></a>

**Datadog** é uma plataforma de monitoramento e análise baseada na nuvem, projetada para fornecer visibilidade completa sobre a infraestrutura de TI, aplicações e serviços em execução em ambientes modernos, especialmente os que utilizam arquiteturas distribuídas, microserviços, contêineres e nuvens públicas ou híbridas. Seu objetivo é ajudar engenheiros, desenvolvedores, times de DevOps, SRE e segurança a observarem o comportamento de seus sistemas em tempo real, correlacionando métricas, logs, rastreamentos distribuídos e eventos em uma interface unificada e de fácil uso. Com isso, o Datadog permite detectar problemas de desempenho, gargalos, falhas ou comportamentos anômalos antes que impactem os usuários finais.

O grande diferencial do Datadog é justamente essa abordagem unificada. Ele coleta dados de centenas de integrações prontas — como AWS, Azure, GCP, Docker, Kubernetes, PostgreSQL, Redis, NGINX, entre outros — e os centraliza para que se possa visualizar tudo em painéis interativos, alertar sobre condições específicas com base em regras configuráveis, e realizar análises históricas. O usuário não precisa se preocupar com a instalação de servidores ou infraestrutura de armazenamento local para os dados monitorados, pois tudo é processado e armazenado na nuvem da própria plataforma. Além disso, com o suporte nativo a APM (Application Performance Monitoring), é possível rastrear o tempo de execução de requisições em serviços complexos, visualizar onde ocorrem lentidões ou erros, e otimizar o desempenho do software com base em dados concretos.

Outra camada que o Datadog oferece é o monitoramento de segurança e conformidade, chamado de Cloud Security Posture Management (CSPM) e Runtime Security, que ajuda a detectar configurações erradas, vulnerabilidades, comportamentos suspeitos ou riscos em tempo real, correlacionando-os com o restante da infraestrutura observada. Há também recursos de monitoramento de experiência do usuário, como testes sintéticos, RUM (Real User Monitoring) e dashboards focados em frontend, permitindo uma visão fim a fim, do navegador do usuário até o banco de dados.

O Datadog é um serviço comercial, baseado em planos por volume de dados e quantidade de hosts monitorados. Ele é muito valorizado por empresas que operam em larga escala, principalmente pelo fato de permitir que múltiplas equipes compartilhem contexto sem silos de informação. Também oferece uma API completa e SDKs em várias linguagens para customização, além de suporte a Infrastructure-as-Code para automatizar sua configuração via Terraform, CloudFormation, entre outros. Com uma interface polida, rica em visualizações, e uma comunidade ativa, o Datadog se posiciona como uma das soluções mais modernas e completas no campo de observabilidade, sendo amplamente adotado em startups, corporações globais e setores com alto nível de exigência tecnológica.

# 🦖 Dynatrace
O **Dynatrace** é uma plataforma de observabilidade e inteligência de software impulsionada por IA que vai muito além do monitoramento tradicional. Em sua essência, é um sistema que fornece visibilidade completa e automatizada sobre o desempenho, a saúde e a segurança de toda a sua pilha tecnológica, desde a experiência do usuário final até a infraestrutura subjacente. A grande diferença em relação a ferramentas mais antigas está na sua arquitetura baseada em agentes que utilizuma tecnologia de descoberta automática e rastreamento de dependências, eliminando a necessidade de configuração manual extensiva para instrumentar aplicações.

A peça central da inovação do Dynatrace é a sua engine de inteligência artificial proprietária, chamada Davis. Diferente de sistemas de alerta comuns que dependem de limiares estáticos pré-definidos por humanos, o Davis aprende continuamente o comportamento normal de seu ambiente e, a partir dessa linha de base, é capaz de detectar automaticamente anomalias e problemas. Ele não apenas identifica que algo está errado, mas faz a correlação causal entre eventos em diferentes partes da stack para apontar a causa raiz de um problema. Por exemplo, ele pode conectar diretamente um pico no tempo de carregamento de uma página web a uma lentidão específica em um microserviço, que por sua vez foi causada por um consumo excessivo de CPU em um nó específico do Kubernetes, tudo de forma automática e em tempo real.

A plataforma é abrangente por design, cobrindo todos os pilares da observabilidade moderna. Ela monitora a experiência digital dos usuários, rastreando cada clique, transação e jornada em aplicações web e móveis, capturando não apenas métricas de desempenho, mas também a frustração ou satisfação do usuário. No nível das aplicações, ela realiza o APM (Application Performance Monitoring) com rastreamento distribuído detalhado, mapeando automaticamente todas as transações entre serviços, bancos de dados e filas de mensagens. Na infraestrutura, monitora não apenas VMs e containers, mas também serviços em nuvem, bancos de dados e redes. E, de forma crítica para os times de DevOps modernos, possui uma integração nativa e profunda com ecossistemas de orquestração como Kubernetes e OpenShift, fornecendo um mapa topológico dinâmico e em tempo real de todos os seus pods, serviços e namespaces.

Um dos conceitos mais poderosos introduzidos pelo Dynatrace é a noção de "Smartscape", que é um mapa de dependências em tempo real e auto-atualizável de toda a sua arquitetura de aplicação. Este mapa visual mostra como cada componente — desde um load balancer na AWS até um banco de dados SQL em um container — se conecta e depende dos outros. Quando um problema ocorre, o Smartscape é automaticamente destacado para mostrar o caminho exato do impacto, permitindo que os engenheiros entendam instantaneamente o escopo completo de uma falha.

Além do monitoramento de desempenho, o Dynatrace expandiu suas capacidades para incluir automação de DevOps, segurança aplicacional e gerenciamento de custos em nuvem. A plataforma pode integrar-se com pipelines de CI/CD para fornecer gating automático, onde deploys podem ser automaticamente aprovados ou revertidos com base em métricas de qualidade de serviço. Na segurança, ele identifica vulnerabilidades em tempo de execução e bibliotecas de terceiros. E no gerenciamento de nuvem, ele ajuda a identificar recursos subutilizados e otimizar gastos.

Em resumo, o Dynatrace representa uma evolução do conceito de monitoramento para uma abordagem de observabilidade contínua e automatizada. Ele substitui a sobrecarga operacional de configurar milhares de alertas e dashboards manuais por um sistema que descobre, monitora e diagnostica problemas de forma autônoma, permitindo que os times de engenharia se concentrem na construção e melhoria de produtos, em vez de gastar tempo tentando entender por que um sistema complexo e distribuído está se comportando de maneira inesperada.

# 🦡 Honeybadger
<img height="77" align="right" src="https://github.com/user-attachments/assets/7c63a975-3d56-4f60-81ae-5d9df8da0f1c" />

Quando falamos de observabilidade com **Honeybadger**, estamos entrando em um terreno que combina conceitos de engenharia de software, monitoramento e análise de falhas em aplicações. Observabilidade, de maneira geral, é a capacidade de entender o que está acontecendo dentro de um sistema complexo apenas a partir de suas saídas, como logs, métricas e traces. Diferente do monitoramento tradicional, que geralmente se limita a avisar quando algo está fora do normal, a observabilidade permite que você investigue profundamente as causas de problemas, entenda padrões de comportamento do sistema e até antecipe falhas antes que se tornem críticas. É uma abordagem proativa, que dá poder ao engenheiro de enxergar além do que os alertas básicos conseguem mostrar.

Honeybadger, nesse contexto, é uma ferramenta de observabilidade focada em aplicações, especialmente em sistemas web e serviços que utilizam linguagens como Ruby, Elixir, Python e JavaScript. Ele atua como um intermediário inteligente, capturando exceções, erros de runtime, falhas em background jobs e problemas de performance, e apresentando essas informações de forma estruturada para que a equipe consiga agir rapidamente. O diferencial do Honeybadger não está apenas em registrar erros, mas em contextualizá-los: ele mostra exatamente onde ocorreu a falha no código, quais parâmetros estavam sendo utilizados, o histórico de requisições e até o ambiente em que o erro surgiu. Isso transforma a forma como desenvolvedores lidam com problemas, passando de uma abordagem reativa, onde se corrige o que já quebrou, para uma abordagem mais investigativa e estratégica, em que se consegue entender tendências, padrões e até prevenir futuros erros.

Além disso, Honeybadger integra métricas de monitoramento e health checks, permitindo que equipes observem não apenas erros isolados, mas também o comportamento geral da aplicação ao longo do tempo. Ele se conecta a pipelines de CI/CD, sistemas de notificação e dashboards de observabilidade, criando uma visão unificada do estado do sistema. Isso significa que, com Honeybadger, a observabilidade deixa de ser apenas um conceito abstrato e se torna prática diária, proporcionando transparência, redução de downtime e aumento da confiabilidade do software. A combinação entre capturas detalhadas de erros, contexto rico e integração com o fluxo de desenvolvimento transforma o Honeybadger em uma ferramenta poderosa para qualquer equipe que queira manter sistemas complexos estáveis, resilientes e compreensíveis.

# 🍨 Elastic Stack
<img src="https://cdn.worldvectorlogo.com/logos/elastic.svg" height="77" align="right">

A empresa Elastic ajuda as organizações, seus funcionários, e clientes a acelerarem os resultados que importam com soluções de busca, monitoramento, e segurança. A empresa fornece vários serviços com seus produtos, dentre eles, o mais famoso é o **Elastic Stack**, abreviado como **ELK Stack** que é uma pilha de software de código aberto usada para coletar, armazenar, pesquisar, visualizar e analisar dados de log e outros tipos de dados em tempo real. O nome "ELK" é um acrônimo que representa os três principais componentes da pilha: **E**lasticsearch, **L**ogstach e **K**ibana.

Elastic Stack ou ELK Stack é um produto open-source designado para tratar e organizar grandes quantidades de dados em qualquer tipo de fonte e formato. Devido a sua alta capacidade de armazenamento na centralização de logs, esse recurso garante a análise e pesquisa de informações em tempo real.

<img src="https://cdn.worldvectorlogo.com/logos/elastic-stack.svg" height="77" align="right">

O ELK Stack é amplamente utilizado em operações de TI, monitoramento de sistemas e segurança da informação para coletar, analisar e visualizar logs e eventos de diversas fontes. É uma ferramenta poderosa para detectar problemas, solucionar problemas, monitorar o desempenho e a segurança de sistemas e aplicativos, e muito mais. Oferecendo diversos mecanismos de busca e análise, o processo de integrar e centralizar os logs em um único local nos ajuda a identificar diversos problemas com os nossos servidores e aplicações. Portanto, o Elastic Stack pode ser usado para monitorar tanto a aplicação quanto a infraestrutura em produção, oferecendo uma gama de ferramentas para coleta, armazenamento, análise e visualização de dados operacionais.

<img width="656" height="393" alt="diagram-opentelemetry-api-sdk-with-elastic-apm-agents" src="https://github.com/user-attachments/assets/223f6b93-f553-49f1-b062-c17eb117ab78" />

Com a difusão, crescimento e expansão desses projetos, a comunidade inseriu um novo projeto para coleta de dados, conhecido como **Beats**. Deste modo, a ferramenta que era formada pelo acrônimo “ELK” não tinha mais sentido com os Beats, pois iria ficar uma sopa de letrinhas. Assim, surgiu o Elastic Stack que atualmente é mantido pela Elastic.

<img src="https://user-images.githubusercontent.com/61624336/234415822-3c516b5b-9779-4c6a-bed3-78367f8b3be1.svg" height="77" align="right">

O **Elasticsearch** é um mecanismo de busca rápido e ampliável que é o coração do Elastic Stack. O Elasticsearch é um mecanismo de busca e análise distribuída altamente escalável. Ele é projetado para indexar, armazenar e recuperar dados de forma eficiente, permitindo buscas rápidas e análises avançadas. O Elasticsearch é frequentemente usado como o mecanismo de armazenamento central para dados de log e outros tipos de dados. O **Index Lifecycle Management (ILM)** é um recurso oferecido pelo Elasticsearch, um mecanismo de busca e análise distribuída, que permite gerenciar o ciclo de vida dos índices de dados armazenados no Elasticsearch. É particularmente útil para a gestão de índices de log e outros tipos de dados que têm requisitos específicos de retenção, compactação e arquivamento ao longo do tempo.

O ILM oferece as seguintes funcionalidades:

- Definição de Políticas de Ciclo de Vida: Você pode definir políticas de ciclo de vida que especificam regras para a criação, retenção, compactação e arquivamento de índices. As políticas podem ser personalizadas para atender aos requisitos específicos do seu aplicativo.

- Fases de Ciclo de Vida: As políticas de ciclo de vida normalmente têm várias fases, como "quente" (hot), "morno" (warm), "frio" (cold) e "congelado" (frozen), que representam diferentes estágios na vida de um índice. Por exemplo, índices recentes podem ser mantidos na fase "quente" para consultas em tempo real, enquanto índices mais antigos podem ser movidos para a fase "frio" para economizar recursos.

- Transições Automáticas: O ILM permite que você configure regras para que os índices façam transições automáticas entre as fases com base em critérios predefinidos, como idade do índice ou tamanho total.

- Ações de Gerenciamento: Você pode especificar ações a serem executadas em índices quando eles fazem transições de fase. Isso pode incluir a alocação de índices para diferentes nós do cluster, compactação, exclusão ou arquivamento.

- Rastreamento de Histórico: O ILM registra um histórico das ações realizadas em índices, o que permite rastrear as mudanças de fase e entender o ciclo de vida de cada índice.

- Integração com o Elasticsearch Stack: O ILM é integrado com outros componentes do Elasticsearch, como o Kibana (para visualização e gerenciamento) e a segurança do Elasticsearch (para controle de acesso).

O ILM é uma ferramenta valiosa para ambientes que lidam com grandes volumes de dados, como logs de servidor, métricas de desempenho, eventos de segurança e muito mais. Ele ajuda a otimizar o uso de recursos de armazenamento e a simplificar a manutenção de índices, garantindo que os dados estejam disponíveis quando necessário e que sejam arquivados de forma eficiente quando não são mais necessários para consultas em tempo real.

<img src="https://cdn.worldvectorlogo.com/logos/elastic-logstash.svg" height="77" align="right">

O **Logstash** é um mecanismo de coleta, transformação e ingestão de dados. Ele permite que você colete dados de várias fontes, os transforme para um formato desejado e, em seguida, os encaminhe para o Elasticsearch ou para outros sistemas de armazenamento ou análise. O Logstash é especialmente útil para ingestão de logs de várias fontes, como servidores, aplicativos e dispositivos de rede.

Com o passar do tempo muitas pessoas fizeram testes com o Elasticsearch, incluindo uma integração com os logs gerados pelos nossos servidores, aplicações ou sistemas. E como o Elasticsearch guarda muita informação, ele obviamente aguentaria os logs.

Partindo desse princípio, eles reconheceram que as informações dos logs podiam ser tratadas um pouco antes, no meio do caminho, para que ficassem mais legíveis quando fossem integradas ao Elasticsearch. E a partir desse conceito foi criada uma ferramenta chamada Logstash, responsável pela intermediação entre as informações dos nossos logs antes de integrá-las ao Elasticsearch.

Ou seja, quando um servidor web envia um axis log, seja um Apache, Nginx ou quando o seu PhP apresenta algum erro, essas informações são enviadas ao Logstash, que recebe os logs e aplica filtros para prepará-las da melhor forma possível antes dessa integração.

Algumas características e funcionalidades do Logstash:

- Coleta de dados: O Logstash pode coletar dados de uma ampla variedade de fontes, incluindo logs de aplicativos, eventos de sistemas, bancos de dados, feeds de dados, entre outros.

- Transformação de dados: Ele permite que você transforme os dados brutos de log em um formato estruturado e enriqueça esses dados adicionando informações relevantes antes de armazená-los no Elasticsearch. Isso é especialmente útil para normalizar dados de várias fontes diferentes.

- Suporte a plugins: O Logstash possui uma arquitetura de plugin que permite estender suas funcionalidades. Existem plugins disponíveis para várias entradas, filtros e saídas, tornando-o altamente configurável e adaptável a diferentes casos de uso.

- Escalabilidade: O Logstash pode ser escalado horizontalmente para lidar com grandes volumes de dados. Você pode configurar clusters de Logstash para distribuir a carga de processamento.

- Integração com o Elasticsearch: O Logstash é frequentemente usado em conjunto com o Elasticsearch e o Kibana para criar uma solução completa de análise de logs e eventos, onde os dados coletados são armazenados no Elasticsearch e visualizados usando o Kibana.

<img src="https://cdn.worldvectorlogo.com/logos/elastic-kibana.svg" height="77" align="right">

O **Kibana** é a interface do usuário e a poderosa camada de visualização customizável para o Elastic Stack. O Kibana é uma interface de usuário de código aberto que facilita a visualização e a análise de dados armazenados no Elasticsearch. Com o Kibana, você pode criar painéis interativos, gráficos, tabelas e painéis de controle personalizados para explorar dados, criar visualizações e obter insights em tempo real. É uma ferramenta poderosa para monitoramento e análise de dados de logs, métricas e eventos. Abaixo, vou explicar algumas das principais características e funcionalidades do Kibana:

- Visualização de Dados: O Kibana oferece uma ampla variedade de opções para visualizar dados. Você pode criar gráficos de barras, gráficos de pizza, tabelas dinâmicas, gráficos de dispersão, mapas geográficos e muito mais. Essas visualizações ajudam a transformar dados brutos em informações facilmente compreensíveis.

- Painéis de Controle: Com o Kibana, você pode criar painéis de controle personalizados que agregam várias visualizações e gráficos em uma única página. Isso é útil para monitorar o desempenho de aplicativos, sistemas ou serviços em tempo real.

- Exploração de Dados Interativa: Os usuários podem explorar e filtrar dados interativamente, permitindo que investiguem eventos específicos e identifiquem tendências ou anomalias rapidamente.

- Consulta e Pesquisa Avançadas: O Kibana possui uma poderosa linguagem de consulta chamada KQL (Kibana Query Language) que permite criar consultas complexas para recuperar dados específicos do Elasticsearch.

- Integração com Elasticsearch: O Kibana é altamente integrado ao Elasticsearch, facilitando a configuração de painéis e visualizações para usar os dados armazenados no Elasticsearch. Os dados de log ou métricas coletados pelo Logstash ou outros meios podem ser facilmente acessados e visualizados no Kibana.

- Segurança e Autenticação: O Kibana oferece recursos de segurança robustos, permitindo controlar o acesso dos usuários aos dados e às funcionalidades. Ele suporta autenticação de usuário, autorização baseada em funções e integração com sistemas de autenticação externa.

- Personalização: Você pode personalizar a aparência e a experiência do usuário no Kibana, adaptando-o às necessidades específicas da sua organização. Isso inclui a criação de painéis de controle com temas personalizados e layouts específicos.

- Programação de Alertas: O Kibana permite criar alertas com base em condições definidas, como eventos críticos ou métricas fora dos limites aceitáveis. Os alertas podem ser configurados para notificar automaticamente as equipes de operações ou administradores quando ocorrem eventos importantes.

- Exportação e Compartilhamento: Você pode exportar visualizações, painéis e relatórios do Kibana em vários formatos, como PDF ou PNG. Além disso, é possível compartilhar links para painéis específicos com outros membros da equipe para colaboração e revisão.

<img src="https://cdn.worldvectorlogo.com/logos/elastic-beats.svg" height="77" align="right">

O **Elastic Beats**, muitas vezes chamado apenas de "Beats," é uma coleção de agentes leves de código aberto desenvolvidos pela Elastic. Cada agente Beat é projetado para uma tarefa específica, como coleta, envio e agregação de dados de diferentes fontes para o Elasticsearch ou para outras saídas, como sistemas de armazenamento ou visualização. Os Beats são projetados para serem simples de configurar, altamente eficientes e escaláveis.

# ☀️ Grafana Stack
<img src="https://img.shields.io/badge/Grafana_Stack-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white"> <img src="https://img.shields.io/badge/Grafana-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white"> <img src="https://img.shields.io/badge/Prometheus-25.3.2-E6522C?style=flat&logo=Prometheus&logoColor=white"> <img src="https://img.shields.io/badge/OpenTelemetry-25.3.2-gold?style=flat&logo=OpenTelemetry&logoColor=white">

<a href="https://grafana.com/"><img src="https://cdn.worldvectorlogo.com/logos/grafana.svg" align="right" height="77"></a>

O **Grafana Stack** é um conjunto de ferramentas desenvolvidas e mantidas pela Grafana Labs com o objetivo de fornecer uma plataforma completa e integrada para observabilidade, ou seja, para o monitoramento, análise e visualização de dados de sistemas, aplicações, infraestrutura e serviços. Ele é muito utilizado por equipes de DevOps, SREs e engenheiros de software para entenderem como os sistemas estão se comportando em tempo real, detectar falhas, identificar gargalos e manter a confiabilidade dos ambientes em produção. A base desse stack é o Grafana, uma ferramenta open source de visualização de métricas, logs e traces que permite a criação de dashboards interativos altamente customizáveis.

Dentro do Grafana Stack, há várias soluções que se complementam. O Grafana em si é a interface principal, onde os usuários constroem painéis e gráficos a partir de dados oriundos de diferentes fontes. Ele se conecta a bancos de dados de séries temporais como Prometheus, InfluxDB, Graphite e também a fontes de logs como Loki. 

<img src="https://github.com/user-attachments/assets/ebd56e12-4d17-4348-add3-972b4865df48" align="right" height="77">

**Prometheus** é uma ferramenta de monitoramento e alertas desenvolvida inicialmente pela SoundCloud, e hoje é um projeto open source altamente adotado na comunidade de observabilidade. Ele é usado para coletar, armazenar e consultar métricas de sistemas e aplicações, permitindo uma visão detalhada sobre o desempenho e comportamento do ambiente em tempo real. A grande característica do Prometheus é sua abordagem baseada em coleta ativa: em vez de receber dados enviados pelas aplicações, ele se conecta periodicamente a endpoints HTTP expostos pelos serviços (chamados de targets), geralmente na rota `/metrics`, e extrai as informações no formato de pares chave-valor.

Diferente de soluções baseadas em logs ou traces, Prometheus trabalha principalmente com séries temporais — valores numéricos associados a uma métrica, registrados ao longo do tempo com rótulos (labels) que representam dimensões como nome da aplicação, tipo de instância, região, status HTTP, entre outros. Isso permite a análise detalhada com um alto nível de segmentação, como por exemplo o número de requisições com erro por segundo apenas em uma determinada região, ou o uso de memória por tipo de serviço. As queries sobre essas métricas são feitas com PromQL, uma linguagem de consulta específica da ferramenta, capaz de expressar estatísticas, agregações e alertas com muita flexibilidade.

Prometheus é frequentemente usado em arquiteturas modernas como microserviços orquestrados por Kubernetes, onde cada serviço ou container pode expor suas métricas e ser descoberto automaticamente pelo Prometheus. Isso torna a ferramenta muito eficaz para ambientes dinâmicos e distribuídos. Ele também possui suporte nativo para armazenamento local das métricas, que são mantidas por um período definido (por padrão, duas semanas), mas pode ser integrado a sistemas de armazenamento remoto para long-term metrics.

Além da coleta e consulta, Prometheus tem um sistema de alertas robusto, geralmente configurado com arquivos YAML que definem regras sobre quando disparar notificações com base nos dados de métricas. Esses alertas são gerenciados por um componente chamado Alertmanager, que pode enviar mensagens para e-mails, Slack, PagerDuty, entre outros destinos, aplicando filtros e agrupamentos para evitar ruídos desnecessários.

Por fim, Prometheus é frequentemente combinado com o Grafana, uma ferramenta de visualização que consome suas métricas e permite criar dashboards interativos e informativos para visualização em tempo real. Essa combinação se tornou praticamente um padrão de fato em observabilidade, especialmente em ambientes de DevOps e SRE, por oferecer uma solução completa, flexível e escalável de monitoramento, com grande adoção na comunidade open source.

<img src="https://github.com/user-attachments/assets/0b1c3fd2-ae8a-4c90-b249-1b4f7924a39a" align="right" height="77">

O **Loki**, inclusive, é parte do stack e foi desenvolvido pela própria Grafana Labs para tratar logs de maneira semelhante ao Prometheus trata métricas: como séries temporais indexadas, porém com menor sobrecarga de processamento. Já o Prometheus, embora não seja originalmente criado pela Grafana Labs, é amplamente adotado e compatível com o stack, sendo responsável pela coleta de métricas de aplicações e sistemas, muitas vezes através de endpoints expostos pelas próprias aplicações (como o padrão /metrics).

<img src="https://github.com/user-attachments/assets/e258fe05-6aa0-4df5-9189-3a023aa894b0" align="right" height="77">

Além disso, o stack inclui o **Tempo**, que é uma ferramenta de rastreamento distribuído (distributed tracing). O Grafana Tempo permite visualizar e analisar traces de requisições em sistemas complexos, o que é essencial para diagnosticar problemas de performance, identificar latências entre serviços e entender o fluxo de chamadas em arquiteturas de microsserviços. Ele se integra com bibliotecas como OpenTelemetry e Jaeger, permitindo rastrear requisições de ponta a ponta. Com Loki, Prometheus e Tempo juntos, o Grafana Stack oferece uma solução chamada de “correlação de observabilidade”, onde o usuário consegue cruzar logs, métricas e traces em uma única interface, facilitando investigações e diminuindo o tempo de resposta a incidentes.

O Grafana Stack também pode incluir o **Grafana Agent**, que é um componente leve para coleta de métricas, logs e traces, simplificando a instrumentação de aplicações e o envio dos dados para os demais componentes. Em ambientes maiores ou gerenciados, há ainda o Grafana Cloud, que oferece tudo isso como serviço, com escalabilidade e facilidades de gerenciamento. Com isso, o Grafana Stack se posiciona como uma alternativa completa para observabilidade, integrando coleta, armazenamento e visualização de dados em tempo real, com foco em flexibilidade, performance e comunidade ativa.

<img src="https://github.com/user-attachments/assets/952f9c0f-78dd-4f72-946c-c444ba38829f" align="right" height="77">

**OpenTelemetry (OTel)** é um framework de observabilidade open source com o qual as equipes de desenvolvimento podem gerar, processar e transmitir dados de telemetria em um formato unificado. Foi desenvolvido pela Cloud Native Computing Foundation (CNCF) para fornecer protocolos e ferramentas padronizados com o objetivo de coletar e rotear métricas, logs e traces para plataformas de monitoramento.

O OpenTelemetry fornece SDKs, APIs e ferramentas com independência de fornecedor para que seus dados possam ser enviados para qualquer backend de observabilidade para análise.

O OpenTelemetry está rapidamente se tornando o padrão de telemetria de observabilidade dominante em aplicações nativas da nuvem. A adoção do OpenTelemetry é considerada crítica para as organizações que querem estar preparadas para as demandas de dados do futuro sem estarem vinculadas a um fornecedor específico ou às limitações de suas tecnologias existentes.

![image](https://github.com/user-attachments/assets/550b9c21-58cb-46e0-afa5-79a6abeef9f9)

# ⚡ Typesense
<a href="https://typesense.org/"><img src="https://github.com/user-attachments/assets/c1fd54a2-4353-4067-8844-4802542e59f2" align="right" height="77"></a>

**Typesense** é um mecanismo de busca de código aberto, criado para oferecer uma alternativa moderna, rápida e fácil de usar em comparação com ferramentas mais complexas como Elasticsearch e Solr. Ele é projetado com foco na simplicidade e na performance, tornando-se ideal para desenvolvedores que desejam implementar funcionalidades de busca com qualidade, sem precisar configurar ou manter uma infraestrutura muito pesada. 

O Typesense é escrito em C++ e otimizado para oferecer tempos de resposta muito baixos, mesmo com grandes volumes de dados. A ideia central é facilitar a indexação e a consulta de dados estruturados, como registros de produtos, usuários, artigos ou qualquer outro conjunto de documentos que possa se beneficiar de busca textual eficiente.

O grande diferencial do Typesense é sua abordagem voltada para o desenvolvedor. Sua API é simples, baseada em REST, com opções modernas de integração que funcionam bem em back-ends e também diretamente em front-ends. Ele oferece recursos como tolerância a erros de digitação (fuzzy search), autocompletar, ordenação por relevância e por campos personalizados, filtros facetas, e indexação em tempo real, o que permite que os dados atualizados sejam quase imediatamente refletidos nos resultados de busca. Isso é especialmente útil em sistemas de e-commerce, catálogos, dashboards administrativos ou portais de notícias.

O Typesense pode ser usado localmente ou como serviço em nuvem, através do Typesense Cloud, que elimina a necessidade de configuração manual de servidores. Ele foi criado para consumir poucos recursos e ainda assim fornecer desempenho de nível profissional. A instalação e a configuração são diretas: é possível ter um cluster funcional em minutos. Ele também oferece SDKs e bibliotecas para diversas linguagens como JavaScript, Python, Ruby e outros, facilitando ainda mais sua adoção em projetos variados. Além disso, a estrutura de indexação dele é baseada em esquemas simples, o que ajuda a manter a clareza dos dados e evitar erros durante a indexação ou consulta.

Em um cenário onde a busca é uma funcionalidade crítica — seja para melhorar a experiência do usuário final, seja para oferecer relatórios ou filtros poderosos — o Typesense surge como uma solução eficiente, moderna e acessível, com uma curva de aprendizado muito menor que seus concorrentes tradicionais, sem abrir mão de funcionalidades robustas e performance de alto nível.

# 🟠 OpMon
<img src="https://github.com/user-attachments/assets/719e67fe-2882-447e-9e45-bda77564fcc3" align="right" height="177">

O **OpMon** é uma plataforma brasileira de monitoramento de infraestrutura de TI, redes, servidores, serviços, aplicações e negócios, desenvolvida com o objetivo de proporcionar visibilidade completa e em tempo real sobre os ativos tecnológicos de uma organização. Ele se baseia em conceitos como observabilidade, automação e análise proativa de falhas para oferecer um ambiente de monitoramento robusto, permitindo que as equipes de tecnologia antecipem problemas, identifiquem gargalos e tomem decisões com mais agilidade e segurança.

A ferramenta se destaca por ser altamente personalizável e adaptável a diferentes cenários corporativos. Ela é capaz de monitorar tanto ativos locais quanto ambientes em nuvem ou híbridos, integrando diferentes protocolos como SNMP, WMI, SSH, API REST, entre outros. Com dashboards interativos, gráficos de desempenho, alertas por diversos canais (e-mail, SMS, Telegram, etc.) e recursos como relatórios automatizados e detecção de anomalias, o OpMon se torna um aliado essencial para times de infraestrutura e operações, permitindo uma gestão proativa e eficiente.

Além disso, o OpMon permite a correlação entre indicadores técnicos e processos de negócio, criando uma camada de monitoramento orientada ao impacto nos serviços finais da empresa. Isso significa que é possível acompanhar o funcionamento de um sistema de forma mais contextualizada, considerando seu papel no fluxo operacional da empresa como um todo. Ele também possui recursos de integração com ITSMs, CMDBs e ferramentas de automação, promovendo um ecossistema de TI mais coeso e inteligente.

Por ser uma solução nacional, o OpMon se alinha às necessidades do mercado brasileiro, com suporte técnico especializado, documentação em português e atualizações constantes que acompanham as tendências de TI. Sua adoção é comum em ambientes corporativos que exigem alta disponibilidade, controle rigoroso de SLA e visibilidade completa sobre os recursos tecnológicos, posicionando-se como uma alternativa sólida frente a soluções internacionais de monitoramento.

O OpMon pode ser considerado **equivalente em propósito**, mas **não idêntico em arquitetura e escopo** a ferramentas como Grafana Stack, Elastic Stack, Datadog, Zabbix e New Relic. Todos esses sistemas compartilham o objetivo principal de monitorar infraestrutura, aplicações e serviços de TI, mas cada um tem enfoques, arquiteturas e diferenciais técnicos distintos.

O OpMon, por ser uma plataforma nacional, tem uma abordagem mais integrada e pronta para uso, com foco em **monitoramento unificado** e **correlação entre TI e negócio**, sem exigir que o usuário monte ou componha diferentes partes de uma stack. Ele possui coleta de métricas, geração de alertas, visualização gráfica, automação de respostas e gestão de disponibilidade, atuando de forma semelhante ao Zabbix e ao Datadog em sua proposta de “tudo em um”.

O Grafana Stack (com Prometheus, Loki, Tempo, etc.) e o Elastic Stack (com Elasticsearch, Logstash, Kibana) são **plataformas altamente modulares**, onde cada componente tem uma responsabilidade clara (como logs, métricas ou tracing) e precisam ser integrados manualmente. Eles oferecem **grande flexibilidade**, sendo ideais para times com maturidade técnica e que desejam controle fino sobre cada etapa da observabilidade.

Já o Datadog e o New Relic são soluções **SaaS completas**, com forte foco em observabilidade como serviço (metrics, logs, traces, synthetics, APM), integração com centenas de tecnologias e interface unificada, com foco em **performance de aplicações e experiência do usuário final**. São geralmente mais abrangentes que o OpMon em termos de APM e suporte a instrumentação automática, mas exigem orçamentos mais altos.

O Zabbix, por sua vez, tem um modelo mais próximo do OpMon, sendo uma solução open source robusta para monitoramento de rede e infraestrutura, com foco em escalabilidade, alertas e desempenho. A principal diferença é que o Zabbix tem uma **comunidade internacional enorme e arquitetura baseada em agentes**, enquanto o OpMon foca mais no mercado brasileiro e em uma integração mais “turn-key” com visualização voltada ao negócio.

Portanto, o OpMon **é comparável em finalidade**, mas seu posicionamento está mais próximo de ferramentas como **Zabbix e Datadog**, combinando recursos de monitoramento com usabilidade empresarial e suporte local. Já Grafana Stack, Elastic Stack e New Relic oferecem maior customização e profundidade, especialmente em ambientes que exigem alta observabilidade distribuída.
