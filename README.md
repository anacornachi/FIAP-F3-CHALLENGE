# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Nome do projeto
Enterprise Challenge - Solução para a Hermes Reply - Plataforma inteligente de manutenção preditiva

## Nome do grupo

## 👨‍🎓 Integrantes:

- <a href="https://www.linkedin.com/in/anacornachi/">Ana Cornachi</a>
- <a href="https://www.linkedin.com/in/carlamaximo/">Carla Máximo</a>
- <a href="https://www.linkedin.com/in/lucas-lins-lima/">Lucas Lins</a>

## 👩‍🏫 Professores:

### Tutor(a)

- <a href="https://www.linkedin.com/in/lucas-gomes-moreira-15a8452a/">Lucas Gomes Moreira</a>

### Coordenador(a)

- <a href="https://www.linkedin.com/in/andregodoichiovato/">André Godoi Chiovato</a>

## Justificativa do Problema & Descrição da Solução

**Problema**

Interrupções inesperadas em linhas de produção industrial causam perdas financeiras e operacionais significativas. A baixa previsibilidade e reação tardia a falhas em máquinas elevam custos de manutenção corretiva, reduzem a eficiência e impactam a produtividade.

**Solução Proposta**

Desenvolver uma </b>plataforma inteligente de manutenção preditiva</b>. Essa plataforma irá monitorar equipamentos em tempo real, detectar anomalias operacionais, prever falhas de máquinas antes que elas ocorram e sugerir ações preventivas por meio de </b>dashboards intuitivos e relatórios automáticos</b>. Tudo isso baseado em algoritmos avançados de Inteligência Artificial (Machine Learning) e integrando sensores via IoT.

## Definição das Tecnologias

| FINALIDADE | TECNOLOGIA PROPOSTA | JUSTIFICATIVA |
| ------------- | ------------- | ------------- |
| Programação/Análise de Dados/IA | Python, Pandas, Scikit-learn, TensorFlow, Keras, R | Python é referência para dados e IA; Pandas/Scikit-learn para preprocessamento e modelos tradicionais; TensorFlow/Keras para Deep Learning; R para análises extras |
| Coleta dos Dados (IoT) | ESP32, MQTT | ESP32 é acessível para prototipagem e facilita o envio de dados via MQTT (padrão de mercado para IoT) |
| Armazenamento de Dados | PostgreSQL/AWS RDS, arquivos CSV, Amazon S3 | PostgreSQL/AWS RDS é robusto e escalável; S3 atende ao armazenamento de arquivos brutos; CSVs usados nos estágios iniciais |
| Processamento e Integração | AWS EC2 (ou Azure VM), scripts Python, APIs Flask/FastAPI | EC2/Azure para processamento escalável na nuvem; Flask/FastAPI para criação de APIs simples e integráveis |
| Visualização/Relatórios | Power BI, Tableau, Dash (Plotly), Streamlit | Dashboards interativos e relatórios automatizados para visualização clara e tomada de decisão rápida |
| Notificações / Alertas | AWS SNS (Simple Notification Service), E-mail, SMS, Teams/Slack | AWS SNS permite envio automatizado e escalável de alertas em múltiplos canais |
| Gestão e Versionamento do Projeto | GitHub, README estruturado | Colaboração e versionamento do código/documentação |

## Pipeline de Dados & Arquitetura da Solução

**Esboço do Pipeline**
1. Coleta dos Dados
   - Dados gerados por sensores (protótipo: ESP32), simulados usando arquivos CSV recebidos.
   - Envio dos dados via MQTT para um broker central.
2. Ingestão & Armazenamento
   - Recepção via API (Flask/FastAPI).
   - Armazenamento inicial em banco de dados relacional (PostgreSQL na nuvem/local).
   - Armazenamento dos arquivos brutos em Amazon S3.
3. Processamento & Pré-processamento
   - Limpeza e engenharia de atributos com Python (Pandas).
   - Pipeline automatizada para preparação dos dados.
4. Análise & Modelagem Preditiva
   - Desenvolvimento e treinamento de modelos de Machine Learning (Scikit-learn, Keras, TensorFlow, R).
   - Geração de modelos para detecção de anomalias, classificação de falhas, predição de vida útil e manutenção preditiva.
5. Visualização & Alertas
   - Dashboards responsivos (Dash, Power BI, Tableau) com insights em tempo real.
   - Alertas automáticos enviados (e-mail, SMS, integrações) para os responsáveis.
6. Recomendações & Relatórios
   - Relatórios detalhados com recomendações de manutenção.
   - APIs para geração e consulta dos relatórios personalizados.

## Justificativa do Banco de Dados em Nuvem
- **Escalabilidade:** Solução preparada para crescimento, com mais sensores e mais linhas de produção.
- **Resiliência e Backup:** Dados protegidos em casos de falhas locais.
- **Facilidade de Integração:** Serviços nativos da AWS/Azure facilitam o uso de Machine Learning e notificações.
- **Custo-Benefício:** Escalabilidade de recursos conforme a demanda real.

## Modelo da Arquitetura  

![Arquitetura_Hermes Reply drawio](https://github.com/user-attachments/assets/c59678c0-1853-4614-9674-1d1c5c5c30f8)

## Estratégia de Coleta de Dados
- Etapa inicial: Utilização de arquivos CSV simulando a coleta dos sensores reais.
- Etapas seguintes: Integração com sensores ESP32 para coleta de dados em tempo real (prototipagem).
- Envio dos dados via MQTT simulando o fluxo dos eventos sensoriais para a API de ingestão.

## Plano Inicial de Desenvolvimento e Divisão de Responsabilidades

| ÁREA | RESPONSÁVEL | RESPONSABILIDADE |
| ------------- | ------------- | ------------- |
| Coleta & Simulação de Dados | Ana | Prototipar dados com ESP32/CSV, simular envio via MQTT |
| Ingestão & Armazenamento | Carla | Desenvolvimento da API, modelagem do banco de dados e integração com S3/RDS |
| Pipeline de Dados & Pré-processo | Lucas | Scripts de processamento, análise inicial dos dados |
| Modelos de IA | Ana | Construção, treinamento e teste dos modelos preditivos |
| Dashboards & Visualização | Carla | Desenvolvimento de dashboards e relatório automáticos |
| Alertas & Notificações | Lucas | Configuração de alertas automáticos e integrações com SNS/E-mail/SMS |
| Documentação & GitHub | Todos | README, documentação técnica, organização das entregas e versionamento |

## Referências

**Link Úteis**

- www.reply.com
- aws.amazon.com
- azure.microsoft.com
- app.diagrams.net
- streamlit.io
- dash.plotly.com

## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>.github</b>: Nesta pasta ficarão os arquivos de configuração específicos do GitHub que ajudam a gerenciar e automatizar processos no repositório.

- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens.

- <b>config</b>: Posicione aqui arquivos de configuração que são usados para definir parâmetros e ajustes do projeto.

- <b>document</b>: aqui estão todos os documentos do projeto que as atividades poderão pedir. Na subpasta "other", adicione documentos complementares e menos importantes.

- <b>scripts</b>: Posicione aqui scripts auxiliares para tarefas específicas do seu projeto. Exemplo: deploy, migrações de banco de dados, backups.

- <b>src</b>: Todo o código fonte criado para o desenvolvimento do projeto ao longo das 7 fases.

- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🔧 Como executar o código

_Não existem scripts para serem executados neste repositório_

## 🗃 Histórico de lançamentos

* 0.1.0 - 26/04/2025
* 0.2.0 - 05/05/2025
* 0.3.0 - 07/05/2025

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
