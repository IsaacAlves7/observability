<a href="https://github.com/IsaacAlves7/observability"><img src="https://github.com/user-attachments/assets/30c91eae-98e9-486d-b383-1ea3b393f553"></a>

> Versículo chave: "Consagre ao Senhor tudo o que você faz, e os seus planos serão bem-sucedidos." - Provérbios 16:3

# It's a repository of Observability from scratch 🔍
<img src="https://img.shields.io/badge/Grafana_Stack-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white"> <img src="https://img.shields.io/badge/Datadog-25.3.2-632CA6?style=flat&logo=Datadog&logoColor=white"> <a href="https://www.instagram.com/_eth0_/"><img src="https://img.shields.io/badge/Elastic_Stack-25.3.2-005571?style=flat&logo=Elastic&logoColor=white"></a> <img src="https://img.shields.io/badge/Graylog-25.3.2-FF3633?style=flat&logo=Graylog&logoColor=white"> <img src="https://img.shields.io/badge/NewRelic-25.3.2-1CE783?style=flat&logo=NewRelic&logoColor=white"> 

<a href="https://medium.com/@osomudeyazudonu/15-automation-scripts-for-monitoring-and-logging-every-devops-engineer-must-know-e92cd20111fe?source=email-afeafff77325-1737696271889-digest.reader--e92cd20111fe----14-99------------------61b76857_92a7_4fdc_86c4_ad47d198acad-1"><img src="https://em-content.zobj.net/source/microsoft-teams/400/magnifying-glass-tilted-left_1f50d.png" align="right" height="77"></a>

A **observabilidade** (observability) é um conceito fundamental em engenharia de sistemas e DevOps, que se refere à capacidade de entender o que está acontecendo dentro de um sistema complexo através da coleta, agregação e análise de seus dados de desempenho e operação. A ideia central é fornecer visibilidade e insights sobre o estado interno do sistema com base nas saídas externas. 

Observabilidade refere-se à capacidade de monitorar, mensurar e entender o estado de um sistema ou aplicação por meio da análise de seus resultados, logs e métricas de desempenho. Em sistemas de software modernos e na cloud computing, a observabilidade desempenha um papel de extrema importância, por garantir confiabilidade, desempenho e segurança a aplicações e a infraestrutura.

Essa maior importância da observabilidade hoje pode ser atribuída a fatores como: o aumento da complexidade dos sistemas de software, a adoção difundida dos microsserviços e a crescente dependência das arquiteturas distribuídas.

> "Quem não é visto, não é lembrado, Quem não é lembrado, acaba sendo esquecido." - Patrick Münzfeld

A observabilidade absorve e estende os sistemas de monitoramento clássicos e ajuda as equipes a identificarem a causa raiz dos problemas. Por ela, os stakeholders também esclarecem dúvidas sobre suas aplicações e negócios, como, por exemplo, previsões sobre possíveis erros. Um conjunto diversificado de ferramentas e tecnologias usadas hoje leva a uma grande matriz de possibilidades de implantação. Isso traz consequências arquitetônicas, portanto as equipes precisam saber configurar seus sistemas de observabilidade de maneira que sejam funcionais para elas. 

Observabilidade e monitoramento são conceitos relacionados, mas têm algumas diferenças importantes. A observabilidade refere-se à capacidade de fazer perguntas sobre seu sistema examinando seu comportamento de fora. Fazer um sistema e não saber seu rendimento é como "dar tiro no próprio pé" ou "pilotar um veículo sem painel" na vida de qualquer desenvolvedor de software.

O **monitoramento** é a prática estabelecida há décadas. Ele opera com uma lógica reativa e baseada em checagens pré-definidas. Você, como engenheiro, decide antecipadamente o que é importante e configura ferramentas para vigiar esses pontos específicos: "O servidor está consumindo mais de 90% de CPU?", "A taxa de erro do endpoint de pagamento está acima de 0,1%?", "O disco do banco de dados está com menos de 10% de espaço livre?". São perguntas essenciais, mas conhecidas. O monitoramento é excelente para alertar quando um dos itens da sua lista de preocupações conhecidas sai do esperado. Ele é sobre encontrar respostas para perguntas que você já sabia que precisava fazer. 

> Monitorar tudo pode parecer útil, mas às vezes menos é mais.

<img src="https://em-content.zobj.net/source/microsoft-teams/400/microscope_1f52c.png" align="right" height="77">

A observabilidade, por outro lado, é uma propriedade do sistema e uma filosofia proativa. Ela não se limita a verificar métricas pré-definidas; ela se preocupa em instrumentar o sistema de forma a gerar dados ricos e correlacionáveis (os famosos "três pilares": métricas, logs e traces distribuídos) que permitam investigar o comportamento interno a posteriori, sem ter que recriar o problema. A observabilidade entra em cena justamente quando você se depara com o inesperado, o novo, o bizarro. Ela responde à pergunta: "Meu sistema está se comportando de forma estranha e não tenho ideia do porquê. Como eu investigo isso?".

A diferença crucial está no fluxo de trabalho. O monitoramento grita: "Algo que eu conheço está errado!". A observabilidade sussurra: "Aqui estão todos os dados. Agora, faça as perguntas certas para descobrir o que há de errado, mesmo que você não soubesse que isso poderia acontecer."

E é aí que a sua frase final ganha um peso ainda maior. Desenvolver um software sem se preocupar com sua observabilidade é como construir um avião sem colocar instrumentos no painel. Você pode ter construído a aeronave mais bela e aerodinâmica do mundo, mas, uma vez no ar, sem altímetro, sem bússola, sem indicador de combustível e sem os registros de telemetria (os "dados ricos"), você está voando cego. Qualquer problema — uma turbulência inesperada, um consumo anormal de combustível, uma falha de motor — se torna uma catástrofe imprevisível e inexplicável. Você não consegue diagnosticar, muito menos corrigir a rota.

Portanto, a evolução natural é: o monitoramento é um subproduto, uma aplicação, de um sistema observável. Quando você tem um sistema verdadeiramente observável — com logs contextuais, métricas detalhadas e traces que mapeiam o caminho de uma requisição por todos os microservícies —, você pode então configurar alertas de monitoramento muito mais inteligentes e contextuais. Mais do que isso, você empodera seus desenvolvedores a não apenas apagar incêndios, mas a entender profundamente o comportamento do sistema, antever problemas e criar softwares mais resilientes. Em resumo, a observabilidade não substitui o monitoramento; ela o eleva de uma simples checklist de verificação para uma ferramenta de investigação e descoberta contínua, tornando o "tiro no pé" não apenas doloroso, mas evitável.

À medida que mais organizações adotam a infraestrutura nativa da nuvem, é provável que a necessidade de ferramentas de observabilidade projetadas especificamente para esses ambientes cresça. As ferramentas de observabilidade nativas em nuvem são projetadas para coletar e analisar dados de microsserviços, contêineres e outras tecnologias nativas em nuvem e fornecer insights sobre o desempenho do sistema nesses ambientes.

Em poucas palavras, a observabilidade nativa da nuvem é uma prática de monitoramento, análise e solução de problemas de aplicativos modernos e nativos da nuvem criados usando arquitetura de microsserviços e implantados em contêineres ou ambientes sem servidor. 

A observabilidade baseia-se em três pilares principais:

<img src="https://user-images.githubusercontent.com/61624336/172407209-627822a2-0a5f-4778-b58e-954481ee788b.gif" align="right" height="77">

1. **Logs** (Diagnósticos): Registros detalhados de eventos que ocorrem dentro do sistema. Logs fornecem um histórico cronológico das atividades do sistema e são úteis para diagnosticar problemas específicos, entender a sequência de eventos e rastrear bugs. É todo o diagnóstico preciso dentro do sistema.

2. **Métricas** (Detectar): Dados numéricos que representam o desempenho do sistema. Métricas podem incluir o uso de CPU, memória, taxa de erros, latência de solicitações, entre outros. Elas ajudam a monitorar a saúde do sistema e a identificar tendências ou anomalias. É tudo aquilo que foi detectado no sistema.

3. **Traços** (Isolar e melhorar): Informações sobre a execução de solicitações e transações através de diferentes componentes do sistema. Traços mostram como as solicitações se propagam pelo sistema, permitindo a identificação de gargalos, pontos de falha e a compreensão do fluxo de trabalho completo. Os Traços (Traces) são rastreamentos distribuídos que seguem o caminho de uma solicitação através de vários serviços e componentes de um sistema, ajudam a isolar e melhorar problemas em sistemas distribuídos, permitindo identificar gargalos de desempenho e falhas em componentes específicos. O rastreamento é focado na coleta de dados sobre a execução de solicitações ou transações em seu ambiente e aplicativos Kubernetes. Os rastreamentos podem ajudá-lo a entender como as solicitações ou transações são processadas por seus aplicativos, identificar problemas de desempenho e otimizar o desempenho do aplicativo.

> Além desses três pilares principais, temos os **Eventos** que é focado na coleta de dados sobre eventos importantes que ocorrem em seu ambiente Kubernetes, como implantações de aplicativos, eventos de dimensionamento e erros. Os eventos podem ajudá-lo a monitorar a integridade do seu ambiente Kubernetes e responder rapidamente aos problemas à medida que eles surgem.

A observabilidade é fundamentalmente a intersecção prática entre a ciência de dados e as disciplinas de DevOps e DevSecOps, representando a materialização operacional de princípios científicos aplicados à complexidade dos sistemas distribuídos contemporâneos.

<a href="https://medium.com/cloud-native-daily/7-best-tracing-tools-for-microservices-27a5e3bc4b9c"><img height="177" align="right" src="https://github.com/user-attachments/assets/64217819-653f-4a74-86e8-291b1bf3d5ec" /></a>

Entrando mais a fundo no terceiro pilar da observabilidade, o **rastreamento distribuído** (<a href="https://javascript.plainenglish.io/9-best-distributed-tracing-tools-for-developers-185e415b7101">distributed tracing</a>) é um método usado para criar o perfil ou monitorar o resultado de uma solicitação executada em um sistema distribuído. Monitorar um sistema distribuído pode ser desafiador porque cada ponto central individual tem seu próprio fluxo de logs e de métricas. 

Para obter uma visão precisa de um sistema distribuído, essas métricas de pontos centrais diferentes precisam ser agregadas em uma visão abrangente. As solicitações para sistemas distribuídos, em geral, não acessam todo o conjunto de pontos centrais dentro do sistema, mas acessam um conjunto parcial ou um caminho através dos pontos centrais. O <a href="https://youtu.be/CqLB-tBYB2Q">rastreamento distribuído</a> ilumina os caminhos acessados com frequência por meio de um sistema distribuído e permite que as equipes analisem e monitorem esses caminhos. O rastreamento distribuído é instalado em cada ponto central do sistema e, em seguida, permite que as equipes consultem o sistema para obter informações sobre a integridade do ponto central e o desempenho da solicitação.

- **Revela dependências de serviço**: A decisão estratégica foi tomada: sua empresa começou a migrar para uma arquitetura distribuída, o número de componentes começou a aumentar e a capacidade de entender a arquitetura da organização diminuiu; aplicando o rastreamento distribuído, você pode rastrear o caminho de uma requisição à medida que ela passa por um sistema complexo. Algumas ferramentas até calculam e desenham um grafo de dependência completo. Pode ser útil ter uma visão geral de sua arquitetura e mergulhar profundamente para entender melhor as dependências.

- **Descubra a latência dos componentes ao longo do caminho**: Você pode descobrir a latência monitorando requisições de **serviços de borda** (edge services) usando sistemas de monitoramento. OK, você recebeu o alerta, mas agora precisa descobrir qual componente faz com que a solicitação específica exceda o **Service Level Objective** (SLO). É exatamente por isso que o rastreamento distribuído existe: para localizar componentes no caminho que são gargalos ou passíveis de causar falhas.

- **Análise de causa raiz**: Imagine o seguinte cenário – você acorda com um alerta, são 2h da manhã e uma requisição envolvendo 5 microsserviços diferentes está falhando repetidamente. Você procura desesperadamente nos logs, ainda tentando abrir os olhos contra a tela ultra iluminada, em busca de erros na hora do alerta, mas o fluxo de dados é gigantesco demais para descobrir com precisão e rapidez o que aconteceu. Está demorando demais. Pois bem: usando o rastreio distribuído, é possível encontrar o primeiro serviço que falhou, obter os logs dessa falha e algumas outras coisas mais (a depender da implementação de rastreio feita no sistema).

- **Colete eventos durante a requisição**: Para ajudar no processo de debug, é possível adicionar elementos ao rastreamento. Por exemplo, você pode adicionar todas as feature flags avaliadas ao rastreamento para que, em caso de falha, possa saber exatamente quais flags foram avaliadas em cada um dos serviços no caminho da requisição.

Vamos começar com o básico, de onde todas as soluções de rastreamento distribuídas se originaram. Embora antes houvesse algumas soluções de rastreamento distribuído, o artigo entitulado <a href="https://static.googleusercontent.com/media/research.google.com/en//archive/papers/dapper-2010-1.pdf">Google Dapper (2010)</a>, de 14 páginas, é a pedra angular do rastreamento distribuído, por assim dizer. O documento trata de explicar como o Google desenvolveu uma ferramenta de rastreamento em nível de produção, tendo em vista 3 objetivos principais:

A observabilidade permite às equipes de engenharia de software detectar, diagnosticar e resolver problemas mais rapidamente, melhorar a estabilidade e o desempenho do sistema, e fornecer uma base para melhorias contínuas. **Plataformas/Ferramentas de observabilidade**, como Prometheus, Grafana, Jaeger e Splunk, são um conjunto de sistemas que podem coletar, processar, analisar e visualizar sinais de telemetria, incluindo métricas, logs e rastreamentos. As plataformas de observabilidade incluem New Relic, Splunk, Datadog, Grafana Stack, e Apache JMeter. Essas ferramentas de observabilidade de código aberto, como Grafana, Jaeger, Kafka, OpenTelemetry e Prometheus, tornaram-se cada vez mais populares nos últimos anos, e essa tendência provavelmente continuará. Isso é parcialmente impulsionado pelo desejo de reduzir os custos associados às ferramentas proprietárias de observabilidade e às opções de flexibilidade e personalização oferecidas pelas ferramentas de código aberto.

Portanto, são comumente usadas para implementar essas práticas. Em resumo, a observabilidade é crucial para a manutenção e operação eficiente de sistemas modernos, especialmente em arquiteturas distribuídas e baseadas em microsserviços. Então, logging, monitoring e observabilidade são partes essenciais do ciclo de vida de desenvolvimento, implantação e operação de software. Eles estão relacionados à fase de operação contínua (ou operação) e monitoramento no ciclo de vida do DevOps e CI/CD. 

Continuous Integration (CI): Visão ampliada

<img height="177" align="right" src="https://github.com/user-attachments/assets/48b293ce-e582-4d58-8536-8ce6cdaeb03b" />

  - Logging: Durante a fase de integração contínua, logs são gerados para registrar o progresso da construção, testes e integração do código. Eles ajudam a identificar e resolver problemas de build e erros de integração.

  - Monitoring: Nesta fase, o monitoramento pode ser usado para acompanhar o desempenho das builds, uso de recursos do CI server, e saúde dos serviços de CI.

  - Observabilidade: Não é um foco principal nesta fase, mas alguns aspectos podem ser monitorados para melhorar a eficiência e detectar problemas nos pipelines de CI.

Continuous Delivery/Deployment (CD): Visão periférica

<img height="177" align="right" src="https://github.com/user-attachments/assets/3342bc19-b756-4539-b5eb-56bbcd622e2f" />

  - Logging: Logs são cruciais durante a fase de deployment para registrar as atividades de implementação, mudanças de configuração e qualquer problema que ocorra durante o processo. Eles permitem o rastreamento de quem fez o que e quando.

  - Monitoring: O monitoramento é intensificado para garantir que as novas versões sejam implementadas sem causar interrupções ou degradação de desempenho. Ferramentas de monitoramento verificam a disponibilidade dos serviços, tempos de resposta e outros indicadores de desempenho.

  - Observabilidade: A observabilidade começa a ter um papel mais importante, ajudando a entender o comportamento do sistema pós-deployment, identificar possíveis regressões e garantir que todas as partes do sistema estejam funcionando conforme esperado.

Nas etapas/fases de Operações e Monitoramento: Visão espacial

<img height="177" align="right" src="https://github.com/user-attachments/assets/37bea0f6-185b-4c91-95a0-204ba66b4860" />

  - Monitoring: O monitoramento contínuo do sistema em produção garante que o serviço esteja funcionando corretamente e permite a detecção proativa de problemas. Isso inclui a monitorização de métricas como uso de CPU, memória, latência, taxas de erro, etc.

  - Observabilidade: A observabilidade aqui é fundamental para obter uma visão abrangente do estado do sistema. Utiliza logs, métricas e traços para proporcionar uma compreensão profunda de como o sistema está operando, identificar anomalias, realizar análises de causa raiz e otimizar o desempenho.

Em resumo, enquanto logging e monitoring são utilizados em todas as fases do CI/CD, a observabilidade se torna especialmente crítica na fase de operações e monitoramento, onde a complexidade e a necessidade de insights detalhados sobre o sistema são maiores.

<img width="656" height="853" alt="unnamed" src="https://github.com/user-attachments/assets/9a838911-43b3-4c65-af67-fc3f3a9d81fa" />

No contexto do DevOps, a observabilidade geralmente é considerada uma prática que abrange várias etapas do ciclo de vida do software. Ela envolve a capacidade de compreender o comportamento interno de um sistema com base em suas saídas externas. Isso inclui métricas, registros (logging), rastreamentos (traces) e outras formas de dados que fornecem insights sobre o funcionamento de um sistema. Portanto, logging, monitoring e observabilidade estão presentes em várias etapas do processo de desenvolvimento e implantação de software:

<img height="177" align="right" src="https://github.com/user-attachments/assets/77fefcf5-4e9f-4bfa-ad2c-1cdd85c92456" />

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

<img src="https://em-content.zobj.net/source/microsoft-teams/400/page-facing-up_1f4c4.png" align="right" height="77">

- <a href="">NLog</a>: é uma biblioteca para C-Sharp.

- <a href="">Serilog</a>: é uma biblioteca para .NET.

- <a href="">Apache Log4J</a>: é uma biblioteca de logging de código aberto muito popular em sistemas Java. Ele é usado para registrar informações de eventos em aplicativos, ajudando os desenvolvedores a rastrear problemas, entender o fluxo de execução do código e monitorar o comportamento do sistema em tempo real.

- <a href="">Winston</a>: é uma biblioteca de log para Node.js.

- <a href="">Monolog</a>: É uma biblioteca de log para PHP.

- <a href="">Graylog</a>: é uma plataforma de gerenciamento de logs de código aberto que ajuda na coleta, armazenamento, análise e visualização de registros de diferentes fontes. Ele oferece uma solução integrada para lidar com logs de várias fontes, permitindo que as equipes de operações e desenvolvimento monitorem e analisem informações cruciais dos sistemas.

<img height="177" align="right" src="https://github.com/user-attachments/assets/7682458c-7491-445a-962e-0e8ec050f957" />

**Monitoring**: Pode ser que aconteça outros casos também, vamos supor que seu servidor vai ficar sem internet ou desligado ou ficar travado e você não vai estar tomando nenhum erro, mas os usuários não vão conseguir acessar, o que você pode fazer pra entender esse tipo de situação é utilizar um serviço de **health check** (checagem de saúde), ele pode não só ver se sua URL do site está em pé, mas também fazer uma consulta no banco. Veja as soluções abaixo:

- <a href="">UptimeRobot</a>: é um serviço online grátis que monitora a disponibilidade e o desempenho de sites, servidores, serviços web e outros recursos online. Ele verifica regularmente os recursos cadastrados e notifica os usuários caso haja qualquer interrupção ou queda de disponibilidade.

- <a href="">Site 24x7</a>: é uma plataforma de monitoramento e gerenciamento de TI baseada em nuvem que fornece uma gama abrangente de ferramentas para monitorar o desempenho de sites, servidores, aplicações e infraestruturas de rede.

- <a href="">Pingdom</a>: é um serviço de monitoramento de desempenho e disponibilidade de sites e aplicações web. Ele ajuda as empresas a garantir que seus sites e serviços estejam sempre disponíveis e operando com desempenho ideal.

Esta folha de dicas oferece uma comparação concisa, porém abrangente, dos principais elementos de monitoramento entre os três principais provedores de nuvem e ferramentas de código aberto/terceiros:

![unnamed](https://github.com/user-attachments/assets/d58727c3-5b89-40c9-ac83-2504095c6c0a)

Vamos explorar os aspectos essenciais do monitoramento abordados:

1. Coleta de Dados: Colete informações de fontes diversas para aprimorar a tomada de decisões.
2. Armazenamento de Dados: Armazenar e gerenciar os dados com segurança para análise e referência futuras.
3. Análise de Dados: Extraia insights valiosos dos dados para impulsionar ações informadas.
4. Alertas: Receba notificações em tempo real sobre eventos ou anomalias críticas.
5. Visualização: Apresente dados em um formato visualmente compreensível para melhor compreensão.
6. Relatórios e Conformidade: Gere relatórios e garanta a conformidade com os padrões regulatórios.
7. Automação: Otimize processos e tarefas por meio de fluxos de trabalho automatizados.
8. Integração: Conecte e troque dados de forma fluida entre diferentes sistemas ou ferramentas.
9. Ciclos de Feedback: Refinar continuamente estratégias com base em feedback e análise de desempenho.

> Com você: como você prioriza e aproveita esses aspectos essenciais de monitoramento em sua área para alcançar melhores resultados e eficiência?

Por que o monitoramento do Amazon Prime Video passou de serverless para monolítico? Como isso pode economizar 90% do custo?

O diagrama abaixo mostra a comparação de arquitetura antes e depois da migração:

![unnamed](https://github.com/user-attachments/assets/8c461e1d-f32b-4741-946e-e1e4df23637a)

O que é o Serviço de Monitoramento Amazon Prime Video? O serviço Prime Video precisa monitorar a qualidade de milhares de transmissões ao vivo. A ferramenta de monitoramento analisa automaticamente os fluxos em tempo real e identifica problemas de qualidade como corrupção de blocos, congelamento de vídeo e problemas de sincronização. Esse é um processo importante para a satisfação do cliente.

São 3 etapas: conversor de mídia, detector de defeitos e notificação em tempo real.

Qual é o problema com a arquitetura antiga?

A arquitetura antiga era baseada na Amazon Lambda, que era boa para serviços de construção rapidamente. No entanto, não era econômico ao rodar a arquitetura em grande escala. As duas operações mais caras são:

1. O fluxo de trabalho de orquestração - as funções step da AWS cobram os usuários por transições de estado e a orquestração executa múltiplas transições de estado a cada segundo.

2. Passagem de dados entre componentes distribuídos - os dados intermediários são armazenados no Amazon S3 para que a próxima etapa possa ser baixada. O download pode ser caro quando o volume está alto.

A arquitetura monolítica economiza 90% de custo. Uma arquitetura monolítica é projetada para resolver os problemas de custo. Ainda existem 3 componentes, mas o conversor de mídia e o detector de defeitos são implantados no mesmo processo, economizando o custo de passar dados pela rede. Surpreendentemente, essa abordagem para a mudança na arquitetura de implantação resultou em uma economia de custos de 90%!

Este é um estudo de caso interessante e único, pois os microserviços se tornaram uma escolha de referência e na moda na indústria de tecnologia. É bom ver que estamos tendo mais discussões sobre evoluir a arquitetura e ter discussões mais honestas sobre seus prós e contras. Decompor componentes em microserviços distribuídos tem um custo.

O que os líderes da Amazon disseram sobre isso? 

> CTO da Amazon, Werner Vogels: "Construir sistemas de software evolutivos é uma estratégia, não uma religião. E revisitar suas arquiteturas com mente aberta é obrigatório."

> Ex-vice-presidente de Sustentabilidade da Amazon, Adrian Cockcroft: "A equipe do Prime Video seguiu um caminho que chamo de Serverless First... Eu não defendo o uso apenas de servidores".

A palavra é sua: a arquitetura de microserviços resolve um problema de arquitetura ou um problema organizacional?

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

Como detectamos falhas de nós em sistemas distribuídos? O diagrama abaixo mostra os 6 principais mecanismos de detecção de batimentos cardíacos.

![unnamed](https://github.com/user-attachments/assets/64882059-6690-4d42-ba8d-39570cbe575f)

Os mecanismos do batimento cardíaco são cruciais em sistemas distribuídos para monitorar a saúde e o estado de vários componentes. Aqui estão vários tipos de mecanismos de detecção de batimentos cardíacos comumente usados em sistemas distribuídos:

- Batimentos cardíacos baseados em Push A forma mais básica de batimento cardíaco envolve um sinal periódico enviado de um nó para outro ou para um serviço de monitoramento.
Se os sinais de batimentos cardíacos pararem de chegar dentro de um intervalo especificado, o sistema assume que o nó falhou. Isso é simples de implementar, mas a congestão da rede pode levar a falsos positivos.

- Batimentos cardíacos baseados em puxada Em vez de os nós enviarem batimentos cardíacos ativamente, um monitor central pode periodicamente "puxar" informações de status dos nós.
Reduz o tráfego de rede, mas pode aumentar a latência na detecção de falhas.

- Batimentos cardíacos com Verificação de Saúde: Inclui informações diagnósticas sobre a saúde do nódulo no sinal do batimento cardíaco. Essas informações podem incluir uso de CPU, uso de memória ou métricas específicas da aplicação. Fornece informações mais detalhadas sobre o nó, permitindo decisões mais nuançadas. No entanto, isso aumenta a complexidade e o potencial para maior overhead de rede.

- Batidas cardíacas com carimbos de tempo Batidas que incluem carimbos de tempo podem ajudar o nó ou serviço receptor a determinar não apenas se um nó está ativo, mas também se há atrasos na rede afetando a comunicação.

- Batimentos cardíacos com reconhecimento: O receptor da mensagem de batimento cardíaco deve enviar um reconhecimento neste modelo. Isso garante que não apenas o remetente esteja vivo, mas que o caminho de rede entre o remetente e o receptor também seja funcional.

- Batimentos cardíacos com quórum: Em alguns sistemas distribuídos, especialmente aqueles que envolvem protocolos de consenso como Paxos ou Raft, é utilizado o conceito de quórum (a maioria dos nós). Batimentos cardíacos podem ser usados para estabelecer ou manter um quórum, garantindo que um número suficiente de nós esteja operacional para que o sistema tome decisões. Isso traz complexidade na implementação e no gerenciamento das mudanças de quórum, à medida que os nós entram ou saem do sistema.

<img height="177" alt="james-web-telescope-3d-icon-png-download-4514240" align="right" src="https://github.com/user-attachments/assets/618add6e-8cde-48f0-bfc7-4d1dec6e1fd5" />

Os **mecanismos de busca** e **SEO** são úteis em observabilidade, isso é um insight extremamente perspicaz e que vai direto ao cerne de um dos maiores desafios na observabilidade moderna. A comparação entre mecanismos de busca e SEO com a prática da observabilidade não é apenas uma analogia interessante; ela representa uma mudança fundamental na forma como equipes precisam pensar sobre seus dados operacionais. A utilidade reside precisamente em abordar o problema do volume massivo de dados e da complexidade inerente aos sistemas distribuídos atuais.

A observabilidade gera uma quantidade astronômica de dados: trilhões de logs, métricas e traces que, por si só, são inúteis se não puderem ser explorados e compreendidos de forma eficiente. Um mecanismo de busca tradicional, como o Google, não se limita a armazenar páginas da web; ele as indexa, cria um ranking de relevância e fornece uma interface simples onde uma consulta complexa retorna resultados ordenados pela probabilidade de atender à sua necessidade. Da mesma forma, uma plataforma de observabilidade moderna precisa ser, antes de tudo, um mecanismo de busca extremamente eficiente sobre seus dados de telemetria. A capacidade de um engenheiro digitar "erro de timeout no serviço de pagamento" e, em segundos, receber não apenas os logs relevantes, mas também os traces das transações afetadas, os gráficos de métricas de latência do banco de dados e até mesmo uma sugestão de causa raiz, é o equivalente funcional a uma pesquisa bem-sucedida no Google. A alternativa — saber qual exatamente arquivo de log procurar, em qual servidor, e qual query exata escrever em um banco de dados de logs — é o equivalente a ter que navegar manualmente em um diretório da web sem um motor de busca.

É aí que o "SEO" entra na equação. Em um website, o Search Engine Optimization é o conjunto de práticas que você adota para garantir que seu conteúdo seja compreensível, bem estruturado e, portanto, facilmente encontrável pelo algoritmo do mecanismo de busca. Na observabilidade, o "SEO" são as convenções, padrões e boas práticas de instrumentação que as equipes de desenvolvimento adotam para que seus dados sejam "encontráveis" pela plataforma e pelos colegas. Isso inclui a padronização de atributos e tags em spans de tracing, como usar `service.name`, `http.status_code` e `db.operation` de forma consistente em todos os serviços. Inclui a estruturação de logs de forma a extrair campos-chave como `user_id`, `transaction_id` e `error_code`, em vez de depender de strings de texto livre. Também envolve a enriquecimento de métricas com labels padronizadas que permitem agregação e filtro eficientes, como `environment=production`, `region=us-east-1` e `version=v2.1.5`.

Sem esse "SEO interno", os dados de observabilidade se tornam uma coleção de silos desconexos e de difícil consulta. Um engenheiro investigando um problema pode saber que a resposta está em algum lugar nos logs, métricas e traces, mas não conseguirá conectá-los rapidamente. Uma consulta por `transaction_id=xyz` pode funcionar nos logs, mas falhar nos traces se o atributo estiver nomeado como `trace_id` em um serviço e `correlation_id` em outro. A falta de padronização quebra a capacidade de "navegar" pelos dados de forma correlacionada, que é a essência da observabilidade. As plataformas mais avançadas, como o Dynatrace mencionado anteriormente, tentam automatizar parte dessa correlação, mas a eficácia máxima é alcançada quando a automatização da plataforma encontra a disciplina e a padronização das equipes humanas.

Portanto, a mentalidade de mecanismo de busca e SEO é fundamental porque reorienta o foco da simples coleta de dados para a *descoberta de insights*. A métrica de sucesso deixa de ser "quantos terabytes de logs armazenamos" e passa a ser "em quanto tempo um engenheiro consegue encontrar a causa raiz de um problema desconhecido". Em um sistema complexo, ninguém sabe antecipadamente todas as perguntas que precisarão ser respondidas. A observabilidade, assim como a web, é um universo de informações que você precisa ser capaz de explorar sem um mapa pré-definido. Os mecanismos de busca fornecem a interface para essa exploração, e o SEO — a disciplina de instrumentação — garante que o "conteúdo" do seu sistema seja de alta qualidade, bem estruturado e, consequentemente, encontrável no momento de maior pressão, que é durante um incidente.

<img height="177" align="right" src="https://github.com/user-attachments/assets/d49622ad-36d9-43b0-af5e-2b59aa8c5019" />

Quando pensamos em mecanismos de busca e SEO, normalmente o imaginário fica preso ao marketing digital e à forma como sites se posicionam na web. Mas dentro do universo da observabilidade esses conceitos encontram uma utilidade muito interessante e até estratégica. A essência da observabilidade é tornar visível e acessível o que está acontecendo nos sistemas, e isso gera um mar de dados: logs em enormes volumes, métricas em séries temporais, traces distribuídos detalhando cada requisição, além de documentação técnica e relatórios internos. Sem uma forma eficiente de buscar, filtrar e priorizar essa informação, a observabilidade se transforma em um labirinto de dados brutos. É aí que entram mecanismos de busca e até mesmo a mentalidade de SEO aplicada internamente.

Ferramentas como Elasticsearch, Splunk ou Loki funcionam como “motores de busca para observabilidade”. Elas permitem indexar logs e eventos em tempo real, de modo que engenheiros consigam pesquisar rapidamente por termos, padrões, IDs de correlação ou até mensagens de erro específicas. É como se você tivesse um Google voltado para os bastidores da sua aplicação. Além disso, conceitos de SEO entram de forma adaptada: estruturar logs e métricas com campos consistentes, nomes padronizados e metadados bem definidos aumenta a “encontrabilidade” das informações, tornando as consultas mais precisas e reduzindo o tempo de detecção e resolução de incidentes. Nesse sentido, dar “otimização de busca” aos dados de observabilidade não tem a ver com ranquear páginas, mas sim com facilitar a descoberta e priorização daquilo que importa dentro de um oceano de informações.

Essa perspectiva também se aplica à documentação e ao compartilhamento de conhecimento dentro de equipes. Muitas vezes, quando um erro recorrente aparece, alguém já escreveu uma análise ou uma runbook interna explicando como lidar com ele. Se esses registros não são fáceis de encontrar, eles perdem valor. Usar princípios de SEO internos — títulos claros, descrições concisas, palavras-chave adequadas nos documentos técnicos — garante que engenheiros, ao buscarem por determinado erro ou serviço, encontrem de imediato o guia certo. Assim, mecanismos de busca somados a uma “cultura de SEO para observabilidade” funcionam como aceleradores de incident response, reduzindo MTTR (Mean Time to Recovery) e aumentando a maturidade do time.

<img height="177" align="right" src="https://github.com/user-attachments/assets/5c1fe7aa-d923-4bd9-8d1c-3c8c66c0e93a" />

Especialmente pra quem vem do universo de Observability e começa a transitar também por **Product Analytics** ou **Digital Analytics**. A resposta curta é: não são a mesma coisa, mas podem se complementar profundamente, dependendo do contexto e da maturidade da empresa. Vamos por partes:

*Observabilidade (Observability)* é um conceito originado da engenharia de software e da confiabilidade de sistemas. Ela se baseia em três pilares principais são logs, métricas e traces, e serve para responder perguntas como: *“O sistema está funcionando como esperado?”*, *“Por que o serviço X está lento?”* ou *“Qual parte do pipeline de dados falhou?”*. 

Ferramentas típicas de observabilidade incluem **Elastic Stack (ELK)**, **Prometheus**, **Grafana**, **Jaeger**, **OpenTelemetry**, **Datadog**, **New Relic**, **Dynatrace**, entre outras. Ou seja, o foco da observabilidade é técnico e operacional: acompanhar a **saúde**, **performance**, **latência**, **erros** e **comportamento interno** das aplicações e infraestruturas.

Já as **ferramentas de Analytics** como **Google Analytics, Amplitude, Mixpanel, Pendo, Heap, PostHog**, entre outras, são orientadas a *produto e negócio*. Elas servem para responder perguntas como: *“Quantos usuários clicaram nesse botão?”*, *“Qual fluxo de onboarding tem mais abandono?”*, *“Qual cohort de clientes retém mais?”* ou *“Qual feature está gerando mais conversão?”*. Em suma, o foco é **comportamento do usuário, funis de conversão, engajamento e retenção**.

Agora, a conexão entre os dois mundos começa a surgir quando a empresa amadurece e percebe que **a experiência do usuário final e a performance técnica estão interligadas**. Por exemplo, uma queda de conversão observada no Mixpanel pode ter como causa uma lentidão no back-end detectada pelo Grafana. Ou uma alta taxa de erro no Kibana pode estar impactando o evento “checkout_completed” rastreado no Amplitude. 

Nesse ponto, começa o que chamamos de **Observabilidade orientada a produto (Product Observability)**, um conceito emergente que une o melhor dos dois mundos: dados técnicos e dados de uso do usuário.

Em pipelines modernos, é comum integrar essas duas visões. Por exemplo:

<img height="177" align="right" src="https://github.com/user-attachments/assets/5cc1ec4e-e9fb-47a9-b82a-4d8a8121ba1a" />

* Logs de erro e traces (Elastic / OpenTelemetry) podem ser correlacionados com eventos de analytics (Amplitude / Mixpanel).
* Métricas de performance (Prometheus / Grafana) podem alimentar painéis junto com KPIs de produto.
* Dados de sessão (Google Analytics / PostHog) podem ser enriquecidos com dados de infraestrutura em Data Lakes unificados (S3, BigQuery, Snowflake).

Portanto, Analytics e Observability são domínios distintos, técnico vs comportamental, mas complementares. Enquanto a observabilidade te mostra *o que está acontecendo dentro* do sistema, o analytics te mostra *como o usuário está reagindo fora dele*. Quando unidos, fornecem uma visão 360° tanto do produto quanto de sua operação.

Se você trabalha com observabilidade (Elastic, Prometheus, Grafana) e quer expandir para o lado de Analytics, o caminho natural é começar a estudar **instrumentação de eventos**, **telemetria de comportamento**, **cohort analysis** e **funnel tracking**, para depois pensar em como cruzar esses dados técnicos e de produto em um mesmo observability pipeline.

<img height="177" align="right" src="https://github.com/user-attachments/assets/91e023ab-a13e-4f26-8d1a-b9d7a2c1f068" />

Existem também várias ferramentas e plataformas que buscam exatamente isso: medir **tempo médio de visualização** ou **tempo completo assistido** por usuário em vídeos de uma plataforma de streaming VoD (Video on Demand). 

Por exemplo, a plataforma **Mux** oferece uma solução de analytics de vídeo focada em “viewer engagement” e “watch time”.

Se você está montando ou avaliando uma arquitetura para esse tipo de métrica, vale que você foque nos seguintes pontos:

* O sistema deve capturar eventos de reprodução, pausa, término, avanço, retrocesso, plataforma/dispositivo, identificação de usuário (ou sessão anônima), e tempo de play real.
* Esses eventos são normalmente enviados a um backend de analytics em tempo real ou quase real, onde são agregados por vídeo, por usuário, por sessão.
* A métrica “tempo completo assistido” exige definir o que significa “completou” — por exemplo, assistiu ≥ 90% do vídeo ou até o fim nominal — e registrar isso como um evento ou um atributo.
* Depois, para análise, você pode criar dashboards e relatórios que mostram “média de minutos assistidos por sessão”, “percentual médio de conclusão por vídeo”, “distribuição de duração assistida”, “drop-off por minuto da reprodução” etc.
* Finalmente, para tornar em uma solução industrial, pense em como integrar esses dados a painéis de BI, como parte de métricas de engajamento, retenção ou churn da plataforma.

Além da Mux, existem várias outras ferramentas que oferecem analytics para vídeo VoD (Video on Demand) e que podem monitorar métricas como tempo de visualização, completação, dispositivos usados, e comportamento do usuário. Abaixo listo algumas com breves descrições:

* Dacast — Oferece vídeos para streaming e VoD com dashboard de analytics em tempo real, incluindo “average time watching” por vídeo, localização, dispositivo e dados de consumo.

* api.video — Fornece endpoints de analytics para vídeos e transmissões ao vivo que permitem consultar “watch time”, número de reproduções, visualizações únicas, além de filtrar por dispositivo ou navegador.

* Kaltura — Plataforma de vídeo corporativo que inclui funcionalidades de VoD Analytics: minutos assistidos, taxa de conclusão, abandono em quartis, por vídeo/entrada. 

* Zype — Plataforma voltada para distribuidores de vídeo e streaming que oferece métricas de engajamento, tempo assistido, sessões simultâneas e segmentação por plataforma/domain.

* Wowza — Solução para vídeo online e streaming que menciona analytics tanto para vídeo ao vivo quanto VoD, com foco em qualidade de experiência e engajamento

Top 9 Cases Behind 100% CPU Usage
The diagram below shows common culprits that can lead to 100% CPU usage. Understanding these can help in diagnosing problems and improving system efficiency.

<img width="550" height="715" alt="unnamed" src="https://github.com/user-attachments/assets/8db9dbc4-4d9c-4093-b183-85b1648368d9" />

Infinite Loops

Background Processes

High Traffic Volume

Resource-Intensive Applications

Insufficient Memory

Concurrent Processes

Busy Waiting

Regular Expression Matching

Malware and Viruses

Over to you: Did we miss anything important?

## RCA - Root Cause Analysis
Vivência com análise de causa raiz (RCA), engenharia reversa e resolução de incidentes L2/L3; documentar e participar de RCA, runbooks, sessões shadow e troubleshooting, isso descreve um conjunto de práticas muito típicas de equipes de Suporte Técnico Avançado, SRE, Observabilidade, Operações, Sustentação de Sistemas e Engenharia de Plataforma. É basicamente a expectativa de que a pessoa sabe lidar com problemas complexos em produção, diagnosticar falhas profundas, entender sistemas que ela não construiu e registrar tudo isso para evitar que volte a acontecer.

A análise de causa raiz, ou RCA (Root Cause Analysis), é uma disciplina usada para investigar incidentes que geram falhas reais em sistemas, desde indisponibilidades a lentidão, perda de dados, quedas de serviços e bugs críticos. O objetivo não é apenas apagar o incêndio — isso normalmente é L1 ou o hotfix imediato — mas sim **entender por que o problema aconteceu**, qual foi o mecanismo exato da falha, qual caminho levou ao bug, qual processo quebrou e o que precisa ser corrigido para que a falha **não se repita**. Uma RCA bem feita envolve coletar métricas, logs, traces, histórico de deploys, configurações alteradas, erros silenciosos, exceções não tratadas, comportamento inesperado do sistema e até condições de corrida ou incidentes de infraestrutura. Ela tenta ir além da causa superficial (“timeout no banco”) e busca o motivo real (“uma query regressiva gerada por um ORM após um deploy mal testado saturou o pool de conexões e derrubou o serviço”). Em empresas sérias, RCA é um processo formal, documentado, com timeline, responsáveis, ações imediatas, ações preventivas e compromissos de follow-up.

Quando a vaga fala de engenharia reversa dentro desse contexto, não é no sentido de “hackear binários” ou invadir sistemas, mas sim no sentido corporativo: **entender como um sistema funciona sem ter a documentação original**, sem ter todos os responsáveis disponíveis, ou com partes do código obscuras e legado. É comum em times que lidam com incidentes em sistemas que já rodaram por anos: falta documentação, o dev original saiu da empresa, a arquitetura tem partes obscuras, ou existem comportamentos não óbvios. Fazer engenharia reversa nesse contexto significa olhar para logs, interações entre serviços, mensagens no RabbitMQ, chamadas GraphQL ou REST, consultas SQL e comportamento runtime, para reconstruir mentalmente o que está acontecendo. É ler o código com o olhar do detetive, traçar relações, identificar dependências e pistas e entender “como isso funciona de verdade” para poder consertar.

Os níveis L2 e L3 de resolução de incidentes representam níveis de profundidade técnica. L1 é aquele suporte básico que faz triagens, valida se o sistema está fora do ar, roda scripts e aciona equipes. L2 é o nível onde a pessoa já consegue **analisar logs, entender código, identificar problemas não triviais, reiniciar serviços com cautela, validar métricas e tentar diagnóstico inicial**. L3 é o nível mais profundo: **engenheiros que entendem o código-fonte, a arquitetura, as integrações, o banco de dados, o comportamento da aplicação em profundidade** e conseguem realmente propor e aplicar correções. O L3 é o nível responsável por resolver o problema de forma estrutural, não apenas contornar.

Quando falam de documentar e participar de RCA e runbooks, isso indica maturidade operacional. Um runbook é um documento vivo que explica como lidar com incidentes específicos, passo a passo, como se fosse um manual de ação: o que verificar quando o serviço X cai, como reiniciar o container sem causar downtime, como coletar logs, como validar integridade de dados, como rodar scripts de emergência, como escalar para outros times. O runbook transforma conhecimento tribal em conhecimento institucional, permitindo que novatos e níveis L1/L2 sigam procedimentos seguros sem depender do “dev sênior que sabe de tudo”.

Já as sessões shadow são um processo colaborativo onde alguém acompanha um engenheiro mais experiente para observar como ele investiga problemas, rastreia incidentes, consulta métricas, usa observabilidade e conduz RCA. É como uma mentoria prática. O objetivo é que o profissional aprenda na prática, assistindo a análise e depois repetindo junto, até conseguir fazer sozinho.

No conjunto, todas essas expressões representam uma maturidade operacional muito típica de empresas que possuem serviços grandes, complexos, distribuídos, em nuvem, onde falhas acontecem e precisam ser resolvidas com rigor. Não se trata simplesmente de “correção de bug”, mas de uma cultura de operação robusta, orientada a dados, rastreabilidade e aprendizado organizacional. É a essência do que times de SRE, Observabilidade e Sustentação fazem todos os dias — e casa profundamente com o seu perfil técnico de .NET, RabbitMQ, arquitetura limpa e práticas de engenharia de qualidade.

## Chaos Engineering
<img src="https://em-content.zobj.net/source/microsoft-teams/400/exploding-head_1f92f.png" align="right" height="77">

A **engenharia do caos** (Chaos Engineering) é uma disciplina rigorosa e proativa que visa revelar as fraquezas e vulnerabilidades ocultas em sistemas distribuídos complexos através da experimentação controlada. Engenharia do caos é uma disciplina onde falhas são intencionalmente introduzidas em um sistema para testar sua resiliência. O objetivo não é causar estragos, mas sim descobrir fraquezas em um ambiente controlado antes que elas se manifestem na produção.

Ela representa uma mudança de paradigma fundamental: em vez de esperar passivamente que as falhas ocorram naturalmente em produção — com todo o impacto negativo no negócio — as equipes planejam e executam deliberadamente experiências que simulam condições adversas para observar como o sistema responde. O objetivo final não é "quebrar o sistema por quebrar", mas sim construir confiança na capacidade do sistema de suportar condições turbulentas e imprevistas (Ordo ab chao).

Ao simular eventos inesperados como falhas de servidores, quedas de rede ou exaustão de recursos, a engenharia do caos ajuda as organizações a entenderem como seus sistemas se comportam sob estresse e como podem se recuperar de forma mais eficiente.

Os testadores desempenham um papel vital nos experimentos de caos, garantindo que sejam bem planejados, controlados, automatizados e conduzam a insights acionáveis. Abaixo estão os papéis-chave que os testadores desempenham na engenharia do caos, com exemplos de Amazon.com

Imagine que estamos no início dos anos 2000, e você é um desenvolvedor com uma ideia ousada. Você quer testar seu software não em um ambiente seguro e controlado, mas exatamente onde a ação está: no ambiente de produção. É aqui que usuários reais interagem com seu sistema. Naquela época, sugerir algo assim poderia te render olhares estranhos dos seus chefes. Mas agora, testar no mundo real não é apenas aceitável; É frequentemente recomendado.

Por que essa grande mudança? Alguns motivos se destacam. Os sistemas de hoje são mais complexos do que nunca, o que nos impulsiona a inovar mais rápido e garantir que nossos serviços sejam confiáveis e fortes. O avanço da tecnologia em nuvem, microserviços e sistemas distribuídos mudou o jogo. Tivemos que adaptar nossos métodos e mentalidades de acordo.

Nosso objetivo agora é criar sistemas que possam lidar com qualquer coisa — seja uma desaceleração ou uma queda total. Entra em cena a Engenharia do Caos.

Nesta edição, mergulhamos no que realmente é engenharia do caos. Vamos analisar seus princípios-chave, como é praticado e exemplos do mundo real. Você vai aprender como causar um pouco de caos controlado pode realmente ajudar a encontrar e corrigir fraquezas antes que se tornem grandes problemas.

Prepare-se para ver como abraçar o caos pode levar a sistemas mais fortes e confiáveis.

Então, o que exatamente é engenharia do caos? É uma forma de lidar com problemas inesperados no desenvolvimento de software e manter os sistemas funcionando. Algumas pessoas podem pensar que um servidor rodando um app vai continuar sem problemas para sempre. Outros acreditam que problemas fazem parte do acordo e que o tempo de inatividade é inevitável.

A engenharia do caos encontra um equilíbrio entre essas visões. Reconhece que as coisas podem dar errado, mas afirma que podemos tomar medidas para evitar que esses problemas impactem nossos sistemas e o desempenho dos nossos aplicativos.

Essa abordagem envolve experimentar em nossos sistemas de produção ao vivo para identificar pontos fracos e áreas que não são tão confiáveis quanto deveriam ser. Trata-se de medir o quanto confiamos na resiliência do nosso sistema e trabalhar para aumentar essa confiança

No entanto, é importante entender que ter 100% de certeza de que nada vai dar errado é irrealista. Por meio da engenharia do caos, introduzimos intencionalmente eventos inesperados para desvendar vulnerabilidades. Esses eventos podem variar bastante, como derrubar um servidor aleatoriamente, interromper um data center ou manipular balanceadores de carga e réplicas de aplicações.

Em resumo, engenharia do caos é sobre projetar experimentos que testem rigorosamente a robustez dos nossos sistemas.

Definindo Engenharia do Caos: Existem muitas formas de descrever a engenharia do caos, mas aqui está uma definição que captura bem sua essência, extraída de https://principlesofchaos.org/.

> "Engenharia do Caos é a disciplina de experimentar em um sistema para construir confiança na capacidade do sistema de resistir a condições turbulentas na produção."

Essa definição destaca o objetivo central da engenharia do caos: garantir que nossos sistemas possam lidar com a natureza imprevisível das operações do mundo real.

Engenharia de Performance vs. Engenharia do Caos: Quando falamos em garantir que nossos sistemas funcionem sem problemas, dois conceitos frequentemente surgem: engenharia de desempenho e engenharia do caos. Vamos discutir o que diferencia esses dois e como eles podem se sobrepor.

Muitos desenvolvedores já estão familiarizados com engenharia de performance, que pertence à mesma família do DevOps. Envolve o uso de uma combinação de ferramentas, processos e tecnologias para monitorar o desempenho do nosso sistema e promover melhorias contínuas. Isso inclui a realização de vários tipos de testes, como testes de carga, estresse e resistência, todos com o objetivo de aumentar o desempenho de nossas aplicações.

Por outro lado, engenharia do caos é sobre quebrar coisas intencionalmente. Sim, isso inclui testes de estresse, mas é mais sobre observar como os sistemas respondem sob estresse inesperado. Testes de estresse podem ser vistos como uma forma de experimento do caos. Então, uma forma de ver é considerar a engenharia de desempenho como um subconjunto da engenharia do caos ou o contrário, dependendo de como você aplica essas práticas.

Outra forma de enxergar esses dois é como disciplinas distintas dentro de uma organização. Uma equipe pode focar exclusivamente em realizar experimentos de caos e aprender com as falhas, enquanto outra pode se dedicar a tarefas de engenharia de desempenho, como testes e monitoramento. Dependendo da estrutura da organização, das habilidades do time e de vários outros fatores, podemos ter equipes separadas para cada disciplina ou uma equipe que enfrenta ambos.

Engenharia do Caos na Prática: Vamos considerar um exemplo para entender melhor a engenharia do caos. Imagine que temos um sistema com um balanceador de carga que direciona as requisições para servidores web. Esses servidores então se conectam a um serviço de pagamento, que, por sua vez, interage com uma API de terceiros e um serviço de cache, todos localizados na Zona de Disponibilidade A. Se o serviço de pagamento falhar em se comunicar com a API de terceiros ou com o cache, as solicitações precisam ser redirecionadas para a Zona de Disponibilidade B para manter alta disponibilidade.

![unnamed](https://github.com/user-attachments/assets/635a84db-cf48-4efa-aec5-3ff06a3b0628)

A filosofia central da engenharia do caos se baseia em um princípio irrefutável: em um mundo de microserviços, nuvem dinâmica e dependências complexas, as falhas são inevitáveis. Componentes de hardware vão parar, a latência da rede vai flutuar de forma imprevisível, discos vão encher, e pacotes de dados vão se corromper. A engenharia do caos aceita essa realidade caótica e, em vez de tentar criar um sistema "à prova de falhas" (uma impossibilidade prática), foca em criar um sistema "à prova de resiliência", que possa degradar-se graciosamente e se recuperar automaticamente quando as falhas inevitáveis ocorrerem.

A execução da engenharia do caos segue um método científico rigoroso, que pode ser resumido em uma sequência lógica de passos. Primeiro, a equipe formula uma hipótese claramente definida sobre como o sistema *deveria* se comportar sob uma determinada condição de estresse. Por exemplo: "Acreditamos que, se a zona de disponibilidade A da AWS ficar inacessível, o tráfego será redirecionado integralmente para a zona B sem que os usuários finais percebam qualquer interrupção". Em seguida, projeta-se um experimento para testar essa hipótese, escolhendo o escopo (em qual ambiente, com qual "raio de explosão" controlado) e a falha a ser injetada (o "ataque").

A execução do experimento ocorre de forma incremental e segura, preferencialmente começando em ambientes de staging e, conforme a confiança aumenta, avançando para pequenas partes do ambiente de produção, sempre com mecanismos de "abortar" rápidos e claros. Durante a execução, a observabilidade robusta é crucial — métricas, logs e traces são monitorados para coletar dados objetivos sobre o comportamento do sistema. Finalmente, os resultados são analisados: a hipótese foi confirmada? O sistema se comportou como esperado? Se não, quais fraquezas foram expostas? As descobertas alimentam um ciclo de melhoria contínua, levando a ajustes na arquitetura, no código, na configuração ou nos procedimentos operacionais.

Os tipos de experimentos são vastos e podem ser categorizados. Os **ataques de infraestrutura** simulam falhas em componentes físicos e virtuais, como desligar servidores, containers ou instâncias de nuvem. Os **ataques de rede** introduzem latência, perda de pacotes ou DNS spoofing para testar timeouts e retry policies. Os **ataques de recursos** consomem CPU, memória ou disco para verificar mecanismos de auto-scaling e priorização. Experimentos mais avançados, como **ataques de estado de aplicação**, podem corromper dados em memória ou forçar vazamentos, testando a robustez da própria lógica do software.

A relação simbiótica com a observabilidade não pode ser overstated. Realizar engenharia do caos sem uma observabilidade de alta qualidade é como pilotar um avião com os instrumentos quebrados — você está causando turbulência, mas não tem como saber se as asas estão prestes a cair. São os dados da observabilidade que permitem validar ou refutar a hipótese do experimento.

Em sua essência, a engenharia do caos é uma prática cultural tanto quanto é técnica. Ela exige e fomenta uma mentalidade de humildade e curiosidade, onde as equipes assumem que existem pontos fracos desconhecidos em seu sistema e se empenham ativamente em encontrá-los antes que causem um incidente real. É o ápice da maturidade em DevOps e SRE, transformando a operação de sistemas complexos de um exercício de reação a incidentes em uma prática contínua de fortalecimento antecipado e baseado em evidências.

<img height="77" align="right" src="https://github.com/user-attachments/assets/816d5e65-a359-4243-a5bf-bd952154381e" />

O **Gremlin** é uma plataforma de Chaos Engineering - uma disciplina que vai além do teste tradicional para questionar a resiliência fundamental do sistema sob condições anormais e inesperadas. Enquanto o Selenium tenta provar que o sistema funciona quando tudo está normal, o Gremlin tenta descobrir como o sistema falha quando as coisas dão errado. Ele injeta falhas controladas em ambientes de produção ou staging para testar a capacidade do sistema de lidar com cenários catastróficos: desligar instâncias de servidor sem aviso prévio, simular latência extrema na rede, consumir toda a CPU ou memória de um container, corromper pacotes de dados, ou até mesmo derrubar entire availability zones em clouds públicas.

Não confunda, esse Gremlin da engenharia de caos é diferente do Gremlin (linguagem de consulta) que é uma linguagem de travessia de grafos para banco de dados em grafos desenvolvida pela Apache TinkerPop.

O Gremlin é usado para uma categoria específica e avançada de testes conhecida como **Testes de Caos** ou **Experimentos de Caos**, que fazem parte da disciplina mais ampla do **Chaos Engineering**. Esta abordagem representa uma evolução fundamental em relação aos paradigmas de teste tradicionais, focando não na validação do comportamento correto do sistema sob condições ideais, mas sim na descoberta de suas fraquezas e pontos de falha sob condições anormais e estressantes.

![556629471-2ef59741-bc7a-4a90-9c60-398e5d4be77f](https://github.com/user-attachments/assets/2c1f7937-8a7d-4f4e-bfe3-345f8439c1b5)

Diferente de testes funcionais, de integração ou de carga, que verificam requisitos específicos predefinidos, os testes com Gremlin são **exploratórios e hipotéticos**. Eles partem de perguntas como: "O que acontece se o datacenter principal ficar inacessível?" ou "Como o sistema se comporta se o banco de dados ficar extremamente lento?". Em vez de esperar que essas falhas ocorram naturalmente em produção, com impacto real nos usuários, o Gremlin permite que as equipes simulem essas condições de forma controlada e segura para observar como o sistema responde.

Os principais tipos de experimentos conduzidos com o Gremlin se enquadram em categorias distintas de injeção de falhas:

- **Testes de Falha de Infraestrutura:** Estes são os experimentos mais fundamentais. Eles simulam falhas em componentes físicos e virtuais que sustentam a aplicação. Isso inclui desligar repentinamente instâncias de servidor (sejam VMs, containers ou pods no Kubernetes), simular a indisponibilidade de zonas inteiras em um provedor de cloud, ou desabilitar interfaces de rede. O objetivo é verificar se o sistema possui redundância adequada e se os mecanismos de failover funcionam conforme o esperado. Um teste típico seria terminar aleatoriamente 10% dos pods em um namespace do Kubernetes para validar se o sistema se auto-recupera.

- **Testes de Estresse de Recursos:** Estes experimentos não desligam componentes completamente, mas sim degradam seus desempenhos para criar condições de contorno. O Gremlin pode ser usado para consumir CPU, memória RAM, IO de disco ou largura de banda de rede até seus limites máximos. Isso revela como a aplicação se comporta sob escassez de recursos: ela falha graciosamente? Prioriza tarefas críticas? Gera logs de erro úteis? Ou entra em pane completa? Um exemplo é injetar uma carga de 90% de CPU em um container para ver se os mecanismos de auto-scaling são acionados corretamente.

- **Testes de Condições de Rede:** Em sistemas distribuídos, a rede é frequentemente o ponto mais frágil. O Gremlin permite simular uma vasta gama de condições de rede adversárias, como latência alta, perda de pacotes, limitação de banda (throttling) e até corrupção de pacotes. Estes testes são cruciais para validar timeouts, retries e circuit breakers configurados entre os serviços. Simular 500ms de latência em chamadas para um microsserviço de pagamento, por exemplo, pode expor problemas de experiência do usuário ou gargalos em cascata.

- **Testes de Falhas de Aplicação:** Indo um nível acima, o Gremlin pode induzir falhas em nível de aplicação, como encerrar processos específicos, forçar a exaustão de conexões de banco de dados ou corromper o estado na memória. Isso ajuda a testar a resiliência da própria lógica da aplicação e seus mecanismos de recuperação.

A execução destes testes segue uma metodologia rigorosa e científica, geralmente no modelo "Avanço Gradual com Controle de Estrago". Um experimento não começa afetando toda a base de usuários. Ele inicia em um ambiente de staging ou em uma pequena porção isolada da produção, com a equipe totalmente alerta e preparada para abortar o teste instantaneamente se o impacto for maior que o antecipado. Conforme a confiança na resiliência do sistema cresce, os experimentos podem se tornar mais amplos e complexos.

Em essência, o teste com Gremlin não é sobre "quebrar o sistema por quebrar", mas sim sobre aprender proativamente com as falhas em um ambiente controlado. É um investimento na confiabilidade do sistema, cujo resultado não é um simples "passou/falhou", mas um relatório detalhado de pontos fracos descobertos, gaps nos procedimentos de resposta a incidentes e oportunidades de melhoria arquitetural. Ele transforma a postura da equipe de reativa para proativa, permitindo que se fortaleçam as defesas do sistema antes que uma falha real e imprevista cause um prejuízo significativo ao negócio.

## LLM Observability
<img src="https://github.com/user-attachments/assets/a8962dc6-9680-4dc8-b79f-410a6d9b2c61" align="right" height="77">

Os grandes modelos de linguagem (LLMs) e plataformas de IA generativa (geração de IA), como IBM watsonx.ai® e uma variedade crescente de variantes de código aberto, estão se consolidando em todos os setores. Devido a esse aumento, tornou-se mais importante do que nunca manter a confiabilidade, segurança e eficiência dos modelos e aplicações após a adoção. Este espaço é onde a observabilidade do LLM se torna essencial.

A **observabilidade do LLM** é o processo de coleta de dados em tempo real de modelos ou aplicativos do LLM sobre suas características comportamentais, de desempenho e de saída. Como os LLMs são complexos, podemos observá-los com base em padrões no que eles produzem.

Uma boa solução de observabilidade consiste em coletar métricas, rastreamentos e logs relevantes de aplicativos LLM, interfaces de programação de aplicativos (APIs) e fluxos de trabalho, o que permite que os desenvolvedores monitorem, depurem e otimizem aplicativos de forma eficiente, proativa e em escala.

<img src="https://github.com/user-attachments/assets/3917b777-7fcb-4267-8d9b-2ea2f17335e5" align="right" height="77">

O New Relic AIM oferece visibilidade e insights sem precedentes para engenheiros e desenvolvedores que estão modernizando suas pilhas tecnológicas. Com o AIM, as equipes de engenharia podem monitorar, alertar, depurar e causar a raiz de aplicações alimentadas por IA.

## CAST Imaging
![unnamed](https://github.com/user-attachments/assets/4d40c673-af0f-4e56-8fe5-29f3848b5287)

**CAST Imaging** é uma plataforma de Software Intelligence criada pela CAST para fornecer visibilidade profunda e automatizada sobre sistemas de software complexos. Ela foi projetada para ajudar organizações a entender, mapear e analisar aplicações grandes — muitas vezes legadas — sem depender exclusivamente de documentação manual ou do conhecimento tácito de desenvolvedores que já não estão mais na empresa. Em vez de apenas analisar código superficialmente, a ferramenta realiza uma inspeção estrutural do sistema, construindo um modelo interno que representa componentes, dependências, fluxos de dados e interações entre camadas.

Na prática, o CAST Imaging funciona como um “scanner arquitetural” de aplicações. Ele analisa o código-fonte de múltiplas linguagens, identifica como módulos se conectam, detecta chamadas entre serviços, integrações com bancos de dados e até dependências externas. A partir dessa análise estática, a plataforma gera uma representação visual interativa da arquitetura do sistema, permitindo que desenvolvedores e arquitetos naveguem pela aplicação como se estivessem explorando um mapa. Isso facilita a compreensão de sistemas monolíticos extensos, arquiteturas distribuídas ou ambientes híbridos que evoluíram ao longo de anos.

Um dos principais objetivos do CAST Imaging é reduzir risco em iniciativas de modernização, migração para cloud ou refatoração. Em projetos desse tipo, um grande desafio é entender o impacto de alterações em determinadas partes do sistema. A ferramenta permite realizar análises de impacto, mostrando quais componentes serão afetados caso um módulo específico seja modificado. Isso ajuda na tomada de decisão técnica e reduz surpresas em produção. Além disso, ela auxilia na identificação de dívidas técnicas, gargalos arquiteturais e violações de boas práticas estruturais.

Outro ponto relevante é que a plataforma não se limita a métricas superficiais de qualidade de código, como contagem de linhas ou complexidade ciclomática isolada. Ela trabalha com o conceito de inteligência estrutural, avaliando a robustez da arquitetura como um todo. Isso inclui detecção de ciclos de dependência, excesso de acoplamento, violações de camadas arquiteturais e padrões de risco que podem comprometer a escalabilidade ou a manutenibilidade do sistema. Dessa forma, o foco não está apenas em bugs, mas na saúde estrutural da aplicação.

Em termos organizacionais, o CAST Imaging é frequentemente utilizado por grandes empresas que possuem portfólios extensos de aplicações corporativas, especialmente em setores como finanças, telecomunicações, seguros e governo. Nesses ambientes, onde sistemas críticos acumulam décadas de evolução e integrações complexas, a visibilidade arquitetural se torna essencial para governança de TI e planejamento estratégico.

Em essência, o CAST Imaging é uma ferramenta de análise e visualização arquitetural que transforma código-fonte em um modelo navegável e inteligível do sistema, permitindo que equipes compreendam, avaliem riscos e planejem evoluções com base em dados estruturais concretos, em vez de suposições ou documentação desatualizada.

CAST Imaging está muito mais próximo de **observabilidade estrutural de software** do que de Deep Learning.

Ele não é um sistema de aprendizado de máquina que treina modelos neurais para reconhecer padrões como imagens, texto ou voz. Ele trabalha principalmente com **análise estática de código**, engenharia reversa e modelagem estrutural de sistemas. Ou seja, ele “lê” o código-fonte, interpreta dependências, constrói grafos de relacionamento entre componentes e gera uma representação navegável da arquitetura.

Deep Learning, por outro lado, envolve redes neurais profundas, treinamento com grandes volumes de dados e inferência probabilística. O CAST Imaging não está tentando “aprender” padrões a partir de dados históricos para prever algo. Ele está executando análises determinísticas baseadas em regras formais de parsing, semântica de linguagem e modelagem arquitetural.

Se quisermos posicionar conceitualmente:

Deep Learning → foco em aprendizado estatístico a partir de dados.
CAST Imaging → foco em compreensão estrutural determinística de código.

Ele se aproxima mais de ferramentas como APM avançado, análise arquitetural, mapeamento de dependências e governança de software do que de IA generativa ou modelos neurais.

A palavra “inteligência” no contexto da CAST significa mais “Software Intelligence” — isto é, gerar insights estruturais sobre sistemas — e não “inteligência artificial baseada em redes neurais”.

Então sim, é muito mais observabilidade e engenharia estrutural do que Deep Learning.

Que se você pudesse identificar instantaneamente as únicas 3 funcionalidades para testar a não-regressão após modificar uma classe Java complexa?

E se você pudesse visualizar o efeito cascata, do banco de dados para o front-end, de mudar o tipo de dado de uma coluna?

Domine sua aplicação com a arma suprema dos arquitetos

A imagem CAST mapeia automaticamente o funcionamento interno de qualquer aplicação:

Visualize todas as dependências e explore o acesso ao banco de dados

Rastrear dados de ponta a ponta e fluxos de chamadas, avaliar o impacto das mudanças

Identificar falhas estruturais tipicamente ignoradas pelas ferramentas de qualidade de código

Pare de perder horas incontáveis fazendo engenharia reversa do seu código manualmente.
Avance mais rápido com o CAST Imaging, a tecnologia automatizada de mapeamento por software.

O CAST Imaging suporta qualquer combinação de Java/JEE, .NET, Python, COBOL, SQL e 100+ outras linguagens, frameworks e motores de banco de dados.

## SEO, SRE e Mecanismos de busca
Desbloqueie uma busca altamente relevante com IA e insights sobre o uso da busca semântica pela Cococart para impulsionar novas experiências na loja.

Como equipes ágeis podem aproveitar LLMs, bancos de dados vetoriais e amigos para lançar rapidamente experiências de busca semântica de ponta para fama e lucro

![unnamed](https://github.com/user-attachments/assets/91b86ba7-9b10-43da-81a2-09db895f9c9b)

É impressionante como tantas coisas são melhoradas com uma busca excelente. O Google facilitou para pessoas comuns encontrarem tudo o que precisavam online, por mais obscuro que fosse. O fuzzy matching e a busca de símbolos do IntelliJ IDEA ajudaram os programadores a esquecer a estrutura de diretórios de suas bases de código. O AirTag adicionou capacidades avançadas de localização espacial para meu gato. Um recurso de descoberta bem elaborado pode adicionar aquele fator "uau" que produtos icônicos e viciantes têm.

Neste post, abordarei como uma equipe dinâmica pode aproveitar Grandes Modelos de Linguagem (LLMs), Bancos de Dados Vetoriais, Aprendizado de Máquina e outras tecnologias para criar uma experiência de busca e descoberta inspiradora com restrições de orçamento e tempo para startups

Busca Semântica é um método de busca para obter resultados altamente relevantes com base no significado da consulta, contexto e conteúdo. Vai além da simples indexação ou filtragem de palavras-chave. Ele permite que os usuários encontrem as coisas de forma mais natural e com melhor suporte à nuance do que métodos tradicionais de relevância altamente sofisticados, porém rígidos. Na prática, parece a diferença entre perguntar para uma pessoa real ou conversar com uma máquina.

Empresas de tecnologia ao redor do mundo estão correndo para incorporar essas capacidades em seus produtos existentes. A Instacart publicou um artigo extenso sobre como adicionaram a deduplicação semântica à sua experiência de busca. Outras empresas que implementam algum tipo de busca semântica incluem eBay, Shopee, Ikea, Walmart e muitas outras.

<img width="1306" height="797" alt="unnamed" src="https://github.com/user-attachments/assets/ddedbf6d-61eb-47ad-9fac-60b09d6929a1" />

A motivação para adotar a busca semântica é simples: resultados mais relevantes levam a clientes mais satisfeitos e a mais receita. Descoberta, relevância e confiabilidade são alguns dos problemas mais difíceis de resolver no comércio eletrônico. Existe um ecossistema inteiro de soluções para ajudar as empresas a enfrentar esses desafios.

Muitas soluções hoje dependem de embeddings de documentos – representando significado como vetores. Como a busca semântica sozinha pode não fornecer resultados relevantes suficientes, a busca tradicional em texto completo é frequentemente usada para complementar os resuts. Um ciclo de feedback baseado nas interações do usuário (cliques, curtidas, etc.) fornece informações para melhorar continuamente a relevância.

Os principais processos são: indexação, consulta e acompanhamento

![unnamed](https://github.com/user-attachments/assets/240804c3-8ec9-4c10-a59d-178561ce0f1d)

A indexação é feita convertendo o conteúdo de um documento em um vetor de embeddings por meio de um codificador text-para-vetor (por exemplo, a API Embeddings da OpenAI). Os vetores são inseridos em um banco de dados vetorial (por exemplo, Qdrant, Milvus, Pinecone). Modelos de codificação texto-para-vetor, como transformadores de frase, convertem trechos de texto em representações numéricas vetoriais que capturam significado semântico e semelhanças entre textos. Os documentos também são indexados em um mecanismo de busca tradicional em texto completo (por exemplo, Elasticsearch)

![unnamed](https://github.com/user-attachments/assets/a1f64d1d-c691-4f16-b2af-219c0245d2fa)
 
<img width="1600" height="834" alt="unnamed" src="https://github.com/user-attachments/assets/892eee76-5c04-49f2-a610-05598f7604ee" />

Essa imagem representa **métricas de confiabilidade e operação de sistemas**, muito usadas em **SRE (Site Reliability Engineering)**, **DevOps** e **engenharia de confiabilidade** para medir **falhas, detecção de problemas e tempo de recuperação de sistemas**. Ela mostra o ciclo de funcionamento de um sistema: ele opera normalmente (✔️), ocorre uma falha (❌), o problema é **diagnosticado**, depois **reparado**, o sistema volta a funcionar e eventualmente pode falhar novamente. A linha do tempo abaixo ilustra métricas usadas para medir cada parte desse processo.

A primeira métrica mostrada é o **MTTD (Mean Time To Detect)**. Esse valor mede **quanto tempo leva para detectar que ocorreu uma falha no sistema**. Em ambientes modernos isso depende muito de observabilidade, monitoramento, alertas e logs. Ferramentas como **Prometheus**, **Grafana** e **Elastic Stack** ajudam a reduzir esse tempo porque detectam automaticamente anomalias ou falhas.

Depois aparece o **MTTR (Mean Time To Repair ou Mean Time To Recovery)**. Essa métrica mede **quanto tempo leva para corrigir o problema depois que ele foi identificado**. Esse tempo inclui diagnóstico, correção e restauração do serviço. Em engenharia de confiabilidade, reduzir o MTTR é extremamente importante porque significa restaurar o sistema mais rápido quando ocorre uma falha.

Em seguida aparece o **MTTF (Mean Time To Failure)**. Esse valor representa **quanto tempo um sistema ou componente funciona antes de ocorrer uma falha**. Ele é muito usado quando se fala de confiabilidade de hardware ou software que não é reparado imediatamente, mas também pode ser usado para avaliar a estabilidade de serviços.

Por fim, a imagem mostra o **MTBF (Mean Time Between Failures)**, que é uma métrica clássica de confiabilidade. Ela representa **o tempo médio entre uma falha e a próxima falha do sistema**. Em sistemas reparáveis, o MTBF normalmente inclui o tempo de funcionamento mais o tempo de reparo. Quanto maior o MTBF, mais confiável é o sistema.

Em termos simples, o diagrama mostra **o ciclo de vida de uma falha em sistemas distribuídos** e como cada parte pode ser medida: primeiro o problema acontece, depois alguém precisa detectá-lo (MTTD), então ele é corrigido (MTTR), e o tempo que o sistema permanece funcionando antes de falhar novamente é representado por métricas como MTTF e MTBF.

Essas métricas são extremamente importantes em ambientes de **cloud, microservices e infraestrutura distribuída**, porque ajudam equipes a melhorar **disponibilidade, resiliência e confiabilidade operacional** dos sistemas. Elas também são muito usadas para medir **SLA e SLO** em plataformas modernas.

Se quiser, também posso te explicar **a relação entre MTTR, MTBF e disponibilidade do sistema (uptime)** — existe até uma fórmula simples que arquitetos de sistemas usam para calcular **percentual de disponibilidade**.

# 🟥 Zabbix
<img src="https://img.shields.io/badge/Grafana_Stack-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white">

<a href=""><img src="https://www.vectorlogo.zone/logos/zabbix/zabbix-ar21.svg" align="right" height="77"></a>

**Zabbix** é uma plataforma de monitoramento de código aberto usada para acompanhar o desempenho e a disponibilidade de servidores, redes, aplicações, serviços em nuvem e outros componentes de infraestrutura de TI. Ele permite coletar, armazenar, analisar e visualizar métricas em tempo real, alertando administradores quando algo foge do comportamento esperado, como aumento de uso de CPU, queda de serviços, problemas de disco, falhas de conectividade ou qualquer outro evento que comprometa a operação de sistemas. 

Por ser altamente configurável e escalável, o Zabbix é amplamente utilizado por empresas de diversos tamanhos, desde pequenos negócios até grandes corporações e instituições públicas.

A arquitetura do Zabbix é baseada em agentes instalados nos dispositivos a serem monitorados, que coletam os dados e enviam para o servidor Zabbix central. No entanto, ele também suporta coleta de dados sem agente, usando protocolos como SNMP, IPMI, SSH, Telnet, HTTP, entre outros, o que o torna extremamente flexível. Esses dados são armazenados em um banco de dados relacional (geralmente MySQL, PostgreSQL ou Oracle), permitindo análises históricas e geração de gráficos detalhados. O sistema de alertas é poderoso e pode ser integrado com e-mails, SMS, mensagens em aplicativos como Telegram, Slack ou via Webhook com qualquer sistema externo, permitindo ações automatizadas em resposta a incidentes.

A interface web do Zabbix oferece dashboards personalizáveis, gráficos, mapas de rede, relatórios e outras ferramentas de visualização, ajudando as equipes de operações a entenderem rapidamente o que está acontecendo em seus sistemas. Um dos seus pontos fortes é a detecção proativa de problemas baseada em gatilhos definidos pelo usuário, com suporte a expressões condicionais e templates prontos para facilitar a configuração de novos hosts. Ele também permite a descoberta automática de novos dispositivos ou serviços, o que reduz o esforço manual e mantém o ambiente sempre atualizado. Tudo isso contribui para a observabilidade e resiliência da infraestrutura, tornando o Zabbix uma peça fundamental na estratégia de monitoramento de ambientes modernos.

Além disso, o Zabbix é gratuito sob licença GPL, o que atrai a comunidade de software livre e permite personalizações sem custo de licença. No entanto, também existem serviços comerciais e suporte oferecidos pela empresa Zabbix SIA para empresas que desejam assistência profissional ou hospedagem gerenciada. O Zabbix é uma solução madura, ativa desde os anos 2000, com uma base sólida de usuários e ampla documentação. Em um mundo onde manter a disponibilidade e o desempenho dos sistemas é essencial para os negócios, o Zabbix se consolida como uma ferramenta completa e confiável para garantir que tudo esteja funcionando como deveria.

# 🟩 New Relic
<a href=""><img src="" align="right" height="77"></a>

**New Relic** é uma plataforma de observabilidade e monitoramento de desempenho de aplicações (APM — Application Performance Monitoring) que permite a desenvolvedores, engenheiros de software, operadores de infraestrutura e equipes de negócios acompanharem em tempo real o comportamento de seus sistemas digitais. 

Assim como o Datadog, ela centraliza uma ampla variedade de dados como métricas, logs, rastreamentos distribuídos (traces), eventos e informações do navegador do usuário para que os times possam diagnosticar problemas, melhorar a performance e tomar decisões baseadas em dados concretos. A filosofia do New Relic é oferecer uma visão unificada da saúde e do desempenho de toda a stack tecnológica, desde o frontend até os bancos de dados e serviços externos.

A plataforma funciona a partir da instalação de agentes em linguagens como Java, .NET, Node.js, Python, Ruby, PHP e Go, além de integrar com serviços de nuvem como AWS, Azure e Google Cloud. Esses agentes coletam dados automaticamente sobre tempo de resposta, throughput, uso de recursos, erros, gargalos e chamadas externas, e enviam tudo para o console da New Relic, que exibe os resultados por meio de dashboards interativos. Um de seus pontos fortes é a capacidade de traçar a jornada de uma requisição em múltiplos serviços, o que facilita a detecção de falhas em arquiteturas baseadas em microserviços ou contêineres, como os orquestrados por Kubernetes.

Além do monitoramento de backend, o New Relic também oferece funcionalidades para rastrear a experiência do usuário final, como o RUM (Real User Monitoring), que mostra como os visitantes de um site interagem com páginas e qual o impacto do desempenho do frontend sobre sua experiência. Há ainda recursos de testes sintéticos, que simulam acessos programados para detectar quedas ou lentidão antes que usuários reais sejam impactados. Com a evolução da plataforma, o New Relic expandiu suas capacidades para incluir logs centralizados, monitoramento de infraestrutura, alertas baseados em regras e inteligência artificial para detectar anomalias automaticamente.

A interface da ferramenta, chamada New Relic One, é baseada em uma abordagem "tudo-em-um", permitindo a correlação direta entre logs, métricas e traces em um só lugar, o que facilita a análise de causa raiz. A ferramenta também é extensível via APIs e suporta dashboards customizados com sua linguagem de consulta própria, a NRQL (New Relic Query Language), usada para criar visualizações específicas a partir dos dados coletados. Empresas de todos os tamanhos utilizam a New Relic tanto para manter seus sistemas disponíveis e eficientes quanto para otimizar suas aplicações com base em dados de uso reais. Embora seja uma solução comercial, a New Relic possui planos gratuitos com limites mensais, o que facilita sua adoção inicial.

Com o avanço da inteligência artificial e a crescente complexidade das aplicações modernas, ferramentas como o New Relic tornaram-se essenciais para dar visibilidade e controle sobre ambientes distribuídos e dinâmicos. Mais do que apenas um sistema de alerta, ele se posiciona como um verdadeiro copiloto técnico para times de engenharia, capaz de reduzir o tempo de resposta a incidentes e orientar melhorias contínuas com base em dados objetivos.

O New Relic Grok facilita para você obter os insights necessários sem precisar entender toneladas de dados de telemetria. Corte o barulho para obter as respostas certas rápida e fácil. O New Relic Grok aproveita os grandes modelos de linguagem (LLMs) da OpenAI para que qualquer engenheiro possa usar linguagem simples e uma interface de chat familiar para fazer perguntas e obter insights, sem qualquer experiência prévia em observabilidade. A observabilidade agora é tão simples quanto perguntar ao New Relic Grok: "Por que meu carrinho não está funcionando?" ou "Instrumente AWS."

O Teste de Segurança de Aplicações Interativas da Relic (IAST) já está em prévia pública! Engenheiros, equipes de DevOps e segurança agora podem encontrar, corrigir e verificar vulnerabilidades de alto risco cedo e com precisão para construir aplicações mais seguras — e enviar código mais rapidamente.

![unnamed](https://github.com/user-attachments/assets/dc433db8-19e0-4f3e-aa1a-b0e55fe28977)

# 🟢 UptimeRobot
<a href=""><img src="" align="right" height="77"></a>

**UptimeRobot** é um serviço online que tem como principal função monitorar a disponibilidade (uptime) e o tempo de resposta de websites, servidores e serviços web em geral. Ele realiza verificações periódicas — geralmente a cada cinco minutos, no plano gratuito, e em intervalos menores em planos pagos — para assegurar que o serviço monitorado esteja acessível e funcionando corretamente. Quando detecta uma falha, como um site fora do ar (downtime) ou um tempo de resposta excessivo, o UptimeRobot imediatamente envia alertas por e-mail, SMS, chamadas de voz, ou integrações como Slack, Telegram, Discord, Webhooks e outras plataformas, permitindo que os responsáveis tomem providências rápidas para corrigir o problema.

A forma como ele realiza as checagens varia conforme o tipo de monitoramento configurado. Ele pode simplesmente fazer uma requisição HTTP ou HTTPS e verificar se o status code retornado indica sucesso, ou ainda usar métodos como monitoramento por ping, portas específicas (como SMTP, FTP, MySQL), além de verificar palavras-chave específicas dentro do conteúdo retornado por uma página para garantir que ela não só esteja online, mas também exiba a informação esperada. Isso é útil, por exemplo, quando o servidor responde com código 200, mas exibe uma página de erro no conteúdo HTML.

Além da sua simplicidade e facilidade de uso, o UptimeRobot também oferece dashboards e históricos de disponibilidade, permitindo que equipes acompanhem métricas como percentual de uptime mensal ou anual, tempo médio de resposta e momentos em que ocorreram falhas. Esses dados podem ser exibidos em painéis públicos, que são úteis para mostrar transparência ao cliente, ou privados, apenas para os administradores. Como ele possui servidores espalhados pelo mundo, consegue monitorar a disponibilidade de um site a partir de diferentes regiões geográficas, o que ajuda a identificar problemas de acessibilidade regional ou bloqueios por CDN e firewalls.

Empresas de todos os tamanhos usam o UptimeRobot como uma primeira camada de detecção de problemas, especialmente em sistemas que exigem alta disponibilidade, como e-commerces, APIs públicas, serviços financeiros e plataformas SaaS. Embora não ofereça a mesma profundidade de uma ferramenta de observabilidade como o New Relic ou o Datadog, o UptimeRobot é uma excelente escolha para monitoramento simples, direto e com baixo custo, sendo frequentemente usado em conjunto com outras ferramentas. Ele se tornou popular entre desenvolvedores independentes, startups e equipes de DevOps que precisam de alertas confiáveis sem a complexidade de configurar soluções mais robustas. Seu modelo freemium com plano gratuito atrai muitos usuários que desejam garantir que seus sistemas estejam sempre no ar, o que faz dele uma peça útil em qualquer stack de monitoramento.

# 🔷 Nagios
<img src="https://github.com/user-attachments/assets/2e079a13-e9ca-4fda-824d-ca75d18c7a90" align="right" height="77">

O **Nagios** é uma ferramenta de monitoramento de infraestrutura de TI que se tornou uma verdadeira lenda e um pilar fundamental no mundo das operações de sistemas. Desenvolvido originalmente por Ethan Galstad e lançado como projeto open-source em 1999, o Nagios surgiu em uma época onde monitorar servidores, serviços e redes era uma tarefa complexa e fragmentada. Sua arquitetura pioneira estabeleceu padrões que influenciaram praticamente todas as soluções de monitoramento que vieram depois, criando um paradigma que dominou a área por mais de uma década.

A filosofia central do Nagios é relativamente simples, porém extremamente poderosa: ele funciona como um sistema de verificação centralizado que executa "checks" periódicos em recursos de TI distribuídos. Esses recursos podem ser praticamente qualquer coisa - um servidor físico, um serviço como HTTP ou SSH, espaço em disco, utilização de CPU, um switch de rede, um roteador, ou até mesmo um sensor de temperatura em um datacenter. O Nagios agenda e executa esses checks através de agentes ou protocolos padrão como SNMP, e então classifica o estado do recurso como OK, WARNING, CRITICAL ou UNKNOWN, com base em limiares pré-configurados. Quando um check retorna um estado de WARNING ou CRITICAL, o Nagios aciona notificações através de email, SMS ou outros métodos, alertando os administradores sobre a falha.

O que tornou o Nagios verdadeiramente revolucionário foi sua arquitetura modular e extensível. O núcleo do Nagios é enxuto e focado no agendamento de checks, no processamento de resultados e na lógica de notificação. A execução real dos checks de monitoramento é delegada a plugins - programas externos independentes que podem ser escritos em qualquer linguagem (Bash, Perl, Python, C, etc.). Essa separação de responsabilidades permitiu que uma comunidade massiva de desenvolvedores criasse milhares de plugins para os mais variados cenários, desde verificar a saúde de um banco de dados Oracle até monitorar a temperatura de uma sala de servidores através de um sensor IP. Essa ecossistema de plugins transformou o Nagios de uma simples ferramenta em uma plataforma completa de monitoramento.

Outro conceito fundamental introduzido pelo Nagios foi a dependência de hosts e serviços. Em infraestruturas complexas, é comum que a falha de um roteador cause a indisponibilidade de dezenas de servidores. Sem o conceito de dependência, o Nagios geraria uma enxurrada de notificações para cada servidor afetado, ofuscando a causa raiz real - o roteador com problemas. Ao definir dependências hierárquicas, o Nagios se torna inteligente o suficiente para suprimir notificações de problemas derivados, focando a atenção dos administradores no componente crítico que realmente precisa de intervenção.

A evolução do Nagios levou a duas ramificações principais: o Nagios Core, que mantém a versão open-source original e gratuita, e o Nagios XI, uma versão comercial que adiciona uma interface web mais polida, recursos de relatórios avançados, configuração assistida e capacidades de auto-descoberta. Enquanto o XI visa simplificar a vida de empresas com menos expertise em Linux, o Core permanece como a escolha preferida de puristas e grandes organizações com equipes especializadas.

No entanto, nas últimas décadas, o Nagios começou a mostrar sua idade quando confrontado com a realidade dos ambientes de nuvem dinâmicos e arquiteturas de microserviços. Sua natureza baseada em configuração estática em arquivos texto torna-o menos ágil para ambientes onde servidores são criados e destruídos automaticamente através de orquestradores como Kubernetes. A escalabilidade horizontal também se torna um desafio, já que uma instância centralizada do Nagios pode ter dificuldade em monitorar dezenas de milhares de endpoints em tempo real.

Apesar desses desafios, o legado do Nagios é inegável. Ele foi a ferramenta que ensinou uma geração inteira de administradores de sistemas a pensar de forma estruturada sobre monitoramento. Conceitos como checks ativos versus passivos, escalações de alerta, janelas de manutenção e templates de configuração foram todos popularizados pelo Nagios. Mesmo ferramentas modernas como Prometheus, Zabbix e Datadog carregam em seu DNA influências diretas da filosofia do Nagios. Para muitas organizações, especialmente aquelas com infraestruturas mais tradicionais e estáticas, o Nagios continua sendo uma solução robusta, confiável e extremamente custo-efetiva que faz exatamente o que promete: avisar quando algo importante para o negócio para de funcionar.

# ❇️ Splunk
<img src="https://github.com/user-attachments/assets/68af3881-34fa-4c58-9b3e-e6cca4094515" align="right" height="77">

O **Splunk** é uma plataforma de análise e monitoramento de dados que nasceu com a proposta de coletar, indexar e correlacionar grandes volumes de dados gerados por máquinas, como logs de servidores, aplicações, dispositivos de rede e sistemas diversos. Ele funciona como uma espécie de “motor de busca para dados de máquina”, permitindo que uma empresa consiga extrair informações úteis de registros que, de outra forma, ficariam apenas acumulados em arquivos dispersos e difíceis de interpretar. A grande força do Splunk está em transformar esses dados não estruturados em algo pesquisável, indexado e passível de visualização em tempo real.

Em termos de observabilidade, o Splunk é bastante relevante porque consegue unificar métricas, logs e traces em um mesmo ecossistema, o que permite investigar desde falhas em aplicações até incidentes de segurança, além de acompanhar a saúde de sistemas complexos em infraestruturas de grande escala. Ele oferece dashboards dinâmicos, alertas personalizados e uma linguagem de consulta própria (SPL – Search Processing Language) que facilita a exploração dos dados, seja para encontrar padrões, correlacionar eventos, ou até aplicar detecção de anomalias. Isso é fundamental em ambientes distribuídos, microservices e nuvens híbridas, onde o volume e a diversidade de dados crescem em alta velocidade.

Outro ponto importante é que o Splunk extrapola o monitoramento clássico e se posiciona como uma solução de SIEM (Security Information and Event Management) e de análise de dados para negócios. Empresas o utilizam não só para acompanhar performance de sistemas, mas também para detectar ataques cibernéticos, fraudes e até para extrair insights operacionais e de negócios a partir dos eventos. Ele pode ser integrado com diversas fontes, desde bancos de dados, APIs e filas de mensagens, até soluções de observabilidade como Prometheus e OpenTelemetry, funcionando como um ponto central de correlação e visualização.

Resumindo, o Splunk é ao mesmo tempo uma ferramenta de monitoramento, observabilidade, segurança e análise de dados de máquina. Ele ajuda a responder rapidamente a perguntas críticas como “o que está acontecendo agora no meu sistema?”, “onde está o gargalo de performance?” ou “há sinais de ataque em andamento?”. É um exemplo claro de como dados brutos podem se transformar em inteligência operacional e estratégica.

# 🎤 Voice search
O **voice search**, ou busca por voz, representa uma evolução fundamental na forma como os seres humanos interagem com a tecnologia, migrando da interface gráfica e do texto digitado para a modalidade mais natural e primária da comunicação humana: a fala. Trata-se da capacidade de usar comandos de voz para realizar pesquisas na internet, acionar assistentes virtuais, controlar dispositivos smart ou operar aplicativos, sem a necessidade de usar as mãos para digitar ou tocar em telas. Essa tecnologia é a espinha dorsal de assistentes como Google Assistant, Amazon Alexa, Apple Siri e Microsoft Cortana, e está integrada em smartphones, smart speakers, smart TVs, carros e uma gama crescente de dispositivos da Internet das Coisas.

A diferença crucial entre uma busca por voz e uma busca textual tradicional vai muito além do simples método de entrada. Elas refletem contextos, intenções e comportamentos radicalmente diferentes. Uma busca textual é tipicamente concisa, com palavras-chave fragmentadas ("previsão tempo São Paulo"). Já uma busca por voz, por ser conversacional, tende a ser muito mais longa, completa e formulada como uma pergunta natural em linguagem coloquial ("Ok Google, qual é a previsão do tempo para São Paulo neste final de semana?"). Essa mudança de paradigma forçou os mecanismos de busca a evoluírem de sistemas que simplesmente correspondem palavras-chave para sistemas que precisam compreender a linguagem natural, o contexto, a intenção do usuário e, até mesmo, nuances como sarcasmo ou regionalismos.

Do ponto de vista técnico, o voice search é um feito notável de engenharia que envolve uma cadeia complexa de processos. Primeiro, o reconhecimento de fala automático (ASR) converte o sinal de áudio da fala em texto puro. Em seguida, o Processamento de Linguagem Natural (NLP) entra em ação para analisar a estrutura linguística desse texto, identificando a intenção principal da consulta e extraindo entidades importantes (como locais, datas, nomes próprios). Finalmente, essa intenção compreendida é usada para buscar a resposta mais precisa em um banco de dados ou na web, e um sistema de síntese de voz (TTS) frequentemente devolve a resposta em áudio, completando o ciclo de uma conversa bidirecional.

O impacto dessa tecnologia no marketing digital e no SEO (Search Engine Optimization) é profundo e exige uma reestratégia completa. O conceito de "SEO para voz" surgiu como uma disciplina específica, focada em capturar essas consultas longas e conversacionais. Isso envolve a criação de conteúdo que responda diretamente a perguntas, frequentemente utilizando um tom mais direto e estruturado com marcadores de schema como FAQ (Perguntas Frequentes) que os mecanismos de busca podem facilmente extrair para fornecer respostas diretas, conhecidas como "featured snippets" ou "posição zero". Como as respostas de busca por voz geralmente leem em voz alta apenas o primeiro resultado (a resposta considerada ideal), ser essa fonte primária tornou-se o Santo Graal para muitos negócios.

O contexto de uso do voice search também é único. Ele é predominantemente móvel e local. As pessoas usam a busca por voz enquanto estão cozinhando ("quantas colheres de sopa em uma xícara?"), dirigindo ("qual o caminho mais rápido para casa?"), ou em situações onde suas mãos e olhos estão ocupados. Isso cria uma oportunidade enorme para negócios locais, pois consultas como "perto de mim" são extremamente comuns. Um restaurante otimizado para voice search tem muito mais chances de ser sugerido quando alguém perguntar "Alexa, qual é um bom restaurante italiano perto da minha localização?".

Olhando para o futuro, o voice search é muito mais do que um recurso de conveniência; é a porta de entrada para uma computação verdadeiramente ambient, onde a interface desaparece e a interação com a tecnologia se torna uma extensão natural do nosso comportamento. À medida que a precisão do reconhecimento de voz melhorar e a IA se tornar mais contextual, espera-se que a busca por voz se torne o principal método de interação para uma vasta gama de tarefas, desde controlar nossas casas inteligentes até realizar compras complexas e acessar informações de saúde. Compreender e adaptar-se a essa mudança não é mais uma opção para empresas e criadores de conteúdo; é uma necessidade estratégica para permanecerem relevantes em um mundo onde falar com as máquinas será tão comum quanto falar com outras pessoas.

# 🔶 Sentry.io
<img src="https://github.com/user-attachments/assets/f69ff0be-406f-4f56-945e-9c6d91376fd3" align="right" height="77">

O **Sentry.io** é uma plataforma de monitoramento de erro e desempenho de aplicações focada especificamente na experiência do desenvolvedor. Diferente de ferramentas de observabilidade mais abrangentes que monitoram infraestrutura e desempenho de sistemas de forma ampla, o Sentry tem um propósito muito específico: capturar, agregar e analisar cada erro que ocorre no código da sua aplicação, seja no frontend, backend ou mobile. 

A premissa fundamental é simples, mas profundamente poderosa: em vez de depender de usuários reportando bugs ou de engenheiros vasculhando logs em múltiplos servidores, o Sentry instrumenta seu código para capturar automaticamente toda e qualquer exceção que ocorrer em tempo de execução, enriquecendo essas informações com um contexto detalhado que permite reproduzir e diagnosticar o problema rapidamente.

O fluxo de trabalho típico começa com a integração do SDK do Sentry no código da aplicação. Esses SDKs estão disponíveis para praticamente todas as linguagens e frameworks modernos - JavaScript, Python, Java, Go, Ruby, PHP, C# e dezenas de outras. Quando um erro ocorre em produção, mesmo que ele tenha sido capturado por um bloco try-catch genérico, o Sentry o captura automaticamente e envia um "evento" para sua plataforma. Esse evento vai muito além da simples mensagem de erro. Ele inclui um stack trace completo, mostrando exatamente qual linha de código em qual arquivo causou o problema, o estado das variáveis no momento do erro, informações sobre o usuário afetado (como ID, email, geolocalização), o contexto da requisição HTTP (headers, query parameters, body), o estado do browser ou dispositivo móvel, e até mesmo os breadcrumbs - que são um registro passo a passo das ações que levaram ao erro, como chamadas de API, interações de UI e navegação entre páginas.

Uma das capacidades mais valiosas do Sentry é a agregação inteligente de erros. Em sistemas distribuídos com milhares de usuários, o mesmo erro pode ocorrer milhares de vezes. Em vez de inundar a equipe com notificações redundantes, o Sentry agrupa erros idênticos em "issues", permitindo que os desenvolvedores vejam o impacto real de cada bug - quantos usuários foram afetados, com que frequência o erro ocorre e qual é a tendência ao longo do tempo. Isso é crucial para priorização: um erro que afeta 0,1% dos usuários uma vez por dia é muito diferente de um erro que afeta 5% dos usuários a cada hora.

Além do monitoramento de erros, o Sentry evoluiu para incluir monitoramento de desempenho (Performance Monitoring), que rastreia a latência de transações e operações críticas na aplicação. Ele permite identificar não apenas o que está quebrado, mas também o que está lento. Através do rastreamento distribuído, é possível visualizar toda a cadeia de uma requisição - desde o clique no frontend, passando por vários microserviços no backend, até consultas em bancos de dados e chamadas para serviços externos. Isso revela gargalos de performance que seriam impossíveis de detectar com métricas agregadas convencionais.

A integração com fluxos de trabalho de desenvolvimento é outro pilar fundamental. O Sentry se conecta diretamente com GitHub, GitLab, Jira e outras ferramentas do ciclo de desenvolvimento. Quando um novo erro é detectado, ele pode automaticamente criar uma issue no sistema de rastreamento da equipe, atribuir ao desenvolvedor que originalmente escreveu o código problemático (usando o blame do git), e até mesmo sugerir possíveis correções baseadas em erros similares resolvidos no passado. Após um deploy, as equipes podem monitorar a "health check" da release, observando em tempo real se a nova versão introduziu novos erros ou regressões de performance.

Para equipes que praticam SRE (Site Reliability Engineering) ou DevOps, o Sentry fornece as métricas fundamentais relacionadas à estabilidade do sistema, como o SLO (Service Level Objective) baseado em disponibilidade e latência. O cálculo de "time to resolution" - quanto tempo leva desde que um erro é detectado até ser resolvido - torna-se mensurável e otimizável.

Em essência, o Sentry.io preenche uma lacuna crítica no ecossistema de observabilidade: enquanto ferramentas como Dynatrace falam sobre "o que" está acontecendo no sistema como um todo, o Sentry fala sobre "por que" algo está acontecendo no nível do código. Ele traduz falhas de sistema abstratas em problemas de código concretos e acionáveis, fechando o loop entre operações e desenvolvimento. Para uma equipe de engenharia, isso significa menos tempo depurando cegamente e mais tempo corrigindo problemas reais que impactam usuários reais, transformando o caótico processo de lidar com erros em produção em uma disciplina sistemática e eficiente.

# 🐶 Datadog
<a href=""><img src="https://github.com/user-attachments/assets/4865a2d9-589f-4f38-a413-c321236531f4" align="right" height="77"></a>

**Datadog** é uma plataforma de monitoramento e análise baseada na nuvem, projetada para fornecer visibilidade completa sobre a infraestrutura de TI, aplicações e serviços em execução em ambientes modernos, especialmente os que utilizam arquiteturas distribuídas, microserviços, contêineres e nuvens públicas ou híbridas. 

Seu objetivo é ajudar engenheiros, desenvolvedores, times de DevOps, SRE e segurança a observarem o comportamento de seus sistemas em tempo real, correlacionando métricas, logs, rastreamentos distribuídos e eventos em uma interface unificada e de fácil uso. Com isso, o Datadog permite detectar problemas de desempenho, gargalos, falhas ou comportamentos anômalos antes que impactem os usuários finais.

O grande diferencial do Datadog é justamente essa abordagem unificada. Ele coleta dados de centenas de integrações prontas — como AWS, Azure, GCP, Docker, Kubernetes, PostgreSQL, Redis, NGINX, entre outros — e os centraliza para que se possa visualizar tudo em painéis interativos, alertar sobre condições específicas com base em regras configuráveis, e realizar análises históricas. 

O usuário não precisa se preocupar com a instalação de servidores ou infraestrutura de armazenamento local para os dados monitorados, pois tudo é processado e armazenado na nuvem da própria plataforma. Além disso, com o suporte nativo a APM (Application Performance Monitoring), é possível rastrear o tempo de execução de requisições em serviços complexos, visualizar onde ocorrem lentidões ou erros, e otimizar o desempenho do software com base em dados concretos.

Outra camada que o Datadog oferece é o monitoramento de segurança e conformidade, chamado de Cloud Security Posture Management (CSPM) e Runtime Security, que ajuda a detectar configurações erradas, vulnerabilidades, comportamentos suspeitos ou riscos em tempo real, correlacionando-os com o restante da infraestrutura observada. Há também recursos de monitoramento de experiência do usuário, como testes sintéticos, RUM (Real User Monitoring) e dashboards focados em frontend, permitindo uma visão fim a fim, do navegador do usuário até o banco de dados.

O Datadog é um serviço comercial, baseado em planos por volume de dados e quantidade de hosts monitorados. Ele é muito valorizado por empresas que operam em larga escala, principalmente pelo fato de permitir que múltiplas equipes compartilhem contexto sem silos de informação. Também oferece uma API completa e SDKs em várias linguagens para customização, além de suporte a Infrastructure-as-Code para automatizar sua configuração via Terraform, CloudFormation, entre outros. 

Com uma interface polida, rica em visualizações, e uma comunidade ativa, o Datadog se posiciona como uma das soluções mais modernas e completas no campo de observabilidade, sendo amplamente adotado em startups, corporações globais e setores com alto nível de exigência tecnológica.

# 🦖 Dynatrace
<img src="https://www.vectorlogo.zone/logos/dynatrace/dynatrace-icon.svg" align="right" height="77">

O **Dynatrace** é uma plataforma de observabilidade e inteligência de software impulsionada por IA que vai muito além do monitoramento tradicional. Em sua essência, é um sistema que fornece visibilidade completa e automatizada sobre o desempenho, a saúde e a segurança de toda a sua pilha tecnológica, desde a experiência do usuário final até a infraestrutura subjacente. 

A grande diferença em relação a ferramentas mais antigas está na sua arquitetura baseada em agentes que utilizuma tecnologia de descoberta automática e rastreamento de dependências, eliminando a necessidade de configuração manual extensiva para instrumentar aplicações.

A peça central da inovação do Dynatrace é a sua engine de inteligência artificial proprietária, chamada Davis. Diferente de sistemas de alerta comuns que dependem de limiares estáticos pré-definidos por humanos, o Davis aprende continuamente o comportamento normal de seu ambiente e, a partir dessa linha de base, é capaz de detectar automaticamente anomalias e problemas. Ele não apenas identifica que algo está errado, mas faz a correlação causal entre eventos em diferentes partes da stack para apontar a causa raiz de um problema. Por exemplo, ele pode conectar diretamente um pico no tempo de carregamento de uma página web a uma lentidão específica em um microserviço, que por sua vez foi causada por um consumo excessivo de CPU em um nó específico do Kubernetes, tudo de forma automática e em tempo real.

A plataforma é abrangente por design, cobrindo todos os pilares da observabilidade moderna. Ela monitora a experiência digital dos usuários, rastreando cada clique, transação e jornada em aplicações web e móveis, capturando não apenas métricas de desempenho, mas também a frustração ou satisfação do usuário. No nível das aplicações, ela realiza o APM (Application Performance Monitoring) com rastreamento distribuído detalhado, mapeando automaticamente todas as transações entre serviços, bancos de dados e filas de mensagens. Na infraestrutura, monitora não apenas VMs e containers, mas também serviços em nuvem, bancos de dados e redes. E, de forma crítica para os times de DevOps modernos, possui uma integração nativa e profunda com ecossistemas de orquestração como Kubernetes e OpenShift, fornecendo um mapa topológico dinâmico e em tempo real de todos os seus pods, serviços e namespaces.

Um dos conceitos mais poderosos introduzidos pelo Dynatrace é a noção de "Smartscape", que é um mapa de dependências em tempo real e auto-atualizável de toda a sua arquitetura de aplicação. Este mapa visual mostra como cada componente — desde um load balancer na AWS até um banco de dados SQL em um container — se conecta e depende dos outros. Quando um problema ocorre, o Smartscape é automaticamente destacado para mostrar o caminho exato do impacto, permitindo que os engenheiros entendam instantaneamente o escopo completo de uma falha.

Além do monitoramento de desempenho, o Dynatrace expandiu suas capacidades para incluir automação de DevOps, segurança aplicacional e gerenciamento de custos em nuvem. A plataforma pode integrar-se com pipelines de CI/CD para fornecer gating automático, onde deploys podem ser automaticamente aprovados ou revertidos com base em métricas de qualidade de serviço. Na segurança, ele identifica vulnerabilidades em tempo de execução e bibliotecas de terceiros. E no gerenciamento de nuvem, ele ajuda a identificar recursos subutilizados e otimizar gastos.

Em resumo, o Dynatrace representa uma evolução do conceito de monitoramento para uma abordagem de observabilidade contínua e automatizada. Ele substitui a sobrecarga operacional de configurar milhares de alertas e dashboards manuais por um sistema que descobre, monitora e diagnostica problemas de forma autônoma, permitindo que os times de engenharia se concentrem na construção e melhoria de produtos, em vez de gastar tempo tentando entender por que um sistema complexo e distribuído está se comportando de maneira inesperada.

# 🦡 Honeybadger
<img height="77" align="right" src="https://github.com/user-attachments/assets/7c63a975-3d56-4f60-81ae-5d9df8da0f1c" />

Quando falamos de observabilidade com **Honeybadger**, estamos entrando em um terreno que combina conceitos de engenharia de software, monitoramento e análise de falhas em aplicações. Observabilidade, de maneira geral, é a capacidade de entender o que está acontecendo dentro de um sistema complexo apenas a partir de suas saídas, como logs, métricas e traces. 

Diferente do monitoramento tradicional, que geralmente se limita a avisar quando algo está fora do normal, a observabilidade permite que você investigue profundamente as causas de problemas, entenda padrões de comportamento do sistema e até antecipe falhas antes que se tornem críticas. É uma abordagem proativa, que dá poder ao engenheiro de enxergar além do que os alertas básicos conseguem mostrar.

Honeybadger, nesse contexto, é uma ferramenta de observabilidade focada em aplicações, especialmente em sistemas web e serviços que utilizam linguagens como Ruby, Elixir, Python e JavaScript. Ele atua como um intermediário inteligente, capturando exceções, erros de runtime, falhas em background jobs e problemas de performance, e apresentando essas informações de forma estruturada para que a equipe consiga agir rapidamente. 

O diferencial do Honeybadger não está apenas em registrar erros, mas em contextualizá-los: ele mostra exatamente onde ocorreu a falha no código, quais parâmetros estavam sendo utilizados, o histórico de requisições e até o ambiente em que o erro surgiu. Isso transforma a forma como desenvolvedores lidam com problemas, passando de uma abordagem reativa, onde se corrige o que já quebrou, para uma abordagem mais investigativa e estratégica, em que se consegue entender tendências, padrões e até prevenir futuros erros.

Além disso, Honeybadger integra métricas de monitoramento e health checks, permitindo que equipes observem não apenas erros isolados, mas também o comportamento geral da aplicação ao longo do tempo. Ele se conecta a pipelines de CI/CD, sistemas de notificação e dashboards de observabilidade, criando uma visão unificada do estado do sistema. Isso significa que, com Honeybadger, a observabilidade deixa de ser apenas um conceito abstrato e se torna prática diária, proporcionando transparência, redução de downtime e aumento da confiabilidade do software. A combinação entre capturas detalhadas de erros, contexto rico e integração com o fluxo de desenvolvimento transforma o Honeybadger em uma ferramenta poderosa para qualquer equipe que queira manter sistemas complexos estáveis, resilientes e compreensíveis.

# 🍨 Elastic Stack
<img src="https://cdn.worldvectorlogo.com/logos/elastic.svg" height="77" align="right">

A empresa Elastic ajuda as organizações, seus funcionários, e clientes a acelerarem os resultados que importam com soluções de busca, monitoramento, e segurança. A empresa fornece vários serviços com seus produtos, dentre eles, o mais famoso é o **Elastic Stack**, abreviado como **ELK Stack** que é uma pilha de software de código aberto usada para coletar, armazenar, pesquisar, visualizar e analisar dados de log e outros tipos de dados em tempo real. O nome "ELK" é um acrônimo que representa os três principais componentes da pilha: **E**lasticsearch, **L**ogstach e **K**ibana.

Elastic Stack ou ELK Stack é um produto open-source designado para tratar e organizar grandes quantidades de dados em qualquer tipo de fonte e formato. Devido a sua alta capacidade de armazenamento na centralização de logs, esse recurso garante a análise e pesquisa de informações em tempo real.

<img src="https://cdn.worldvectorlogo.com/logos/elastic-stack.svg" height="77" align="right">

O ELK Stack é amplamente utilizado em operações de TI, monitoramento de sistemas e segurança da informação para coletar, analisar e visualizar logs e eventos de diversas fontes. É uma ferramenta poderosa para detectar problemas, solucionar problemas, monitorar o desempenho e a segurança de sistemas e aplicativos, e muito mais. 

Oferecendo diversos mecanismos de busca e análise, o processo de integrar e centralizar os logs em um único local nos ajuda a identificar diversos problemas com os nossos servidores e aplicações. Portanto, o Elastic Stack pode ser usado para monitorar tanto a aplicação quanto a infraestrutura em produção, oferecendo uma gama de ferramentas para coleta, armazenamento, análise e visualização de dados operacionais.

<img width="656" height="393" alt="diagram-opentelemetry-api-sdk-with-elastic-apm-agents" src="https://github.com/user-attachments/assets/223f6b93-f553-49f1-b062-c17eb117ab78" />

Com a difusão, crescimento e expansão desses projetos, a comunidade inseriu um novo projeto para coleta de dados, conhecido como **Beats**. Deste modo, a ferramenta que era formada pelo acrônimo “ELK” não tinha mais sentido com os Beats, pois iria ficar uma sopa de letrinhas. Assim, surgiu o Elastic Stack que atualmente é mantido pela Elastic.

<img src="https://user-images.githubusercontent.com/61624336/234415822-3c516b5b-9779-4c6a-bed3-78367f8b3be1.svg" height="77" align="right">

O **Elasticsearch** é um mecanismo de busca rápido e ampliável que é o coração do Elastic Stack. O Elasticsearch é um mecanismo de busca e análise distribuída altamente escalável. Ele é projetado para indexar, armazenar e recuperar dados de forma eficiente, permitindo buscas rápidas e análises avançadas. O Elasticsearch é frequentemente usado como o mecanismo de armazenamento central para dados de log e outros tipos de dados. 

Top 6 ElasticSearch Use Cases
Elasticsearch is widely used for its powerful and versatile search capabilities. The diagram below shows the top 6 use cases:

<img width="550" height="715" alt="unnamed" src="https://github.com/user-attachments/assets/eed41e05-7cfa-4da3-b0e3-0b8ab355a75c" />

Full-Text Search
Elasticsearch excels in full-text search scenarios due to its robust, scalable, and fast search capabilities. It allows users to perform complex queries with near real-time responses.

Real-Time Analytics
Elasticsearch's ability to perform analytics in real-time makes it suitable for dashboards that track live data, such as user activity, transactions, or sensor outputs.

Machine Learning
With the addition of the machine learning feature in X-Pack, Elasticsearch can automatically detect anomalies, patterns, and trends in the data.

Geo-Data Applications
Elasticsearch supports geo-data through geospatial indexing and searching capabilities. This is useful for applications that need to manage and visualize geographical information, such as mapping and location-based services.

Log and Event Data Analysis
Organizations use Elasticsearch to aggregate, monitor, and analyze logs and event data from various sources. It's a key component of the ELK stack (Elasticsearch, Logstash, Kibana), which is popular for managing system and application logs to identify issues and monitor system health.

Security Information and Event Management (SIEM)
Elasticsearch can be used as a tool for SIEM, helping organizations to analyze security events in real time.

Over to you: What did we miss?

O **Index Lifecycle Management (ILM)** é um recurso oferecido pelo Elasticsearch, um mecanismo de busca e análise distribuída, que permite gerenciar o ciclo de vida dos índices de dados armazenados no Elasticsearch. É particularmente útil para a gestão de índices de log e outros tipos de dados que têm requisitos específicos de retenção, compactação e arquivamento ao longo do tempo.

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

![unnamed](https://github.com/user-attachments/assets/623c4dfa-5758-4613-8d8d-6871a7c2a51b)

## [Elastic] How DoorDash’s In-House Search Engine Achieved a 50% Drop in Latency

> [!Warning]
> Aviso: Os detalhes deste post foram derivados dos artigos escritos pela equipe de engenharia da DoorDash. Todo o crédito pelos detalhes técnicos vai para a equipe de engenharia da DoorDash. Os links para os artigos originais estão presentes na seção de referências ao final do post. Alguns detalhes relacionados ao Luceno Apache® foram retirados da documentação oficial do Luceno® Apache. Apache Lucene® é uma marca registrada da The Apache Software Foundation. Tentamos analisar os detalhes e dar nossa opinião sobre eles. Se você encontrar alguma imprecisão ou omissão, por favor, deixe um comentário e faremos o possível para corrigi-las.

Elasticsearch é um mecanismo de busca comprovado e comprovado, utilizado por milhares de empresas.

No entanto, o que funciona em uma escala pode desmoronar em outra. E para uma empresa como a DoorDash, que opera em continentes com um mercado complexo de lojas, itens e logística, as coisas se complicam rapidamente.

No início de 2022, as rachaduras na fundação eram difíceis de ignorar.

Originalmente, a busca global do DoorDash era focada em lojas. Por exemplo, você procuraria por "pizza" e encontraria pizzarias próximas. Essa é uma consulta simples: devolva documentos marcados com pizza, organizados por localização. Mas, com o tempo, as expectativas dos usuários evoluíram. As pessoas queriam procurar itens específicos, o que significava que a busca precisava entender não só onde pedir, mas o que queriam.

Para acomodar essa mudança, o sistema precisava:

- Pesquise em vários tipos de documentos.
- Gerencie relacionamentos muitos-para-um e entre pais e filhos.
- Filtre e classifique resultados com base na disponibilidade em tempo real, geolocalização, contexto do usuário e lógica de negócios.

Elasticsearch não foi feito para isso. E embora pudesse ser forçado a cumprir esses requisitos, precisava de muito trabalho da equipe de engenharia.

Por que o Elasticsearch não foi suficiente?

Elasticsearch é uma solução amplamente adotada em empresas modernas. Veja o diagrama abaixo que mostra uma configuração típica do Elasticsearch com Logstash e Kibana:

<img width="1100" height="701" alt="unnamed" src="https://github.com/user-attachments/assets/d76c7582-de4d-455b-ba12-64757ead543b" />

No entanto, para o DoorDash, não foi suficiente por alguns motivos.

No cerne da questão estava o modelo de replicação de documentos do Elasticsearch.

Em teoria, esse modelo garante redundância e resiliência. Na prática, isso introduziu uma carga significativa que dificultava escalar horizontalmente sob a carga de trabalho do DoorDash. Cada documento indexado precisava ser replicado entre nós, o que significava mais I/O de disco, mais conversas de rede e mais sobrecarga de coordenação. Isso se tornou especialmente doloroso à medida que a plataforma cresceu e os volumes de indexação dispararam.

O segundo problema era mais profundo: o Elasticsearch não entende nativamente as relações entre documentos. Ele trata cada documento como uma ilha, o que é aceitável se você estiver pesquisando posts de blog ou arquivos de log. Mas a DoorDash precisava conectar os pontos entre lojas e itens, e essas relações eram fundamentais. Por exemplo, se uma loja sair do ar, seus itens não deveriam aparecer nos resultados de busca.

E então, há o entendimento e o ranqueamento das consultas. O DoorDash precisava de lógica de ranqueamento personalizada, ajustes de relevância movidos por ML e pontuação geo-personalizada. Com o Elasticsearch, tudo isso teve que ficar fora do motor (no código do cliente, pipelines ou sistemas upstream), tornando-o frágil e difícil de desenvolver.

Princípios de Design por Trás da Busca Interna da DoorDash: Para resolver os desafios do Elasticsearch, a DoorDash decidiu criar um mecanismo de busca que pudesse atender aos seus requisitos.

No entanto, a DoorDash não queria reinventar a recuperação de informações do zero.

Em vez disso, construíram um motor focado e de alto desempenho sobre um núcleo já testado em batalha e arquitetaram tudo em torno de flexibilidade, escalabilidade e isolamento.

**Apache Lucene® no Núcleo**: Apache Lucene® não é um mecanismo de busca. É uma biblioteca de baixo nível para indexação e consulta de texto. Pense nisso como um motor de banco de dados sem o banco de dados: sem gerenciamento de cluster, sem rede, sem APIs.

<img width="1100" height="633" alt="unnamed" src="https://github.com/user-attachments/assets/7402e805-57b5-4e3c-858a-75b30461f4ae" />

A DoorDash escolheu a Apache Lucene® por vários motivos:

- É rápido, maduro e amplamente compreendido.
- Apache Lucene® te dá primitivos para construir exatamente o que você quer.
- Já é confiável para Elasticsearch e Solr por baixo do capô.

No entanto, Apache Lucene® era apenas a base. A DoorDash envolveu isso em seus serviços opinativos, feitos sob medida para como pensam sobre busca, tráfego, escalabilidade e lógica de negócios. Isso lhes dava controle total sobre desempenho, extensibilidade e custo.

**Da Replicação de Documentos à Replicação de Segmentos**: No Elasticsearch, toda atualização significa replicar documentos completos entre nós. Isso parece bom até você processar milhares de mudanças por segundo.

A DoorDash encontrou um caminho melhor: a replicação de segmentos.

Em vez de duplicar documentos, eles replicam segmentos de índice do Apache Lucene®: as estruturas reais no disco construídas durante a indexação. Isso lhes deu alguns benefícios:

- Otimizar indexação e desempenho em busca
- Redução do custo de computação, já que o trabalho de indexação ocorre apenas no nó primário, não em todas as réplicas.
- Aumento do rendimento de indexação

Ao tratar os segmentos como unidade de replicação, o sistema conseguiu reduzir o churn e manter os nós de busca enxutos e estáveis.

**Desacoplamento, Indexação e Busca**: Um padrão comum de falha em sistemas de busca é acoplar os caminhos de escrita e leitura de forma muito apertada. Se a indexação disparar, a busca desacelera. Se as consultas se acumularem, a indexação trava. DoorDash não queria isso.

Então eles dividiram as coisas de forma limpa:

- O Serviço de Indexação constrói segmentos do Apache Lucene® e os grava na Amazon S3. É um serviço não replicado porque escalar horizontalmente o indexador significa aumentar o número de fragmentos de índice, o que pode ser caro.
- O Serviço de Busca (totalmente replicado) baixa segmentos do S3 e atende consultas.

A recompensa disso foi enorme. Os indexadores escalavam com base na carga de escrita, enquanto os buscadores escalavam com base no tráfego de leitura. Nenhum dos dois conseguiu derrubar o outro.

Componentes Principais do Mecanismo de Busca do DoorDash: O diagrama abaixo mostra a arquitetura de pilha de busca de alto nível implementada pelo DoorDash:

<img width="1100" height="1375" alt="unnamed" src="https://github.com/user-attachments/assets/ab2dbaae-a0e6-428c-87aa-3d28d8b2dd9f" />

Existem quatro componentes principais dentro do Motor de Busca DoorDash. Vamos analisar cada um em detalhes:

1 - O Indexador
O indexador é a parte do sistema que transforma dados brutos, menus, informações de armazenamento e disponibilidade de itens em segmentos Lucene® que podem ser consultados de forma eficiente. Não atende a nenhuma dúvida. É um pipeline apenas de escrita, enviando segmentos finalizados do Apache Lucene® para a S3, onde os buscadores podem encontrá-los.

Mas nem todos os dados são iguais. Algumas mudanças precisam ser lançadas agora (como uma loja ficando offline). Outros podem esperar (como um novo item do menu adicionado para a próxima semana). DoorDash lida com isso com indexação em dois níveis:

Atualizações de alta prioridade: pense em alternâncias de disponibilidade, fechamento de lojas ou mudanças de preço. Essas atualizações são implementadas imediatamente e são essenciais para a experiência do usuário.

Atualizações em massa: Essas são menos sensíveis ao tempo e processadas durante reconstruções completas programadas do índice, normalmente a cada seis horas.

Essa estratégia equilibra frescor com desempenho. Se tudo fosse indexado imediatamente, poderia sufocar o pipeline. Se tudo fosse lote, os resultados poderiam ficar sem graça. Dividir o caminho permite que o sistema permaneça rápido e preciso.

2 - O Buscador
Searchers são serviços replicados que baixam segmentos pré-construídos do S3 e os usam para responder às dúvidas dos usuários.

Aqui estão alguns pontos-chave sobre eles:

Os buscadores nunca lidam com tráfego de indexação. Em outras palavras, eles não são impactados pelos picos de escrita.

Escale horizontalmente com base no tráfego de leitura

Pode ser trocado e trocado sem reindexação, já que os segmentos são imutáveis e versionados.

Essa separação de preocupações mantém o sistema estável. Mesmo quando a indexação está ocupada, a busca continua rápida. Quando o tráfego de busca dispara, a indexação permanece no caminho certo.

3 - O Corretor
Em um sistema de busca distribuído, os resultados vivem em muitos shards. Então, quando alguém busca um termo, o sistema precisa:

Espalhe a consulta para cada fragmento relevante.

Colete e junte os resultados.

Classifique e devolva.

Esse é o trabalho do corretor.

Mas o corretor não encaminha a consulta apenas para o local. Antes de fazer qualquer coisa, ele executa a entrada por um Serviço de Compreensão e Planejamento de Consultas. Isso significa que a entrada bruta do usuário, erros ortográficos, sinônimos e contexto de localização são transformados em uma consulta limpa e semanticamente rica que faz sentido para o motor.

4 - Planejamento e Compreensão de Consultas
A busca só é tão boa quanto sua consulta. Os usuários nem sempre digitam o que querem dizer. Além disso, diferentes unidades de negócio podem precisar de modelos de classificação ou regras de filtro diferentes.

Em vez de empurrar toda essa lógica para os clientes (o que causaria duplicação, desvio e problemas), o DoorDash centralizou tudo em um serviço de Planejamento e Compreensão de Consultas.

Esta camada:

Reescreve consultas do usuário com base na lógica de negócios, conhecimento de esquemas e contexto do usuário.

Aplica regras e transformações específicas do tipo de índice (item vs. loja).

Codifica estratégias de classificação e lógica computada de campos.

Dessa forma, os clientes não precisam microgerenciar a estrutura da consulta. Eles enviam intenções de alto nível, e o planejador de consultas cuida da complexidade.

Esquema de Índice e Linguagem de Consulta
Os sistemas de busca tendem a se fragmentar de duas maneiras:

O esquema é rígido demais, então todo novo caso de uso precisa de um truque.

A linguagem de consulta é muito abstrata, então a lógica de negócios acaba enterrada em código de configuração ou cliente ilegível.

A DoorDash enfrentou ambos os problemas de frente. Eles construíram um sistema de esquemas declarativo, expressivo e extensível, que trata a busca não como correspondência de texto, mas como uma recuperação estruturada e contextual de informações.

Configuração de Índice Declarativo
O primeiro princípio era a separação das preocupações: a lógica de negócio pertence ao esquema, não espalhada entre bases de código. Assim, o DoorDash permite que as equipes definam seu comportamento de busca de forma declarativa, usando três conceitos centrais:

1 - Campos Indexados
Esses são os ingredientes brutos que são armazenados no índice invertido da Lucene® Apache. Eles podem ser:

Campos de texto: Tokenizados e pontuados com modelos como BM25.

Valores numéricos ou valores de documentação: Usados para filtragem, ordenação ou reforço.

Vetores KNN: Para busca semântica ou correspondência baseada em embedding.

Pontos dimensionais: Úteis para coisas como geobusca ou faixas de preço.

Esses são processados em tempo de indexação: rápido para consulta, estático até reindexação.

2 - Campos Calculados
Os campos computados são avaliados no momento da consulta, com base em:

A própria consulta

Valores de campo indexados

Outros campos computados

3 - Pipelines de Planejamento de Consultas
Essa é a cola que conecta a intenção à execução.

Um pipeline de planejamento de consultas pega uma consulta bruta do usuário, frequentemente incompleta, bagunçada ou ambígua, e a transforma em uma consulta de busca estruturada e executável.

Essa lógica fica em um só lugar, não está codificada diretamente nos clientes, então é fácil de versar, atualizar e reutilizar.

Namespaces e Relações
Você não pode construir um motor de busca real sem modelar relacionamentos.

Na DoorDash, as lojas têm itens, e essa relação é importante. Você não quer itens órfãos aparecendo quando a loja principal estiver fechada. Para modelar isso, o esquema suporta namespaces (classes de documentos fortemente tipadas) e relacionamentos entre eles.

Cada namespace representa um tipo distinto de documento, como armazenar, item e categoria. Esses tipos de documento possuem seus campos, configurações de índice e lógica.

DoorDash suporta dois tipos de relacionamentos entre namespaces, cada um com concessões:

Na junção local, o filho é indexado apenas se o pai o referenciar. Isso é usado quando a flexibilidade importa.

Na junção em blocos, o pai e os filhos são indexados juntos como uma única unidade. Isso é usado ao otimizar para latência, e não há problema em reindexar lotes.

Linguagem de Consulta do Tipo SQL: O DoorDash construiu uma API semelhante a SQL que permite às equipes descrever consultas de forma clara e clara. Esta linguagem suporta:

- Grupos de palavras-chave: Por exemplo, busque por sinônimos, raízes, categorias
- Restrições do filtro: faixa de preço, raio geográfico, limiar de avaliação
- Ordenação: Por pontuação, distância, frescura ou qualquer lógica personalizada
- Operações de entrada e desduplicação: Evite listagens duplicadas ou resultados mal definidos
- Seleção de campos: Devolver apenas os campos necessários para sistemas a jusante

A linguagem de consulta oferece aos engenheiros uma forma limpa e legível de construir consultas poderosas. Também estabelece um contrato consistente entre as equipes.

Isolamento da Pilha de Busca e Plano de Controle: A maioria dos sistemas compartilhados eventualmente cede sob seu peso, não porque a lógica central falha, mas porque os inquilinos pisam uns nos outros, implantações colidem e desvios de configuração criam bugs sutis e difíceis de depurar.

O DoorDash previu isso e fez uma decisão de design ousada: todo índice recebe sua pilha de busca isolada. Não é a abordagem leve. Mas é uma das mais confiáveis.

Pense em uma pilha de busca como um mecanismo de busca autônomo dentro de uma caixa. Inclui:

Um indexador para construir segmentos Apache Lucene®.

Um ou mais Searchers para atender consultas.

Um corretor que se espalha, agrega e classifica.

Metadados de esquema, configuração e versão que são escopados apenas para esse índice.

Cada pilha está vinculada a um índice e caso de uso específicos, como busca global de itens, descoberta de loja ou busca em campanhas promocionais.

<img width="1100" height="589" alt="unnamed" src="https://github.com/user-attachments/assets/42b96098-4bb9-4ceb-bfc2-55d27e0e33b0" />

Esse projeto traz muita facilidade operacional devido aos seguintes motivos:

- Estabilidade: Se uma configuração ruim de índice ou segmento corrompido derruba uma pilha, as outras permanecem ativas.
- Flexibilidade: Diferentes equipes podem usar diferentes planejadores de consultas, esquemas, modelos de ranking ou pipelines sem coordenação.
- Rastreabilidade: Uso de recursos, desempenho de consultas e atraso de indexação podem ser atribuídos à equipe proprietária. Chega de apontar o dedo durante as avaliações de incidentes.

Uma pergunta, porém, permanece: se cada equipe tem sua pilha, como você gerencia lançamentos, mudanças de esquema e novas implantações sem introduzir caos?

É aí que o plano de controle entra. É uma camada de orquestração responsável por:

Lançando novas gerações de uma pilha de busca.

Gerenciando implantações versionadas (código + esquema + config).

Aumentando gradualmente novas instâncias e desativando as antigas.

Conclusão: Reconstruir a infraestrutura central é sempre arriscado e complexo. Então, quando o DoorDash migrou do Elasticsearch, o risco era alto. Mas o resultado valeu a pena.

Aqui estão alguns ganhos que eles alcançaram:

Redução de 50% na latência p99.9. Essa não é a latência média, mas a latência de cauda que tem maior impacto em momentos de alto tráfego. Reduzir pela metade o p99.9 significa menos tempos de espera, experiência do usuário mais suave e menos necessidade de superprovisionamento.

Queda de 75% nos custos de hardware. Ao reduzir computações redundantes, diminuir a sobrecarga de replicação e melhorar o isolamento da carga de trabalho, a DoorDash reduziu drasticamente a pegada de sua infraestrutura de busca.

No fim das contas, a DoorDash não construiu apenas um mecanismo de busca, mas uma plataforma inteira que roda mais rápido, custa menos e se adapta melhor às necessidades futuras.

Nota: Apache Lucene® é uma marca registrada da Apache Software Foundation.

# ☀️ Grafana Stack
<img src="https://img.shields.io/badge/Grafana_Stack-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white"> <img src="https://img.shields.io/badge/Grafana-25.3.2-F46800?style=flat&logo=Grafana&logoColor=white"> <img src="https://img.shields.io/badge/Prometheus-25.3.2-E6522C?style=flat&logo=Prometheus&logoColor=white"> <img src="https://img.shields.io/badge/OpenTelemetry-25.3.2-gold?style=flat&logo=OpenTelemetry&logoColor=white">

<a href="https://grafana.com/"><img src="https://cdn.worldvectorlogo.com/logos/grafana.svg" align="right" height="77"></a>

O **Grafana Stack** é um conjunto de ferramentas desenvolvidas e mantidas pela Grafana Labs com o objetivo de fornecer uma plataforma completa e integrada para observabilidade, ou seja, para o monitoramento, análise e visualização de dados de sistemas, aplicações, infraestrutura e serviços. Ele é muito utilizado por equipes de DevOps, SREs e engenheiros de software para entenderem como os sistemas estão se comportando em tempo real, detectar falhas, identificar gargalos e manter a confiabilidade dos ambientes em produção. 

A base desse ecossistema (stack) é o Grafana, uma ferramenta open source de visualização de métricas, logs e traces que permite a criação de dashboards interativos altamente customizáveis.

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

<img src="https://github.com/user-attachments/assets/31458caf-6921-42a6-a8bf-636f587c2f23" align="right" height="77">

O **Mimir**, dentro do ecossistema Grafana, é um banco de dados de métricas de longo prazo, open-source e horizontalmente escalável, projetado especificamente para resolver os gargalos de desempenho e operacionais que surgem quando os ambientes de monitoramento baseados em Prometheus crescem para escalas massivas. Ele representa a evolução natural do Prometheus para um contexto empresarial, atuando como uma camada de armazenamento e agregação que permite a centralização de dados de centenas ou mesmo milhares de clusters Prometheus distribuídos, sem sacrificar a performance de consulta ou a confiabilidade.

A motivação fundamental por trás do Mimir é um desafio comum em organizações com infraestruturas complexas: a fragmentação de dados. Em uma arquitetura típica, cada time ou aplicação pode ter seu próprio Prometheus, criando silos de métricas onde é impossível correlacionar eventos entre diferentes domínios. O Mimir quebra esses silos ao oferecer um backend único e unificado para todos os dados de métricas, permitindo consultas globais que abrangem toda a organização. Ele é compatível com a API do Prometheus, o que significa que ferramentas existentes como o Grafana podem se conectar a ele de forma transparente, como se fosse um Prometheus local, mas com a capacidade de acessar um volume de dados ordens de magnitude maior.

Sua arquitetura é construída desde a base para a escala, seguindo um design de microserviços que separa claramente as funções de ingestão, armazenamento e consulta. Esta separação permite que cada componente seja dimensionado independentemente conforme a demanda. A ingestão, por exemplo, pode lidar com milhões de amostras por segundo de diversos provedores, não apenas do Prometheus, mas também de agentes como o Grafana Agent ou qualquer sistema que fale o protocolo de remoto write. O armazenamento utiliza uma estratégia de objetos, frequentemente integrado a backends como Amazon S3, Google Cloud Storage ou Azure Blob Storage, o que elimina a necessidade de gerenciar discos locais complexos e oferece durabilidade e custo imbatíveis. A engine de consulta é otimizada para executar PromQL de forma distribuída e eficiente, mesmo sobre petabytes de dados históricos, utilizando técnicas avançadas de paralelização e cache.

Uma das características mais poderosas do Mimir é a sua capacidade de realizar queries em tempo real sobre dados altamente compactados e armazenados de forma econômica em object storage. Isto resolve o dilema clássico entre retenção de dados de longo prazo e custo de armazenamento. As empresas não precisam mais decidir entre deletar dados históricos valiosos para economizar custos ou pagar fortunas para mantê-los em sistemas caros de armazenamento de séries temporais. Com o Mimir, é possível reter anos de dados métricos a um custo acessível, mantendo a capacidade de consultá-los com performance interativa, o que é fundamental para análise de tendências, planejamento de capacidade e investigação forense de incidentes passados.

<img width="4036" height="1576" alt="mimir-how-does-it-work" src="https://github.com/user-attachments/assets/2420d5f5-ae92-4749-9e90-c6982b55b900" />

Além da escala e economia, o Mimir introduz funcionalidades de nível empresarial que faltam no Prometheus puro. Isto inclui controle de acesso fino (RBAC) para determinar quais times podem ver ou modificar quais métricas, limites de taxa (rate limiting) configuráveis para prevenir que queries malformadas sobrecarreguem o sistema, e a capacidade de criar "regras de gravação" que agregam métricas em tempo real, permitindo a criação de métricas consolidadas de alto nível a partir de milhares de métricas brutas. A alta disponibilidade é inerente ao design, com replicação de dados e tolerância a falhas de componentes, garantindo que o sistema de monitoramento, que é crítico para a operação do negócio, permaneça sempre operacional.

Em essência, o Mimir não é um substituto para o Prometheus, mas sim seu complemento ideal em ambientes de grande escala. Ele permite que as organizações mantenham a simplicidade operacional e o modelo de dados do Prometheus em cada unidade de deploy, enquanto colhe os benefícios de um data lake de métricas corporativo. Ele transforma o monitoramento de uma coleção de instâncias independentes e desconectadas em um sistema nervoso centralizado e unificado para a infraestrutura inteira, permitindo que engenheiros façam perguntas ambiciosas sobre o comportamento de seus sistemas em qualquer escala de tempo, desde segundos até anos, com a mesma facilidade e velocidade. É a materialização da visão de que, na era da nuvem, o monitoramento não deve ser um luxo ou um custo proibitivo, mas uma utilidade pública dentro da organização, tão confiável e escalável quanto a própria plataforma que ela observa.

<img alt="800px-OBS" src="https://github.com/user-attachments/assets/f092945d-cc75-4ec6-a620-599acd6b22fb" />


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
