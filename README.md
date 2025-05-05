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

</b>Problema</b>
Interrupções inesperadas em linhas de produção industrial causam perdas financeiras e operacionais significativas. A baixa previsibilidade e reação tardia a falhas em máquinas elevam custos de manutenção corretiva, reduzem a eficiência e impactam a produtividade.

</b>Solução Proposta</b>
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

_Acrescentar as informações necessárias sobre pré-requisitos (IDEs, serviços, bibliotecas etc.) e instalação básica do projeto, descrevendo eventuais versões utilizadas. Colocar um passo a passo de como o leitor pode baixar o seu código e executá-lo a partir de sua máquina ou seu repositório. Considere a explicação organizada em fase._

## 🗃 Histórico de lançamentos

- ## 0.1.0 - 05/05/2025

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
