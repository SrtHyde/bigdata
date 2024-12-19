# Ciência de Dados para Negócios

# Universidade Federal da Paraíba

## Atividade I

Leitura e fichamento do capítulo I - Livro: Big Data
Concepts, Technology, and Architecture

**Introduction to the World of Big Data**

Balamurugan Balusamy, Nandhini Abirami. R, Seifedine Kadry, and Amir H. Gandomi

**Aluno**: Bianca Maria Souza Pedrosa

**Matrícula**

## Instruções

```bash
# clonar o repositório
git clone git@github.com:hiltonmbr/bigdata.git
# criar uma branch com sua matrícula
git checkout -b <sua matrícula>
# Criar o arquivo markdown 
# Copiar e colar o conteúdo do README.md
# Editar o arquivo CAPITULO1.md e salvar commits em sua branch
git push origin <sua matrícula>
# Ao finalizar, abrir um pull request
```

# 1. Introdução

## 1.1 Entendendo o Big Data

- Big data não é apenas um conjunto muito grande de dados, corresponde a um conjunto de dados com características como: velocidade de ingestão e processamento, variedade de tipos de dados e volume de dados que ultrapassam terabytes de memória.
- Big data deve possuir dados veridicos e que ao analisar gerem valor ao negócio.
- Big data por ser complexo em sua natureza deve ser manipulado utilizando ferramentas e estruturas de hardware adequados.

## 1.2 Evolução do Big Data

- A primeira aparição do big data foi emum artigo da nasa em 1997.
- O ciclo de processamento do Big Data inclui etapas como aquisição, pré-processamento, armazenamento, gestão, privacidade, segurança, análise e visualização.
- A quantidade de dados cresceu significativamente ao longo das décadas, passando de 600 MB na década de 1950 para 100 petabytes em 2010.

## 1.3 Falha dos Bancos de dados relacionais em lidar com Big Data

- Quase 80% dos dados obtidos estavam em formatos semiestruturados e não estruturados, os quais os SGBDs relacionais não conseguiam processar adequadamente.
- A velocidade de entrada dos dados não é suportada em bancos de dados relacioonais.
- Para tentar se adequar a big data é necessário aumentar o número de processadores o que eleva o custo no uso de SGBDs relacionais.

## 1.3.1 Data Mining vs Big Data

- Mineração de Dados: Processo de descobrir conhecimentos ocultos em conjuntos de dados; Capaz de processar grandes volumes de dados, mas com custos elevados; Limita-se a dados que variam de gigabytes a terabytes.
- Big Data: Capaz de armazenar e processar dados de petabytes a zettabytes com custos mais baixos; Lida com dados estruturados, semiestruturados e não estruturados, geralmente em bancos não relacionais (NoSQL).

## 1.4 ­3Vs of Big Data

- **Volume**: O volume de captura de dados de Big Data vai de terabytes até zettabytes
- **Variedade**: Dados normalmente são não estruturados, como videos, audio, texto de sites, e-mails, mensagens, fotos e etc.
- **Velocidade**: A geração de dados chega a ser de dados por segundo, por isso os dados precisam de rápido processamento para atualizaçãoes constantes das informações.

## 1.5 Fontes do Big Data

- Os dados que compõem o big data podem vir de diversas fontes como: sensores,  sistemas de saúde, sistemas de transporte aéreo,  plataformas de vendas online, redes sociais, dados organizacionais e de transações financeiras.

## 1.6 Tipos Diferentes de Dados

- Dados Gerados por Humanos: Correspondem a dados criados a partir de interações humanas com máquinas. Como: e-mails, documentos e postagens em redes sociais.
- Dados Gerados por Máquinas: Dados produzidos por softwares ou máquinas sem intervenção de humanos. Como: logs de sites, dados de satélites, alertas de desastres, sensores e etc
- Podemos ter também diferentes tipos de dados no big data. São eles:
    - **Dados Estruturados:** Dados tabulados, como em planilhas e bancos de dados relacionais.
    - **Dados Semistruturados:** Arquivos Json e Xml, que possuem um tipo de hierarquia e organização de dados mas não sgeuem os padrões tabulares.

## 1.7 Infraestrutura de Big Data

- O modelo tradicional de armazenamento em tabelas (RDBMS) tornou-se caro e ineficiente no contexto do big data, por isso foram desenvolvidos softwares e ferramentas que premitissem a ecalabilidade e o menor custo no processamento desses dados.
- Algumas tecnologias mais comuns são:
    - **Hadoop**: Corresponde a um Framework de código aberto, que permite armazenar e processar dados estruturados, semiestruturados e não estruturados em sistemas distribuídos. Ele utiliza  clusters (grupos de computadores interconectados) para processar grandes volumes de dados de maneira eficiente.
    - **MapReduce**: Esse modelo de programação é  baseado no princípio de "dividir e conquistar”. Processa dados em paralelo e reduz significativamente o tempo de processamento.
    - **HDFS (Hadoop Distributed File System)**: Correspond a um sistema de arquivos distribuídos projeto para lidar com grandes bases de dados com hardaware de baixo custo.

## 1.8 Ciclo de Vida do Big Data

- O ciclo de Vida do Big Data pode ser descrito através de 6 etapas principais:
    - **Captura de dados**: Os dados gerados são coletados de diferentes fontes e podem te diversos formatos.
    - **Armazenamento de dados**: Dados capturados são armazenados e preparados para um futuro processamento, removendo redundancias e garantindo a objetividade dos dados.
    - **Pré-processamento**: Realiza cáculos e organiza os dados para a análise futura, realiza limpeza, redução, integração e transformação.
    - **Integração de dados**: Envolve a combinação de dados de várias fontes para a vizualização única dos dados, ou seja padronização das entradas.
    - **Limpeza de dados**:  Trata valores faltantes, corrige erros e inconsistencias nos dados
    - **Redução de dados**: Agrupamento e seleção de dados cruciais para a análise, inclui compressão dos dados, redução de dimensionalidade e redução de numerosidade.
    - **Transformação dos Dados**: Consiste em transformar e consolidar os dados no tipo apropriado para análise e gestão. Envolve a aplicação de técnicas como agrupamento de dados, generalização, dicretização e suavização.
    - **Análise:** Aplicação de modelos para a extração de informações relevantes para o negócio.
    - **Vizualização:** Consiste na apresentação dos resultados e informações relevantes extraídas do Big Data, com o uso de gráficos, dashboards e relatórios.

## 1.9 Tecnologia do Big Data

- Uma das tecnologias mais usadas para a manipulação de Big Data é o Apache Hadoop. O Hadoop possui alguns componentes principais, são eles: **HDFS** (Hadoop Distributed File System), **Hadoop Common** (uma coleção de utilitários comuns que suportam outros módulos do Hadoop), **MapReduce**, **Yarn** (Yet Another Resource Negotiator).
- Mesmo com a criação das tecnologias de Big Data, o gerenciamento desses dados ainda sofre vários desafios como: a imcompletude dos dados, tamanho do armazenamento necessário, privacidade de dados , variedade de tipos de dados e velocidade de processamento.

## 1.10 Aplicações do Big Data

- Cuidados com a Saúde: A área da saúde possui dados cmplexos e de crescimento rápido, a implementação de aoluções de big data podem ajudar a analisar e processar dados de maneira rápida e com baixo custo. Alguns usos nessa área podem ser destacados como:
    - Monitoramento remoto de pacientes
    - Registros eletrônicos de saúde para otimização do diagnóstico
    - Saúde baseada em evidências → laudos médicos, sinais biomédicos e etc
    - Descoberta de padrões para prevenção e tratamento de doenças
- Telecomunicações: Os dados de ráfego de rede, dados de chamadas e comportamentodo cliente são muito importantes para empresas. Por isso o big data pode ser usado como uma estratégia para a retenção de clientes com a personalização de planos e serviços, detceção de anomalias e fraudes, otimização de estratégias de marketing, previsão de desempenho de produtos e etc.
- Serviços Financeiros: No ramo de finanças ter as informações mais atualizadas é crucial para melhor desempenho na gestão de riscos. O big data pode ajudar a promover diversos benefícios, como:
    - Insights de dados ajudam consultores a orientarem investimentos.
    - Avaliação de crédito baseada em comportamento de compra, atividades sociais e parcerias empresariais.
    - Análise preditiva detecta padrões de fraudes e previne fraudes em cartões de crédito em tempo real.

## 1.1 Entendendo o Big Data

- Big Data não é apenas um conjunto muito grande de dados; corresponde a um conjunto de dados com características como: velocidade de ingestão e processamento, variedade de tipos de dados e volume de dados que ultrapassam terabytes de memória.
- Big Data deve possuir dados verídicos e que, ao serem analisados, gerem valor ao negócio.
- Big Data, por ser complexo em sua natureza, deve ser manipulado utilizando ferramentas e estruturas de hardware adequados.

## 1.2 Evolução do Big Data

- A primeira aparição do Big Data foi em um artigo da NASA em 1997.
- O ciclo de processamento do Big Data inclui etapas como aquisição, pré-processamento, armazenamento, gestão, privacidade, segurança, análise e visualização.
- A quantidade de dados cresceu significativamente ao longo das décadas, passando de 600 MB na década de 1950 para 100 petabytes em 2010.

## 1.3 Falha dos Bancos de Dados Relacionais em Lidar com Big Data

- Quase 80% dos dados obtidos estavam em formatos semiestruturados e não estruturados, os quais os SGBDs relacionais não conseguiam processar adequadamente.
- A velocidade de entrada dos dados não é suportada em bancos de dados relacionais.
- Para tentar se adequar ao Big Data, é necessário aumentar o número de processadores, o que eleva o custo no uso de SGBDs relacionais.

## 1.3.1 Data Mining vs. Big Data

- **Mineração de Dados**: Processo de descobrir conhecimentos ocultos em conjuntos de dados; capaz de processar grandes volumes de dados, mas com custos elevados; limita-se a dados que variam de gigabytes a terabytes.
- **Big Data**: Capaz de armazenar e processar dados de petabytes a zettabytes com custos mais baixos; lida com dados estruturados, semiestruturados e não estruturados, geralmente em bancos não relacionais (NoSQL).

## 1.4 3Vs do Big Data

- **Volume**: O volume de captura de dados do Big Data vai de terabytes até zettabytes.
- **Variedade**: Dados normalmente não estruturados, como vídeos, áudios, textos de sites, e-mails, mensagens, fotos etc.
- **Velocidade**: A geração de dados ocorre em grandes volumes por segundo; por isso, os dados precisam de rápido processamento para atualizações constantes das informações.

## 1.5 Fontes do Big Data

- Os dados que compõem o Big Data podem vir de diversas fontes, como: sensores, sistemas de saúde, sistemas de transporte aéreo, plataformas de vendas online, redes sociais, dados organizacionais e transações financeiras.

## 1.6 Tipos Diferentes de Dados

- **Dados Gerados por Humanos**: Correspondem a dados criados a partir de interações humanas com máquinas, como e-mails, documentos e postagens em redes sociais.
- **Dados Gerados por Máquinas**: Dados produzidos por softwares ou máquinas sem intervenção humana, como logs de sites, dados de satélites, alertas de desastres, sensores etc.
- Diferentes tipos de dados no Big Data incluem:
    - **Dados Estruturados**: Dados tabulados, como em planilhas e bancos de dados relacionais.
    - **Dados Semiestruturados**: Arquivos JSON e XML, que possuem uma hierarquia e organização, mas não seguem os padrões tabulares.

## 1.7 Infraestrutura de Big Data

- O modelo tradicional de armazenamento em tabelas (RDBMS) tornou-se caro e ineficiente no contexto do Big Data; por isso, foram desenvolvidos softwares e ferramentas que permitissem escalabilidade e menor custo no processamento desses dados.
- Algumas tecnologias mais comuns são:
    - **Hadoop**: Framework de código aberto que permite armazenar e processar dados estruturados, semiestruturados e não estruturados em sistemas distribuídos. Ele utiliza clusters (grupos de computadores interconectados) para processar grandes volumes de dados de maneira eficiente.
    - **MapReduce**: Modelo de programação baseado no princípio de "dividir e conquistar”. Processa dados em paralelo e reduz significativamente o tempo de processamento.
    - **HDFS (Hadoop Distributed File System)**: Sistema de arquivos distribuídos projetado para lidar com grandes bases de dados com hardware de baixo custo.

## 1.8 Ciclo de Vida do Big Data

- O ciclo de vida do Big Data pode ser descrito através de seis etapas principais:
    - **Captura de Dados**: Os dados gerados são coletados de diferentes fontes e podem ter diversos formatos.
    - **Armazenamento de Dados**: Dados capturados são armazenados e preparados para um futuro processamento, removendo redundâncias e garantindo a objetividade dos dados.
    - **Pré-processamento**: Realiza cálculos e organiza os dados para a análise futura; inclui limpeza, redução, integração e transformação.
    - **Integração de Dados**: Envolve a combinação de dados de várias fontes para uma visualização única, ou seja, padronização das entradas.
    - **Limpeza de Dados**: Trata valores faltantes, corrige erros e inconsistências nos dados.
    - **Redução de Dados**: Agrupamento e seleção de dados cruciais para a análise, incluindo compressão, redução de dimensionalidade e de numerosidade.
    - **Transformação dos Dados**: Consiste em transformar e consolidar os dados no tipo apropriado para análise e gestão. Envolve a aplicação de técnicas como agrupamento, generalização, discretização e suavização.
    - **Análise**: Aplicação de modelos para a extração de informações relevantes para o negócio.
    - **Visualização**: Consiste na apresentação dos resultados e informações extraídas do Big Data, com o uso de gráficos, dashboards e relatórios.

## 1.9 Tecnologia do Big Data

- Uma das tecnologias mais usadas para a manipulação de Big Data é o Apache Hadoop. O Hadoop possui alguns componentes principais: **HDFS** (Hadoop Distributed File System), **Hadoop Common** (uma coleção de utilitários comuns que suportam outros módulos do Hadoop), **MapReduce** e **Yarn** (Yet Another Resource Negotiator).
- Mesmo com a criação das tecnologias de Big Data, o gerenciamento desses dados ainda enfrenta vários desafios, como: incompletude dos dados, tamanho do armazenamento necessário, privacidade, variedade de tipos de dados e velocidade de processamento.

## 1.10 Aplicações do Big Data

- **Cuidados com a Saúde**: A área da saúde possui dados complexos e de crescimento rápido; a implementação de soluções de Big Data pode ajudar a analisar e processar dados de maneira rápida e com baixo custo. Alguns usos incluem:
    - Monitoramento remoto de pacientes.
    - Registros eletrônicos de saúde para otimização do diagnóstico.
    - Saúde baseada em evidências (laudos médicos, sinais biomédicos etc.).
    - Descoberta de padrões para prevenção e tratamento de doenças.
- **Telecomunicações**: Dados de tráfego de rede, chamadas e comportamento do cliente são muito importantes para as empresas. O Big Data pode ser usado como estratégia para retenção de clientes, personalização de planos e serviços, detecção de anomalias e fraudes, otimização de estratégias de marketing, previsão de desempenho de produtos etc.
- **Serviços Financeiros**: No ramo de finanças, ter informações atualizadas é crucial para a gestão de riscos. O Big Data pode promover benefícios como:
    - Insights que ajudam consultores a orientar investimentos.
    - Avaliação de crédito baseada em comportamento de compra, atividades sociais e parcerias empresariais.
    - Análise preditiva para detecção de padrões de fraudes e prevenção de fraudes em cartões de crédito em tempo real.
