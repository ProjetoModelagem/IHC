# Projeto de IHC – Automação da Geração de Relatórios Baseados em OSINT

## Membros da Equipe
- Guilherme de Abreu – 22.222.028-7  
- Kaique Fernandes – 22.221.011-4  

---

##    Entrega 1 – Conhecendo o Problema  (28-08-2025) [Concluído]

### 1.1) Membros da Equipe  
- Guilherme de Abreu – 22.222.028-7  
- Kaique Fernandes – 22.221.011-4  

### 1.2) Título Original do TCC  
Automação da Geração de Relatórios Baseados em OSINT  

### 1.3) Nome do Orientador  
** Prof. Dr. Leonardo Anjoletto Ferreira 

### 1.4) Previsto desenvolver Interface?  
(X) Sim  

### 1.5) Objetivo do trabalho  
Desenvolver uma ferramenta que automatize a coleta e análise de informações públicas (OSINT) para gerar relatórios de pentest de forma ágil, padronizada e confiável.  

### 1.6) Produto final  
Uma aplicação com interface web que realiza buscas OSINT (ex.: HaveIBeenPwned, Shodan, Google Dorks), organiza os dados e gera relatórios automatizados em PDF.  

### 1.7) Usuário final  
Pentesters, analistas de segurança da informação e empresas que desejam validar exposição de dados sensíveis.  

### 1.8) Benefício ao usuário  
- Redução do tempo de coleta manual  
- Relatórios padronizados  
- Maior precisão nas análises  
- Suporte a auditorias de conformidade (LGPD, ISO 27001, etc.)  

### 1.9) Funcionalidades (visão do usuário)  
- Inserir alvo (domínio/email/IP)  
- Executar busca OSINT  
- Visualizar resultados organizados  
- Gerar relatório automático  
- Exportar relatório em PDF  

### 1.10) Tecnologias previstas  
- Linguagem: Typescript 
- Frameworks: Vite 
- Bibliotecas: ReportLab, React, Node
- APIs: Shodan, HaveIBeenPwned, TheHarvester  

### 1.11) Contexto de uso (conceito de IHC)  
Ambiente profissional de segurança cibernética, usado em computadores conectados à internet, por especialistas de TI. Contexto de **alta concentração e criticidade**, pois os resultados impactam auditorias de segurança e decisões empresariais.  

---

## Entrega 2 – Análise de Concorrência  (28-08-2025) [Concluído]

### Versão – Autor: Kaique Fernandes  

#### Público-alvo  
Pentesters independentes, analistas de segurança de pequenas/médias empresas, consultorias que buscam automatização.  

#### Concorrentes analisados  
- **TheHarvester** – coleta de e-mails e domínios a partir de motores de busca.  
- **Holehe** – checagem de e-mails em serviços populares.  

#### Características e funcionalidades  
- **TheHarvester:** busca de e-mails, subdomínios, hosts.  
<img width="1848" height="844" alt="image" src="https://github.com/user-attachments/assets/6f3839b5-bb21-40c0-9e2c-c2781b384a40" />

- **Holehe:** verifica presença de e-mails em serviços (Netflix, Twitter, GitHub, etc.).  
<img width="855" height="313" alt="image" src="https://github.com/user-attachments/assets/d35ac0b8-fba6-4a68-a285-c8c2b431a6e5" />

#### Experiência do usuário (UX)  
- TheHarvester > simples, mas restrito a linha de comando.  
- Holehe > rápido, mas com saída técnica.  

#### Preços e modelos de negócio  
- TheHarvester: open source e gratuito.  
- Holehe: open source e gratuito.  

#### Padrões e tendências  
- Automação de consultas.  
- Exportação de relatórios automáticos.  
- Integração com APIs OSINT.  

---

### Versão – Autor: Guilherme de Abreu  

#### Público-alvo  
Empresas maiores, times internos de segurança e auditores que buscam otimizar auditorias.  

#### Concorrentes analisados  
- **PhoneInfoga** – coleta de informações sobre números de telefone. 
<img width="764" height="346" alt="image" src="https://github.com/user-attachments/assets/219ac06d-cbed-4f10-a702-0b712220b9d2" />
 
- **Maigret** – busca de perfis de usuários em centenas de sites.  
<img width="863" height="524" alt="image" src="https://github.com/user-attachments/assets/4f905727-e622-4c71-8e6e-46655e85395b" />


#### Características e funcionalidades  
- **PhoneInfoga:** metadados de números (país, operadora, possíveis registros).  
- **Maigret:** varredura massiva de nomes de usuário em redes sociais.  

#### Experiência do usuário (UX)  
- PhoneInfoga > simples, mas técnico.  
- Maigret > prático, mas saída longa e técnica.  

#### Preços e modelos de negócio  
- PhoneInfoga: open source e gratuito.  
- Maigret: open source e gratuito.  

#### Padrões e tendências  
- Integração com pipelines de segurança (CI/CD).  
- Uso de OSINT em larga escala para investigação de perfis digitais.  
- Democratização de ferramentas OSINT.  

---

## Entrega 3 – Personas, Mapa de Empatia, Contexto e Jornada (28-08-2025) [Concluído]

### Persona – Autor: Kaique Fernandes  
**Nome:** Lucas Andrade  
**Idade:** 27 anos  
**Profissão:** Analista de Pentest  
**Objetivos:** reduzir tempo de coleta manual e entregar relatórios rápidos e confiáveis.  
**Dores:** falta de padronização, retrabalho, pressão de prazos.  
**Expectativas:** interface simples, exportação rápida, relatórios profissionais.  

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/7012ec32-692b-4b5e-9142-4fc67e3988f9" />


---

### Persona – Autor: Guilherme de Abreu  
**Nome:** Marina Souza  
**Idade:** 32 anos  
**Profissão:** Gerente de Segurança da Informação  
**Objetivos:** ter relatórios claros para apresentar.  
**Dores:** perda de tempo procurando dados manuais, dificuldade em consolidar informações.  
**Expectativas:** ferramenta confiável, relatórios com linguagem executiva, métricas visuais.  

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/75428df1-a853-483c-9700-f919bbb93828" />


---

### Mapa de Empatia (Equipe)  
- **Quem pensa/sente isso? (Marina)** > preocupação com qualidade e prazos de auditoria.  
- **Quem vê isso? (Lucas)** > múltiplas ferramentas fragmentadas.  
- **Quem ouve isso? (Marina)** > gestores pedindo clareza e rapidez.  
- **Quem fala/faz isso? (Lucas)** > usa scripts, consulta várias fontes.  
- **Quem sofre essas dores? (Equipe toda)** > retrabalho, risco de erro humano.  
- **Quem ganha com isso? (Equipe e gestores)** > economia de tempo, padronização, segurança da informação.  

---

### Contexto de Uso (Equipe)  
- **Local:** escritórios de segurança, consultorias, home office.  
- **Dispositivo:** computadores/notebooks.  
- **Ambiente:** multitarefa, conectado, de alta criticidade (impacta conformidade legal).  
- **Características sociais:**  
  - Trabalho colaborativo em equipe multidisciplinar.  
  - Relacionamento direto com gestores e clientes.  
  - Necessidade de comunicação clara e objetiva.  
  - Forte cobrança por produtividade e confiabilidade.  

---

### Jornada do Usuário  

#### Antes da ferramenta  
1. Usuário inicia projeto de pentest manualmente.  
2. Pesquisa dados em múltiplas fontes e scripts isolados.  
3. Gasta muito tempo consolidando informações.  
4. Sente frustração e pressão por prazos curtos.  
5. Relatórios finais ficam inconsistentes ou pouco visuais.  

**Sentimento antes:** sobrecarga, insegurança, falta de confiança no resultado.  

---

#### Depois da ferramenta  
1. Usuário inicia projeto e insere o alvo na aplicação.  
2. Sistema realiza buscas automáticas em APIs OSINT.  
3. Resultados organizados em dashboard centralizado.  
4. Geração de relatório padronizado em PDF.  
5. Cliente recebe documento final claro e objetivo.  

**Sentimento depois:** alívio, confiança na qualidade, satisfação por entregar dentro do prazo.  
**Resultado:** objetivos alcançados > relatórios rápidos, confiáveis e com linguagem adaptada ao público-alvo.  

---


## Entrega 4 – Cenário de Análise/Problema (08/09/2025) [Concluído]

---

### Cenário 1 – Autor: Kaique Fernandes

#### 1) Cenário de Análise/Problema  
Lucas, analista de pentest, está conduzindo um projeto para um cliente do setor financeiro.  
Ele precisa coletar dados de diversas fontes abertas para identificar possíveis vazamentos.  
O processo é todo manual: cada busca exige tempo, atenção e retrabalho, pois os dados chegam em formatos diferentes.  
O prazo do cliente é curto, e Lucas sente frustração porque, mesmo dedicando horas ao processo, o relatório final fica inconsistente e sujeito a erros.  

É uma rotina cansativa e repetitiva, que compromete a produtividade e aumenta a pressão sobre o analista.  

---

#### 2) Questões de Refinamento  
- Quais fontes de dados o analista costuma utilizar no processo manual?  
- Quanto tempo médio é gasto em cada projeto antes da entrega?  
- Que tipo de inconsistências mais aparecem nos relatórios finais?  
- De que forma a pressão do prazo impacta a qualidade do resultado?  
- Qual o sentimento principal do analista durante esse processo?  

---

#### 3) Refinamento do Cenário  
Lucas, como analista de pentest, precisa lidar diariamente com prazos curtos e uma grande quantidade de dados provenientes de diferentes fontes OSINT.  
Sem padronização, ele passa horas copiando, ajustando e organizando informações que chegam em formatos distintos.  
Esse esforço manual aumenta as chances de erro, gera retrabalho e resulta em relatórios pouco consistentes, o que o deixa constantemente estressado e inseguro sobre a qualidade do trabalho entregue.  

---

### Cenário 2 – Autor: Guilherme de Abreu

#### 1) Cenário de Análise/Problema  
Marina, gerente de segurança da informação, recebe relatórios de auditorias internas e externas de sua equipe.  
O problema é que cada documento chega em um formato diferente, com linguagem técnica e pouco acessível para os executivos.  
Ela precisa revisar, interpretar e consolidar manualmente as informações para criar uma versão clara que será apresentada em reuniões estratégicas.  
Esse processo consome muito tempo e gera insegurança sobre se a mensagem transmitida reflete de fato os riscos reais da organização.  

---

#### 2) Questões de Refinamento  
- Quais tipos de relatórios Marina costuma receber da equipe?  
- Quanto tempo ela gasta para consolidar as informações em uma versão executiva?  
- Quais as maiores dificuldades na comunicação entre parte técnica e executiva?  
- O que acontece quando a mensagem não é transmitida de forma clara para a diretoria?  
- Qual é o impacto emocional em Marina ao lidar com esse processo repetitivo?  

---

#### 3) Refinamento do Cenário  
Marina, gerente de segurança da informação, enfrenta constantemente a dificuldade de transformar relatórios técnicos em documentos estratégicos claros para a diretoria.  
O esforço de interpretar termos técnicos, reorganizar dados e montar métricas visuais demanda muito tempo e gera desgaste, especialmente quando há pressão de reuniões próximas.  
Ela sente insegurança ao consolidar os relatórios, pois teme que informações críticas sejam mal comunicadas ou que o nível executivo não compreenda o real impacto dos riscos apresentados.  

---


# Entrega 5 – Análise de Tarefas (15/09/2025) [Concluída]

---

## Persona 1 – Lucas Andrade (Analista de Pentest)

### 1) HTA – Hierarchical Task Analysis

**Tarefa 0: Realizar investigação OSINT e entregar relatório técnico padronizado**

---

## Diagrama de Análise Hierárquica de Tarefas (estrutura em árvore)

> **Plano 0:** **1 > 2 > 3 > 4 > 5 > 6 > 7**  
> (Sequencial: preparar > coletar > monitorar > validar > classificar > relatar > registrar/entregar)  

<img width="2743" height="713" alt="HTA1" src="https://github.com/user-attachments/assets/169a1083-1f89-4bf8-a56c-7d08e53b611e" />


---

## Tabela — Objetivos/Operações × Problemas e Recomendações

| **Objetivos / Operações**                | **Problemas e Recomendações**                                                                                                                                                                                                       |
| ---------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **0. Realizar investigação OSINT 1 > 2 > 3 > 4 > 5 > 6 > 7**   | **Input:** solicitação e escopo.<br>**Plano:** 1>2>3>4>5>6>7.<br>**Feedback:** status geral por etapa.<br>**Recomendação:** checklist de escopo obrigatório antes de iniciar. |
| **1. Preparar alvo e contexto 1.1 > 1.2 > 1.3**      | **Plano:** **1.1 > 1.2 > 1.3** (sequencial; sem 1.1 não prossegue).                                                                                                                                                                 |
| **1.1 Verificar contrato/consentimento** |                                                                                     |
| **1.2 Definir escopo e restrições**  | **Problema:** escopo ambíguo.<br>**Recomendação:** campos estruturados (alvo, subdomínios, janelas, limites legais).                                                                                                                |
| **1.3 Selecionar fontes OSINT**          | **Problema:** fontes redundantes.<br>**Recomendação:** presets por cenário (PF/PJ) e por tipo (credenciais/infra/social/pastes).                                                                                                    |
| **2. Configurar coletas automáticas 2.1 > (2.2 + 2.3)**    | **Plano:** **2.1 > (2.2 + 2.3)** em paralelo controlado.                                                                                                                                                                            |
| **2.1 Provisionar chaves/API**           |                                                                                       |
| **2.2 Parametrizar consultas**           | **Problema:** rate limit/excesso de dados.<br>**Recomendação:** limites padrão, dicas de query e throttling/retries.                                                                                                                |
| **2.3 Agendar/Disparar varreduras**              |                                                                                           |
| **3. Monitorar execução (3.1 + 3.2 + 3.3)***                | **Plano:** **(3.1 + 3.2 + 3.3)*** — ciclo iterativo até término.                                                                                                                                                                    |
| **3.1 Acompanhar progresso**             |                                                                                     |
| **3.2 Tratar falhas**                    | **Problema:** loops de falha.<br>**Recomendação:** circuit breaker + alerta; em quota/credencial, devolver para **2.1/2.2** (reconfigurar).                                                                                         |
| **3.3 Registrar logs de execução**                   | **Problema:** logs incompletos.<br>**Recomendação:** padronizar JSON e política de retenção.                                                                                                                                        |
| **4. Validar e evidenciar achados 4.1 > 4.2 > 4.3**      | **Plano:** **4.1 > 4.2 > 4.3** (sequencial).                                                                                                                                                                                        |
| **4.1 Deduplicar/remover falsos positivos**            | **Problema:** FP elevado.<br>**Recomendação:** regras por fonte; ML simples (fase 2).                                                                                                                                               |
| **4.2 Correlacionar dados entre fontes**              | **Problema:** correlação fraca.<br>**Recomendação:** normalizar chaves (e-mail, domínio, IP, TLD).                                                                                                                                  |
| **4.3 Evidenciar**                       | **Problema:** links quebrados.<br>**Recomendação:** captura “forense” (screenshot + hash + data/hora).                                                                                                                              |
| **5. Classificar e priorizar riscos 5.1 > 5.2**    | **Plano:** **5.1 > 5.2** (sequencial).                                                                                                                                                                                              |
| **5.1 Avaliar impacto × probabilidade**          | **Problema:** critérios subjetivos.<br>**Recomendação:** tabela de avaliação padronizada.                                                                                                                                           |
| **5.2 Mapear requisitos/controles**               | **Problema:** lacunas normativas.<br>**Recomendação:** taxonomia LGPD/ISO/NIST e registro de gaps.                                                                                                                                  |
| **6. Montar relatório técnico 6.1 > 6.2 > 6.3 > 6.4**          | **Plano:** **6.1 > 6.2 > 6.3 > 6.4** (sequencial).                                                                                                                                                                                  |
| **6.1 Preencher template técnico**                 | **Problema:** variabilidade de escrita.<br>**Recomendação:** template rígido com placeholders.                                                                                                                                      |
| **6.2 Inserir KPIs/gráficos**                    | **Problema:** gráficos confusos.<br>**Recomendação:** paleta e legenda padrão.                                                                                                                                                      |
| **6.3 Revisão por pares**                | **Recomendação:** aprovação obrigatória antes de **6.4**.                                                                                                                                                                           |
| **6.4 Exportar PDF**                     | **Problema:** formatação quebrada.<br>**Recomendação:** exportador testado + QA.                                                                                                                                                    |
| **7. Entregar e arquivar 7.1 > 7.2**               | **Plano:** **7.1 > 7.2** (sequencial).                                                                                                                                                                                              |
| **7.1 Enviar ao cliente**                | **Problema:** SMTP/caixa postal.<br>**Recomendação:** envio integrado e registro.                                                                                                                                                   |
| **7.2 Registrar em histórico/KB**        | **Problema:** perda de aprendizado.<br>**Recomendação:** KB versionada + tags por alvo/fonte/severidade.                                                                                                                            |

---
# GOMS–KLM — Lucas (Analista de Pentest)
(**Plano do HTA:** 1 > 2 > 3 > 4 > 5 > 6 > 7)

#GOAL 0: Realizar investigação OSINT e entregar relatório técnico padronizado  
##GOAL 1: Preparar alvo e contexto  (HTA: 1.1 > 1.2 > 1.3)
###GOAL 1.1: Verificar contrato/consentimento  (HTA 1.1)
#### **OP 1.1.1:** [P] Abrir módulo “Escopo/Compliance”
#### **OP 1.1.2:** [K] Digitar nº do contrato/OS
#### **OP 1.1.3:** [B] Clicar em **Validar**
#### **OP 1.1.4:** [R] Aguardar retorno “Autorizado/Negado”
#### **OP 1.1.5:** [M] Confirmar que a base legal está OK

### GOAL 1.2: Definir escopo e restrições  (HTA 1.2)
#### **OP 1.2.1** [K] Inserir alvo (domínio/e-mail/IP)
#### **OP 1.2.2:** [K] Definir janelas/limites (horário, subdomínios, TLD)
#### **OP 1.2.3:** [B] **Salvar escopo**
#### **OP 1.2.4:** [R] Ver confirmação de escopo salvo

### GOAL 1.3: Selecionar fontes OSINT  (HTA 1.3)
#### **OP 1.3.1:** [P] Abrir lista de fontes
#### **OP 1.3.2:** [B] Marcar **HIBP**
#### **OP 1.3.3:** [B] Marcar **Shodan**
#### **OP 1.3.4:** [B] Marcar **Pastebin** (se aplicável)
#### **OP 1.3.5:** [M] Revisar redundâncias e confirmar

## GOAL 2: Configurar coletas automáticas  (HTA: 2.1 > (2.2 + 2.3))

###GOAL 2.1: Provisionar chaves\API  (HTA 2.1)
#### **OP 2.1.1:** [K] Digitar
#### **OP 2.1.2:** [B] Clicar em **salvar**
#### **OP 2.1.3:** [M] Confirmar os dados

### GOAL 2.2: Parametrizar consultas  (HTA 2.2)
#### METHOD 2.2.A Inserir dados 
(SEL. rule: dados baseados no alvo) 
##### **OP 2.2.A.1** [K] Inserir dados (domínio/e-mail/IP/telefone)
##### **OP 2.2.A.2:** [R] Confirmar os parametros

### GOAL 2.3: Agendar\disparar varreduras (HTA 2.3)
#### **OP 2.3.1:** [P] Mover até a posição
#### **OP 2.3.2:** [B] Clicar em **agendar**
#### **OP 2.3.3:** [B] Clicar em **disparar**

## GOAL 3: Monitorar execução  (HTA: (3.1 + 3.2 + 3.3)\*)

### GOAL 3.1: Acompanhar progresso  (HTA 3.1)
#### **OP 3.1.1:** [R] Ver lista de progresso
#### **OP 3.1.2:** [M] Conferir amostras

### GOAL 3.2: Tratar falhas  (HTA 3.2)

### GOAL 3.3: Registrar logs de execução  (HTA 3.3)

## GOAL 4: Validar e evidenciar achados  (HTA: 4.1 > 4.2 > 4.3)

### GOAL 4.1: Deduplicar/remover falsos positivos  (HTA 4.1)

### GOAL 4.2: Correlacionar dados entre fontes  (HTA 4.2)

### GOAL 4.3: Evidenciar  (HTA 4.3)

## GOAL 5: Classificar e priorizar riscos  (HTA: 5.1 > 5.2)

### GOAL 5.1: Avaliar impacto × probabilidade  (HTA 5.1)

### GOAL 5.2: Mapear a requisitos/controles  (HTA 5.2)

## GOAL 6: Montar relatório técnico  (HTA: 6.1 > 6.2 > 6.3 > 6.4)

### GOAL 6.1: Preencher template técnico  (HTA 6.1)

### GOAL 6.2: Inserir KPIs/gráficos  (HTA 6.2)

### GOAL 6.3: Revisão por pares  (HTA 6.3)

### GOAL 6.4: Exportar PDF  (HTA 6.4)
#### **OP 6.4.1:** [B] **Exportar PDF**
#### **OP 6.4.2:** [R] Conferir arquivo gerado

## GOAL 7: Entregar e arquivar  (HTA: 7.1 > 7.2)

### GOAL 7.1: Enviar ao cliente  (HTA 7.1)
#### **OP 7.1.1:** [B] Anexar PDF final
#### **OP 7.1.2:** [K] Inserir destinatários
#### **OP 7.1.3:** [B] **Enviar**
#### **OP 7.1.4:** [R] Ver confirmação de envio

### GOAL 7.2: Registrar em histórico/KB  (HTA 7.2)
#### **OP 7.2.1:** [R] Ver versão arquivada

---

### Legenda KLM
**K** (Keying) ≈ 0,2s • **P** (Pointing) ≈ 1,1s • **B** (Button) ≈ 0,1s • **H** (Homing) ≈ 0,4s • **M** (Mental) ≈ 1,2s • **R** (Response) = variável

_________________________


# ConcurTaskTree - Lucas (Executar Varredura OSINT)


<img width="16384" height="2574" alt="image" src="https://github.com/user-attachments/assets/6bdc93d0-be92-45a8-a930-24e826435219" />
<img width="1519" height="506" alt="image" src="https://github.com/user-attachments/assets/2bfc6c84-e17a-4001-9e83-20ca38ddd748" />
<img width="1626" height="416" alt="image" src="https://github.com/user-attachments/assets/a6abbe58-eca9-482c-b9ad-62ac2a995b89" />





## Persona 2 – Marina Souza (Gerente de Segurança)

#### 1) HTA – Hierarchical Task Analysis

**Tarefa 0: Consolidar relatório OSINT em versão executiva e apresentá-lo à diretoria**

---

## Diagrama de Análise Hierárquica de Tarefas (estrutura em árvore)

> **Plano 0:** **1 > 2 > 3 > 4 > 5 > 6 > 7**  
> (Sequencial: importar > selecionar métricas > redigir sumário > revisar > preparar apresentação > apresentar > arquivar)

<img width="2743" height="712" alt="HTA2" src="https://github.com/user-attachments/assets/2139e5af-5503-4b39-a1ad-045d2e2ebcc6" />


---

## Tabela — Objetivos/Operações × Input / Ação / Feedback / Problemas / Recomendações

| **Objetivos / Operações**             | **Problemas e Recomendações**                                                                                                                                                                                                    |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **0. Consolidar relatório OSINT 1>2>3>4>5>6>7** | **Input:** relatório técnico (base).<br>**Plano:** 1>2>3>4>5>6>7.<br>**Feedback:** relatório executivo gerado.<br>**Recomendação:** estrutura executiva obrigatória antes da apresentação. |
| **1. Importar achados técnicos 1.1 > 1.2**      | **Problema:** foco técnico excessivo.<br>**Recomendação:** selecionar apenas evidências e conclusões úteis ao negócio (checklist mínimo).                                                                                        |
| **1.1 Receber relatório técnico da equipe**        | **Recomendação:** usar template de entrada + checklist (escopo, achados, evidências, severidade) antes de prosseguir.                                                                                 |
| **1.2 Selecionar seções relevantes para gestores** | **Problema:** foco técnico excessivo e perda de contexto de negócio.<br>**Recomendação:** manter apenas 4 blocos: riscos prioritários, impacto (financeiro/reputacional/regulatório), evidências-chave e próximos passos; detalhes técnicos ficam em anexo. |
| **2. Sintetizar risco para negócio 2.1 + 2.2**  | **Plano:** **2.1 Definir KPIs > 2.2 Avaliar impacto** (sequencial).                                                                                                                                                              |
| **2.1 Definir KPIs de risco**         | **Problema:** indicadores irrelevantes.<br>**Recomendação:** usar lista pré-aprovada de KPIs (frequência, severidade, exposição).                                                                                                |
| **2.2 Avaliar impacto no negócio**    | **Problema:** falta de contexto (financeiro/reputacional/regulatório).<br>**Recomendação:** validar com compliance/owner do processo antes de fechar o impacto.                                                                  |
| **3. Redigir sumário executivo 3.1 > 3.2**       | **Plano:** **3.1 Estruturar tópicos > 3.2 Adaptar vocabulário**.                                                                                                                                                                 |
| **3.1 Estruturar tópicos principais**            |                                                                                                      |
| **3.2 Adaptar vocabulário para linguagem nao técnica**           | **Problema:** jargão técnico.<br>**Recomendação:** linguagem executiva; evitar termos internos sem explicação.                                                                                                                   |
| **4. Revisar linguagem e clareza 4.1 > 4.2**                | **Plano:** **4.1 Eliminar jargão > 4.2 Validar clareza**.                                                                                                                                                                        |
| **4.1 Eliminar jargão técnico**               | **Recomendação:** manter glossário simples quando inevitável.                                                                                                                                                                    |
| **4.2 Validar clareza com equipe**               | **Problema:** desalinhamento de expectativa.<br>**Recomendação:** revisão cruzada por duas funções (ex.: Segurança + Produto).                                                                                                   |
| **5. Produzir material visual 5.1 + 5.2**       | **Plano:** **5.1 Criar slides + 5.2 Inserir gráficos**.                                                                                                                                                                          |
| **5.1 Criar slides**                  | **Problema:** slides poluídos.<br>**Recomendação:** modelo corporativo e regra “1 ideia por slide”.                                                                                                                              |
| **5.2 Inserir gráficos**              | **Problema:** gráficos confusos.<br>**Recomendação:** paleta oficial e rótulos/legendas padronizados.                                                                                                                            |
| **6. Apresentar à diretoria 6.1 > 6.2**         | **Plano:** **6.1 Expor sumário executivo > 6.2 Responder dúvidas**.                                                                                                                                                              |
| **6.1 Expor sumário executivo**       | **Problema:** tempo curto.<br>**Recomendação:** pitch de 3–5 minutos + anexo técnico.                                                                                                                                            |
| **6.2 Responder dúvidas e coletar feedbacks**             | **Recomendação:** sessão de Q&A com respostas já roteirizadas; registrar perguntas para ajustes.                                                                                                                                 |
| **7. Arquivar e registrar 7.1 > 7.2**      | **Plano:** **7.1 Salvar versão final > 7.2 Indexar histórico**.                                                                                                                                                                  |
| **7.1 Salvar versão final**           | **Problema:** perda de versão.<br>**Recomendação:** versionamento controlado e registro de aprovações.                                                                                                                           |
| **7.2 Indexar histórico/KB**          | **Problema:** baixa encontrabilidade depois.<br>**Recomendação:** indexação padronizada (tags por alvo, fonte, severidade, data).                                                                                                |

---

# GOMS–KLM — Marina (Gerente de Segurança)

**Goal 0:** Consolidar relatório OSINT em versão executiva para diretoria  
(**Plano do HTA:** 1 > 2 > 3 > 4 > 5 > 6 > 7)

---


# GOMS–KLM — Marina (Gerente de Segurança)

**Goal 0:** Consolidar relatório OSINT em versão executiva para diretoria  
(**Plano do HTA:** 1 > 2 > 3 > 4 > 5 > 6 > 7)

---

## GOAL 1: Importar achados técnicos (HTA 1.1 > 1.2)

###GOAL 1.1: Receber relatório técnico da equipe (HTA 1.1)
- **OP 1.1.1:** [P] Abrir e acessar pasta/drive da equipe  
- **OP 1.1.2:** [B] Clicar no relatório técnico mais recente  
- **OP 1.1.3:** [R] Aguardar carregamento do arquivo  
- **OP 1.1.4:** [M] Verificar checklist (escopo, achados, evidências, severidade)  


### GOAL 1.2: Selecionar seções relevantes para gestores (HTA 1.2)   
### METHOD 1.2.A: Seleção das seções
(SEL. RULE: manter apenas riscos prioritários, impactos, evidências-chave e próximos passos)  
- **OP 1.2.A.1:** [P] Navegar pelas seções do relatório  
- **OP 1.2.A.2:** [B] Destacar blocos importantes (riscos, impacto, evidências)  
- **OP 1.2.A.3:** [M] Validar se conteúdo é relevante para gestores  
- **OP 1.2.A.4:** [R] Conferir versão reduzida com apenas seções relevantes  


---

## GOAL 2: Sintetizar risco para negócio (HTA 2.1 > 2.2)

### GOAL 2.1: Definir KPIs de risco (HTA 2.1)
- **OP 2.1.1:** [P] Selecionar lista de KPIs pré-aprovados  
- **OP 2.1.2:** [B] Marcar indicadores aplicáveis (frequência, severidade, exposição)  
- **OP 2.1.3:** [M] Conferir se todos são relevantes  

### GOAL 2.2: Avaliar impacto no negócio (HTA 2.2)
METHOD 2.2.A: Inserir impacto para avaliação
(SEL. RULE: se há falta de contexto → validar com compliance/owner antes de fechar impacto)  
- **OP 2.2.A.1:** [K] Inserir impacto financeiro/reputacional/regulatório  
- **OP 2.2.A.2:** [M] Comparar com casos semelhantes já registrados  
- **OP 2.2.A.3:** [R] Ver confirmação do sistema ou feedback da área consultada  

---

## GOAL 3: Redigir sumário executivo (HTA 3.1 > 3.2)

### GOAL 3.1: Estruturar tópicos principais (HTA 3.1)
- **OP 3.1.1:** [K] Escrever tópicos principais em bullets curtos  
- **OP 3.1.2:** [M] Organizar em ordem de criticidade (alto > médio > baixo)  

### GOAL 3.2: Adaptar vocabulário para linguagem não técnica
- **OP 3.2.1:** [K] Reescrever trechos técnicos em linguagem de negócio  
- **OP 3.2.2:** [M] Validar clareza e evitar termos internos sem explicação  

---

## GOAL 4: Revisar linguagem e clareza (HTA 4.1 > 4.2)

### GOAL 4.1: Eliminar jargão técnico (HTA 4.1)
- **OP 4.1.1:** [K] Editar texto removendo termos técnicos  
- **OP 4.1.2:** [M] Substituir por expressões simples ou glossário  


### GOAL 4.2: Validar clareza com equipe (HTA 4.2)
- **OP 4.2.1:** [P] Enviar sumário para colega (Segurança/Produto)  
- **OP 4.2.2:** [R] Aguardar feedback  
- **OP 4.2.3:** [M] Ajustar conforme sugestões  

---

## GOAL 5: Produzir material visual (HTA 5.1 + 5.2)

### GOAL 5.1: Criar slides
- **OP 5.1.1:** [P] Abrir modelo corporativo  
- **OP 5.1.2:** [K] Inserir tópicos resumidos  
- **OP 5.1.3:** [M] Validar regra “1 ideia por slide”  

### GOAL 5.2: Inserir gráficos (HTA 5.2)
- **OP 5.2.1:** [B] Selecionar dados no relatório  
- **OP 5.2.2:** [B] Clicar em “Gerar gráfico”  
- **OP 5.2.3:** [R] Ver renderização do gráfico  
- **OP 5.2.4:** [M] Ajustar rótulos/legenda, se confuso  

---

## GOAL 6: Apresentar à diretoria (HTA 6.1 > 6.2)

### GOAL 6.1: Expor sumário executivo (HTA 6.1)
- **OP 6.1.1:** [M] Preparar pitch de 3–5 min  
- **OP 6.1.2:** [P] Abrir slides  
- **OP 6.1.3:** [B] Passar os slides durante apresentação  

### GOAL 6.2: Responder dúvidas e coletar feedback (6.2)
### METHOD 6.2.A: Responder dúvidas (HTA 6.2)  
(SEL. RULE: se pergunta não estiver no roteiro → registrar para resposta posterior)  
- **OP 6.2.1:** [M] Responder com linguagem executiva  
- **OP 6.2.2:** [K] Anotar feedbacks e perguntas  
- **OP 6.2.3:** [R] Confirmar aceitação da resposta pela diretoria  

---

## GOAL 7: Arquivar e registrar (HTA 7.1 > 7.2)

### GOAL 7.1: Salvar versão final aprovada (HTA 7.1)
- **OP 7.1.1:** [B] Salvar documento em drive/versionador  
- **OP 7.1.2:** [K] Inserir nº da versão e data  
- **OP 7.1.3:** [R] Ver confirmação de salvamento  

### GOAL 7.2: Indexar em histórico/ KB corporativo (HTA 7.2)
### METHOD 7.2.A: Adicionar tags baseado na reunião de apresentação
- **OP 7.2.A.1:** [K] Adicionar tags (alvo, fonte, severidade, data)  
- **OP 7.2.A.2:** [B] Publicar no repositório/KB  
- **OP 7.2.A.3:** [R] Conferir indexação concluída  

---

______________

# ConcurTaskTree - Marina (Consolidar Relatório Executivo)

<img width="16384" height="2574" alt="image" src="https://github.com/user-attachments/assets/c797180e-9e98-4085-9a1a-3108d61ac321" />
<img width="1519" height="506" alt="image" src="https://github.com/user-attachments/assets/2bfc6c84-e17a-4001-9e83-20ca38ddd748" />
<img width="1626" height="416" alt="image" src="https://github.com/user-attachments/assets/a6abbe58-eca9-482c-b9ad-62ac2a995b89" />


_________________


## Entrega 6 - 22/09/2025 [Concluído]

### Protótipo em Papel
![Untitled](https://github.com/user-attachments/assets/9f73aff4-fa1a-40ab-985a-1e2d0d4736e1)
![Untitled-1](https://github.com/user-attachments/assets/858d02ad-ec0d-41ce-b54c-329ce7fd9cc7)
![Untitled-1](https://github.com/user-attachments/assets/05746f75-d183-402a-9a70-37abae3162f0)

---

## Entrega 7 - Identificação de Necessidades, Ética e Ferramentas de Coleta - 25/09/2025 [Concluído]

## 1) Necessidades dos Usuários e Requisitos de IHC

### Que dados coletar
- **Perfil:** cargo, tempo de experiência, onde trabalha (empresa, home office), nível de conhecimento em segurança.
- **Uso de tecnologia:** quais ferramentas de coleta de informações já utiliza, quais tem mais dificuldade, como é o ambiente de trabalho (tamanho de tela, internet).
- **Tarefas:** como faz a coleta de dados hoje, etapas mais demoradas, pontos onde costuma ter erro ou retrabalho.
- **Informações desejadas:** tipos de gráficos e indicadores mais importantes no relatório final.
- **Motivações e dificuldades:** pressão de prazo, necessidade de relatórios prontos e padronizados.

### De quem coletar
- **Usuários principais:** analistas de segurança (como Lucas) e gestores de segurança (como Marina).
- **Outros envolvidos:** pessoas de compliance/privacidade e gestores de TI que vão receber os relatórios.

---

## 2) Aspectos Éticos

- **Consentimento:** antes de entrevistas ou questionários, explicar o objetivo, tempo de participação, e garantir que a pessoa pode desistir quando quiser.
- **Privacidade e LGPD:** só pedir dados realmente necessários; não guardar informações sensíveis ou credenciais reais; anonimizar as respostas para que não seja possível identificar quem respondeu.
- **Princípios importantes:**
  - **Evitar dano:** cuidar para que nenhuma informação seja usada de forma indevida.
  - **Benefício:** os dados coletados devem trazer melhorias para o sistema.
  - **Autonomia:** cada participante decide se quer ou não participar.
  - **Justiça:** tratar todos de forma igual, sem sobrecarregar ninguém.
- **No contexto OSINT:** sempre usar dados de teste ou ambientes autorizados, com escopo de coleta bem definido.

---

## 3) Ferramentas de Coleta de Dados

### 3.1 Questionário
- **Objetivo:** confirmar em mais pessoas quais são as maiores necessidades e problemas.
- **Como aplicar:** formulário on-line (por exemplo Google Forms) com perguntas simples de múltipla escolha e algumas abertas; tempo de resposta de 5 a 8 minutos.
- **Exemplo de perguntas:** cargo e tempo de experiência, ferramentas que usa, grau de dificuldade em cada etapa (escala de 1 a 5), quais indicadores são mais importantes no relatório.
- **Link:** https://docs.google.com/forms/d/e/1FAIpQLSdCkHZEQvKec9_t_PKqCh25AAAMZiIz3A1WhI2Ic2zsrxIIPw/viewform?usp=dialog

### 3.2 Observação do trabalho
- **Objetivo:** ver como o analista realmente trabalha no dia a dia para descobrir detalhes que não aparecem em entrevistas.
- **Como aplicar:** acompanhar a pessoa durante cerca de 1 hora enquanto ela faz uma investigação de teste; anotar etapas, erros e tempo gasto, pedindo sempre consentimento.



# Entrega 8 – Características, Princípios e Metas

## 1) Características da Plataforma

- **Descrição do Software:**  
  Aplicação web chamada *Was I Hacked?*, desenvolvida em arquitetura cliente-servidor.  
  O sistema coleta dados de fontes OSINT, organiza os achados em dashboards  
  e gera relatórios técnicos e executivos em PDF/PPT.  

- **Descrição do Hardware:**  
  Requisitos mínimos:  
  - Cliente: notebook/PC com navegador atualizado, tela mínima de 14’’, 4GB RAM.  
  - Servidor: máquina virtual com 4 vCPUs, 8GB RAM, 100GB de armazenamento, conexão estável à internet.  

- **Lista de Capacidades da Plataforma (com explicação):**  
  - **Coleta automatizada em APIs OSINT:** reduz o tempo manual do analista.  
  - **Validação e deduplicação de achados:** garante consistência dos dados.  
  - **Classificação de riscos:** prioriza informações para tomada de decisão.  
  - **Geração de relatórios técnicos:** detalhamento com evidências.  
  - **Geração de relatórios executivos:** resumo com KPIs e gráficos para gestores.  
  - **Exportação em PDF/PPT:** facilita a apresentação e compartilhamento.  

- **Lista de Restrições da Plataforma (com explicação):**  
  - **Dependência de fontes externas (APIs OSINT):** se a API estiver fora do ar, a coleta falha.  
  - **Conexão com internet obrigatória:** não há uso offline.  
  - **Limite de performance em consultas massivas:** coletas muito extensas podem ser lentas.  
  - **Uso apenas com dados autorizados:** não pode ser aplicado em alvos reais sem permissão (ética e legalidade).  

---

## 2) Princípios Gerais do Projeto

| Princípio | Justificativa |
|-----------|---------------|
| **LGPD e Privacidade** | O sistema não armazena dados pessoais sem consentimento e usa apenas informações autorizadas para testes. |
| **Acessibilidade (WCAG)** | Interfaces simples, contraste adequado e elementos claros para usuários com diferentes níveis de experiência. |
| **Usabilidade (ISO 9241)** | Garantir que usuários (analistas e gestores) completem tarefas com eficácia e sem retrabalho. |
| **Segurança da Informação** | Dados coletados ficam restritos, sem exposição pública, respeitando confidencialidade. |

---

## 3) Metas de Usabilidade

- **Qualitativas:**  
  - Usuários devem considerar o sistema fácil de aprender em menos de 30 minutos de uso.  
  - O relatório executivo deve ser compreendido por gestores sem conhecimento técnico.  
  - A interface deve reduzir a necessidade de retrabalho e duplicação de dados.  

- **Quantitativas:**  



---

## Entrega 9 - 13/10/2025 [Em andamento]

### 1) Cenários de Interação
(Narrar como seria a interação na solução. Destacar diferenças em relação ao cenário problema.)

### 2) Design Centrado na Comunicação
(Representar falas e signos em formato de diálogo U/D.)

### 3) Mapa de Objetivos
(Colocar diagramas individuais e um consolidado.)

### 4) Esquema Conceitual de Signos
(Tabela com signos, origem, conteúdo, restrições, prevenção e recuperação.)

---

## Entrega 10 - 20/10/2025 [Em andamento]

### MOLIC
- *Nome do Cenário:*  
- *Diagrama:*  

---

## Entrega 11 - 27/10/2025 [Em andamento]

### Protótipo Correspondente ao MOLIC
- *Link para o Figma:*  

---

## Entrega 12 - 03/11/2025 [Em andamento]

### a) Planejamento de Usabilidade (Método DECIDE)
- *D:*  
- *E:*  
- *C:*  
- *I:*  
- *D:*  
- *E:*  

### b) Lista de Instrumentos
- Termo de consentimento  
- Questionários  
- Tabela de Observação  
- Formulário de avaliação heurística  

---

## Entrega 13 - 10/11/2025 [Em andamento]

### A) Avaliação de IHC através de inspeção HEURÍSTICA
(Para cada tela, listar violações de heurísticas de Nielsen com severidade 0 a 4.)

### B) Indicação de Boas Práticas de Heurística
(Um exemplo do sistema onde a heurística foi atendida.)

---

## Entrega 14 - 17/11/2025 [Em andamento]

### A) Fluxograma de Avaliação de Usabilidade por Observação do Usuário
(Fluxo de como o teste será aplicado.)

### B) Descrição do Procedimento de Preparação do Teste
- Passo 1: ...  
- Passo 2: Lista de tarefas  
- Passo 3: Formulário de perfil do usuário  
- etc.  

### C) Resultados do Teste
Tabela:  
- Grau de sucesso  
- Erros cometidos  
- Tipos de erros  
- Tempo necessário  
- Grau de satisfação  

- *Links dos vídeos:*  
- *Respostas dos formulários:*  
- *Conclusão da avaliação por observação do usuário:*  

---
