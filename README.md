# observability
🔍 It's a repository of Observability from scratch.

# Zabbix

# New Relic

# UptimeRobot

# Datadog

# Elastic Stack

# Grafana Stack

# Typesense
**Typesense** é um mecanismo de busca de código aberto, criado para oferecer uma alternativa moderna, rápida e fácil de usar em comparação com ferramentas mais complexas como Elasticsearch e Solr. Ele é projetado com foco na simplicidade e na performance, tornando-se ideal para desenvolvedores que desejam implementar funcionalidades de busca com qualidade, sem precisar configurar ou manter uma infraestrutura muito pesada. O Typesense é escrito em C++ e otimizado para oferecer tempos de resposta muito baixos, mesmo com grandes volumes de dados. A ideia central é facilitar a indexação e a consulta de dados estruturados, como registros de produtos, usuários, artigos ou qualquer outro conjunto de documentos que possa se beneficiar de busca textual eficiente.

O grande diferencial do Typesense é sua abordagem voltada para o desenvolvedor. Sua API é simples, baseada em REST, com opções modernas de integração que funcionam bem em back-ends e também diretamente em front-ends. Ele oferece recursos como tolerância a erros de digitação (fuzzy search), autocompletar, ordenação por relevância e por campos personalizados, filtros facetas, e indexação em tempo real, o que permite que os dados atualizados sejam quase imediatamente refletidos nos resultados de busca. Isso é especialmente útil em sistemas de e-commerce, catálogos, dashboards administrativos ou portais de notícias.

O Typesense pode ser usado localmente ou como serviço em nuvem, através do Typesense Cloud, que elimina a necessidade de configuração manual de servidores. Ele foi criado para consumir poucos recursos e ainda assim fornecer desempenho de nível profissional. A instalação e a configuração são diretas: é possível ter um cluster funcional em minutos. Ele também oferece SDKs e bibliotecas para diversas linguagens como JavaScript, Python, Ruby e outros, facilitando ainda mais sua adoção em projetos variados. Além disso, a estrutura de indexação dele é baseada em esquemas simples, o que ajuda a manter a clareza dos dados e evitar erros durante a indexação ou consulta.

Em um cenário onde a busca é uma funcionalidade crítica — seja para melhorar a experiência do usuário final, seja para oferecer relatórios ou filtros poderosos — o Typesense surge como uma solução eficiente, moderna e acessível, com uma curva de aprendizado muito menor que seus concorrentes tradicionais, sem abrir mão de funcionalidades robustas e performance de alto nível.

# OpMon
<img src="https://github.com/user-attachments/assets/719e67fe-2882-447e-9e45-bda77564fcc3" align="right" height="177">

O **OpMon** é uma plataforma brasileira de monitoramento de infraestrutura de TI, redes, servidores, serviços, aplicações e negócios, desenvolvida com o objetivo de proporcionar visibilidade completa e em tempo real sobre os ativos tecnológicos de uma organização. Ele se baseia em conceitos como observabilidade, automação e análise proativa de falhas para oferecer um ambiente de monitoramento robusto, permitindo que as equipes de tecnologia antecipem problemas, identifiquem gargalos e tomem decisões com mais agilidade e segurança.

A ferramenta se destaca por ser altamente personalizável e adaptável a diferentes cenários corporativos. Ela é capaz de monitorar tanto ativos locais quanto ambientes em nuvem ou híbridos, integrando diferentes protocolos como SNMP, WMI, SSH, API REST, entre outros. Com dashboards interativos, gráficos de desempenho, alertas por diversos canais (e-mail, SMS, Telegram, etc.) e recursos como relatórios automatizados e detecção de anomalias, o OpMon se torna um aliado essencial para times de infraestrutura e operações, permitindo uma gestão proativa e eficiente.

Além disso, o OpMon permite a correlação entre indicadores técnicos e processos de negócio, criando uma camada de monitoramento orientada ao impacto nos serviços finais da empresa. Isso significa que é possível acompanhar o funcionamento de um sistema de forma mais contextualizada, considerando seu papel no fluxo operacional da empresa como um todo. Ele também possui recursos de integração com ITSMs, CMDBs e ferramentas de automação, promovendo um ecossistema de TI mais coeso e inteligente.

Por ser uma solução nacional, o OpMon se alinha às necessidades do mercado brasileiro, com suporte técnico especializado, documentação em português e atualizações constantes que acompanham as tendências de TI. Sua adoção é comum em ambientes corporativos que exigem alta disponibilidade, controle rigoroso de SLA e visibilidade completa sobre os recursos tecnológicos, posicionando-se como uma alternativa sólida frente a soluções internacionais de monitoramento.

O OpMon pode ser considerado **equivalente em propósito**, mas **não idêntico em arquitetura e escopo** a ferramentas como Grafana Stack, Elastic Stack, Datadog, Zabbix e New Relic. Todos esses sistemas compartilham o objetivo principal de monitorar infraestrutura, aplicações e serviços de TI, mas cada um tem enfoques, arquiteturas e diferenciais técnicos distintos.

O OpMon, por ser uma plataforma nacional, tem uma abordagem **mais integrada e pronta para uso**, com foco em **monitoramento unificado** e **correlação entre TI e negócio**, sem exigir que o usuário monte ou componha diferentes partes de uma stack. Ele possui coleta de métricas, geração de alertas, visualização gráfica, automação de respostas e gestão de disponibilidade, atuando de forma semelhante ao Zabbix e ao Datadog em sua proposta de “tudo em um”.

O Grafana Stack (com Prometheus, Loki, Tempo, etc.) e o Elastic Stack (com Elasticsearch, Logstash, Kibana) são **plataformas altamente modulares**, onde cada componente tem uma responsabilidade clara (como logs, métricas ou tracing) e precisam ser integrados manualmente. Eles oferecem **grande flexibilidade**, sendo ideais para times com maturidade técnica e que desejam controle fino sobre cada etapa da observabilidade.

Já o Datadog e o New Relic são soluções **SaaS completas**, com forte foco em observabilidade como serviço (metrics, logs, traces, synthetics, APM), integração com centenas de tecnologias e interface unificada, com foco em **performance de aplicações e experiência do usuário final**. São geralmente mais abrangentes que o OpMon em termos de APM e suporte a instrumentação automática, mas exigem orçamentos mais altos.

O Zabbix, por sua vez, tem um modelo mais próximo do OpMon, sendo uma solução open source robusta para monitoramento de rede e infraestrutura, com foco em escalabilidade, alertas e desempenho. A principal diferença é que o Zabbix tem uma **comunidade internacional enorme e arquitetura baseada em agentes**, enquanto o OpMon foca mais no mercado brasileiro e em uma integração mais “turn-key” com visualização voltada ao negócio.

Portanto, o OpMon **é comparável em finalidade**, mas seu posicionamento está mais próximo de ferramentas como **Zabbix e Datadog**, combinando recursos de monitoramento com usabilidade empresarial e suporte local. Já Grafana Stack, Elastic Stack e New Relic oferecem maior customização e profundidade, especialmente em ambientes que exigem alta observabilidade distribuída.
