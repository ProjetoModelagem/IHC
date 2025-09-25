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
- TheHarvester → simples, mas restrito a linha de comando.  
- Holehe → rápido, mas com saída técnica.  

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
- PhoneInfoga → simples, mas técnico.  
- Maigret → prático, mas saída longa e técnica.  

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
- **Quem pensa/sente isso? (Marina)** → preocupação com qualidade e prazos de auditoria.  
- **Quem vê isso? (Lucas)** → múltiplas ferramentas fragmentadas.  
- **Quem ouve isso? (Marina)** → gestores pedindo clareza e rapidez.  
- **Quem fala/faz isso? (Lucas)** → usa scripts, consulta várias fontes.  
- **Quem sofre essas dores? (Equipe toda)** → retrabalho, risco de erro humano.  
- **Quem ganha com isso? (Equipe e gestores)** → economia de tempo, padronização, segurança da informação.  

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
**Resultado:** objetivos alcançados → relatórios rápidos, confiáveis e com linguagem adaptada ao público-alvo.  

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
> (Sequencial: preparar → coletar → monitorar → validar → classificar → relatar → registrar/entregar)  
> **Exceções/seleções/paralelos** detalhados nos planos locais abaixo.

**0. Realizar investigação OSINT**  
- **1. Preparar alvo e contexto**  
  - **1.1 Verificar contrato/consentimento**  
  - **1.2 Definir escopo e restrições** (alvo, limites legais, janela de execução)  
  - **1.3 Selecionar fontes OSINT** (por tipo: credenciais, infra, mídia social, pastes)  
  - **Plano 1:** **1.1 > 1.2 > 1.3** (sequencial; sem 1.1 não prossegue)  
- **2. Configurar coletas automáticas**  
  - **2.1 Provisionar chaves/API** (HIBP, Shodan, etc.)  
  - **2.2 Parametrizar consultas** (queries, throttling, retries)  
  - **2.3 Agendar/Disparar varreduras**  
  - **Plano 2:** **2.1 > (2.2 + 2.3)** (2.2 e 2.3 em **paralelo controlado**)  
- **3. Monitorar execução**  
  - **3.1 Acompanhar progresso** (status por fonte)  
  - **3.2 Tratar falhas** (timeout, quota, credencial inválida)  
  - **3.3 Registrar logs de execução**  
  - **Plano 3:** **(3.1 + 3.2 + 3.3)\*** (ciclo **paralelo/iterativo** até término)  
- **4. Validar e evidenciar achados**  
  - **4.1 Deduplicar e remover falsos positivos**  
  - **4.2 Correlacionar dados entre fontes**  
  - **4.3 Evidenciar** (screenshots, hashes, URLs, timestamps)  
  - **Plano 4:** **4.1 > 4.2 > 4.3** (sequencial)  
- **5. Classificar e priorizar riscos**  
  - **5.1 Avaliar impacto x probabilidade** (matriz)  
  - **5.2 Mapear a requisitos/controles** (LGPD/ISO/NIST conforme escopo)  
  - **Plano 5:** **5.1 > 5.2** (sequencial)  
- **6. Montar relatório técnico**  
  - **6.1 Preencher template técnico** (achado, evidência, risco, recomendação)  
  - **6.2 Inserir gráficos/KPIs** (por severidade, fonte, tempo)  
  - **6.3 Revisão por pares**  
  - **6.4 Exportar PDF**  
  - **Plano 6:** **6.1 > 6.2 > 6.3 > 6.4** (sequencial)  
- **7. Entregar e arquivar**  
  - **7.1 Enviar ao cliente**  
  - **7.2 Registrar em histórico/KB** (para reuso, métricas)  
  - **Plano 7:** **7.1 > 7.2** (sequencial)

**Regras de Seleção (globais):**  
- Se **prazo < 24h** → priorizar fontes de **alta cobertura/baixo tempo de resposta** e suspender fontes lentas (**seleção 2/3 de fontes**).  
- Se **falha crítica** numa fonte essencial → **3.2** aciona **retry** até N tentativas; se exceder, **seleciona alternativa** (outro provedor).  
- Se **falsos positivos > limiar** → reforçar **4.1** (deduplicação) antes de seguir para **4.2**.

---

## Tabela — Objetivos/Operações × Input / Ação / Feedback / Problemas / Recomendações

| **Objetivos / Operações** | **Input** | **Ação** | **Feedback** | **Problemas** | **Recomendações** |
|---|---|---|---|---|---|
| **0. Realizar investigação OSINT** | Solicitação + escopo | Executar Plano 0 | Status geral por etapa | Escopo incompleto | Checklist de escopo obrigatório |
| **1. Preparar alvo e contexto** | Contrato, alvo | Confirmar base legal e limites | OK p/ prosseguir ou bloqueio | Falta de consentimento | Gate de compliance que impede 2 sem 1.1 |
| **1.1 Verificar contrato/consentimento** | Documento/ordem serviço | Validar autorização | “Autorizado/Negado” | Documento ausente/expirado | Upload obrigatório + validade |
| **1.2 Definir escopo e restrições** | Alvo, janelas | Registrar limites técnicos/legais | Escopo salvo | Escopo ambíguo | Campos estruturados (alvo, subdomínios, etc.) |
| **1.3 Selecionar fontes OSINT** | Catálogo de fontes | Marcar fontes por tipo | Lista de fontes ativa | Fontes redundantes | Presets por cenário (PF/ PJ) |
| **2.1 Provisionar chaves/API** | Credenciais | Inserir/validar | “Chave válida” | Quota/credencial inválida | Teste automático de conexão |
| **2.2 Parametrizar consultas** | Queries, limites | Configurar filtros/throttle | Preview de consulta | Rate limit/excesso dados | Limites padrão + dicas de query |
| **2.3 Disparar varreduras** | Fontes ativas | Start/coleta | Barra de progresso | Timeouts intermitentes | Retry exponencial + fallback |
| **3.1 Acompanhar progresso** | Status por fonte | Monitorar | Percentual/ETA | Falta de visibilidade | Log detalhado por fonte |
| **3.2 Tratar falhas** | Erros | Retry/alternativa | “Recuperado” | Loop infinito de falha | Circuit breaker + alerta |
| **3.3 Registrar logs** | Eventos | Persistir logs | Log consultável | Logs incompletos | Padronizar JSON + retenção |
| **4.1 Deduplicar/remover FP** | Achados brutos | Regras/heurística | Lista limpa | FP elevado | Regras por fonte + ML simples (fase 2) |
| **4.2 Correlacionar dados** | Lista limpa | Correlacionar por chaves | Itens correlatos | Correlação pobre | Normalizar campos (email, domínios) |
| **4.3 Evidenciar** | Itens finais | Coletar provas | Evidências anexas | Links quebrados | Capturas “forenses” (hash, data/hora) |
| **5.1 Impacto × probabilidade** | Achados validados | Classificar severidade | Risco por item | Critérios subjetivos | Tabela de avaliação padronizada |
| **5.2 Mapear a controles** | Risco por item | Relacionar a normas | Mapeamento exibido | Lacunas normativas | Taxonomia (LGPD/ISO/NIST) |
| **6.1 Template técnico** | Itens classificados | Preencher seções | Prévia do relatório | Variabilidade de escrita | Template rígido c/ placeholders |
| **6.2 KPIs/gráficos** | Métricas | Inserir visualizações | KPIs renderizados | Gráfico confuso | Paleta/legenda padrão |
| **6.3 Revisão por pares** | Draft | Peer review | Comentários | Falta de revisão | Aprovação obrigatória antes de 6.4 |
| **6.4 Exportar PDF** | Documento aprovado | Exportar | PDF gerado | Erros de formatação | Exportador testado + QA |
| **7.1 Enviar ao cliente** | PDF final | Enviar | Confirmação envio | Caixa de e-mail/SMTP | Envio integrado + registro |
| **7.2 Registrar em KB** | Artefatos | Arquivar/Indexar | Versão arquivada | Perda de histórico | Nomeação e versionamento padrão |

---

## Observações didáticas
- **HTA ≠ fluxograma**: usamos **objetivos/subobjetivos/operações numerados** e **PLANOS** para a ordem (**1>2**), seleção (**1/2**) e paralelo (**1+2**).  
- **Decisões** aparecem nos **planos** (ex.: priorizar fontes sob prazo curto).  
- **Tabela** cobre **Input/Ação/Feedback** (estado final), com **Problemas/Recomendações** — como no modelo exigido pelo professor.



# GOMS-KLM — Lucas (Analista de Pentest)

**Goal 0:** Produzir relatório OSINT técnico confiável

---

## Goal 1: Preparar alvo e fontes
### Method 1.A: Definir escopo e restrições
- OP 1.A.1: [K] Digitar identificação do cliente no campo do sistema  
- OP 1.A.2: [K] Digitar o domínio alvo (ex.: empresa.com)  
- OP 1.A.3: [P] Mover cursor até checkbox "Limites legais"  
- OP 1.A.4: [B] Clicar em confirmar escopo  
- OP 1.A.5: [R] Esperar feedback do sistema sobre validação do escopo  
- **Selection Rule:** Se o escopo não for validado → voltar para OP 1.A.2

### Method 1.B: Selecionar fontes OSINT
- OP 1.B.1: [P] Mover cursor até lista de fontes  
- OP 1.B.2: [B] Marcar checkbox de “HaveIBeenPwned”  
- OP 1.B.3: [B] Marcar checkbox de “Shodan”  
- OP 1.B.4: [B] Marcar checkbox de “Pastebin”  
- OP 1.B.5: [M] Pensar e revisar se todas as fontes são adequadas  
- **Selection Rule:** Se prazo < 24h → selecionar apenas fontes de alta cobertura (pular OP 1.B.3 e OP 1.B.4)

---

## Goal 2: Executar coleta
### Method 2.A: Configurar APIs e parâmetros
- OP 2.A.1: [K] Digitar chave da API HIBP no campo de credenciais  
- OP 2.A.2: [B] Pressionar botão "Validar chave"  
- OP 2.A.3: [R] Aguardar retorno do sistema  
- OP 2.A.4: [M] Preparar query para pesquisa  
- OP 2.A.5: [K] Digitar query (e.g. “email:alvo@dominio.com”)  
- OP 2.A.6: [P] Mover cursor até botão "Salvar parâmetros"  
- OP 2.A.7: [B] Clicar no botão  
- **Selection Rule:** Se a API não validar → repetir OP 2.A.1 com nova chave

### Method 2.B: Disparar varredura
- OP 2.B.1: [P] Mover cursor até botão "Iniciar varredura"  
- OP 2.B.2: [B] Clicar botão  
- OP 2.B.3: [R] Aguardar barra de progresso carregar  
- OP 2.B.4: [M] Observar status de cada fonte  
- OP 2.B.5: [P] Mover cursor até “Reexecutar” (se falha)  
- OP 2.B.6: [B] Clicar em reexecutar  
- **Selection Rule:** Se coleta terminar sem falhas → prosseguir para Goal 3

---

## Goal 3: Validar resultados
### Method 3.A: Deduplicar
- OP 3.A.1: [P] Selecionar opção “Remover duplicados”  
- OP 3.A.2: [B] Clicar em executar deduplicação  
- OP 3.A.3: [R] Aguardar sistema processar  
- OP 3.A.4: [M] Pensar e revisar lista final  

### Method 3.B: Correlacionar achados
- OP 3.B.1: [P] Mover cursor até “Correlacionar por e-mail”  
- OP 3.B.2: [B] Clicar em correlacionar  
- OP 3.B.3: [R] Esperar resposta do sistema  
- OP 3.B.4: [M] Revisar resultados correlacionados  

### Method 3.C: Evidenciar
- OP 3.C.1: [P] Mover cursor até item do achado  
- OP 3.C.2: [B] Clicar em “Salvar evidência”  
- OP 3.C.3: [R] Esperar confirmação  
- OP 3.C.4: [M] Verificar se evidência foi anexada corretamente  

---

## Goal 4: Classificar riscos
### Method 4.A: Impacto x Probabilidade
- OP 4.A.1: [P] Selecionar matriz de riscos  
- OP 4.A.2: [B] Clicar em célula de classificação (Baixo, Médio, Alto)  
- OP 4.A.3: [R] Esperar registro do risco  

### Method 4.B: Mapear a normas
- OP 4.B.1: [P] Selecionar “Mapear para LGPD”  
- OP 4.B.2: [B] Clicar confirmar  
- OP 4.B.3: [R] Aguardar resposta  

---

## Goal 5: Montar relatório técnico
### Method 5.A: Preencher template
- OP 5.A.1: [K] Digitar título do relatório  
- OP 5.A.2: [K] Digitar resumo técnico  
- OP 5.A.3: [K] Inserir achados e riscos  
- OP 5.A.4: [P] Mover cursor até botão “Salvar”  
- OP 5.A.5: [B] Clicar em salvar  

### Method 5.B: Inserir gráficos e KPIs
- OP 5.B.1: [P] Selecionar aba “KPIs”  
- OP 5.B.2: [B] Clicar em “Gerar gráfico”  
- OP 5.B.3: [R] Aguardar visualização do gráfico  
- OP 5.B.4: [M] Validar se gráfico corresponde aos dados  

### Method 5.C: Revisar e Exportar
- OP 5.C.1: [P] Selecionar “Exportar PDF”  
- OP 5.C.2: [B] Clicar em exportar  
- OP 5.C.3: [R] Aguardar geração do arquivo  
- OP 5.C.4: [M] Conferir se relatório gerado está íntegro  
- **Selection Rule:** Se relatório não aprovado em revisão de pares → voltar a Method 5.A

---

## Legenda (KLM)
- **K (Keying):** Digitar no teclado (≈0.2s por tecla)  
- **P (Pointing):** Mover cursor até alvo na tela (≈1.1s)  
- **B (Button press):** Clicar botão do mouse (≈0.1s)  
- **H (Homing):** Alternar mão entre teclado e mouse (≈0.4s)  
- **M (Mental preparation):** Pensar/preparar próxima ação (≈1.2s)  
- **R (Response):** Tempo de resposta do sistema (variável)  

---

### Observação
Esse GOMS-KLM do Lucas cobre **todo o fluxo da investigação OSINT até o relatório técnico**.  
- Em cada Goal temos **Methods com Operators detalhados**.  
- Incluímos **Selection Rules** para lidar com falhas e exceções.  
- Pode ser usado tanto para análise de tarefas quanto para estimar **tempo total de execução** (somando tempos de KLM).


# ConcurTaskTree - Lucas (Executar Varredura OSINT)

T0: Executar Varredura OSINT

T0 = 
    T1 >> T2 >> T3 ||| T4 >> T5 >> T6

Onde:

- T1: Preparar alvo (tarefa do usuário)  
- T2: Configurar coleta (tarefa interativa)  
- T3: Executar varredura (tarefa do sistema)  
- T4: Validar achados (tarefa interativa)  
- T5: Classificar riscos (tarefa do usuário)  
- T6: Gerar relatório técnico (tarefa do sistema + usuário)  

### Relações:
- T1 >> T2 → só é possível configurar coleta após preparar o alvo.  
- T2 >> T3 → execução da varredura depende da configuração.  
- T3 ||| T4 → a validação pode ocorrer em paralelo à execução (comunicação entre sistema e usuário).  
- T4 >> T5 → só é possível classificar após validar.  
- T5 >> T6 → relatório é produzido somente após classificação.  



## Persona 2 – Marina Souza (Gerente de Segurança)

#### 1) HTA – Hierarchical Task Analysis

**Tarefa 0: Consolidar relatório OSINT em versão executiva e apresentá-lo à diretoria**

---

## Diagrama de Análise Hierárquica de Tarefas (estrutura em árvore)

> **Plano 0:** **1 > 2 > 3 > 4 > 5 > 6 > 7**  
> (Sequencial: importar → selecionar métricas → redigir sumário → revisar → preparar apresentação → apresentar → arquivar)

**0. Consolidar relatório OSINT**  
- **1. Importar achados técnicos**  
  - **1.1 Receber relatório técnico da equipe**  
  - **1.2 Selecionar seções relevantes para gestores**  
  - **Plano 1:** **1.1 > 1.2** (sequencial)  
- **2. Selecionar métricas relevantes**  
  - **2.1 Definir KPIs de risco** (quantidade de vazamentos, severidade, tempo de resposta)  
  - **2.2 Avaliar impacto no negócio** (financeiro, reputacional, compliance)  
  - **Plano 2:** **2.1 + 2.2** (paralelo; métricas e impacto analisados juntos)  
- **3. Redigir sumário executivo**  
  - **3.1 Estruturar tópicos principais**  
  - **3.2 Adaptar vocabulário para linguagem não técnica**  
  - **Plano 3:** **3.1 > 3.2** (sequencial)  
- **4. Revisar linguagem e clareza**  
  - **4.1 Eliminar jargão técnico**  
  - **4.2 Validar clareza com equipe**  
  - **Plano 4:** **4.1 > 4.2** (sequencial)  
- **5. Preparar material de apresentação**  
  - **5.1 Criar slides** (visuais, objetivos)  
  - **5.2 Inserir gráficos e dashboards**  
  - **Plano 5:** **5.1 + 5.2** (paralelo)  
- **6. Apresentar à diretoria**  
  - **6.1 Expor sumário executivo**  
  - **6.2 Responder dúvidas e coletar feedback**  
  - **Plano 6:** **6.1 > 6.2** (sequencial)  
- **7. Arquivar e registrar**  
  - **7.1 Salvar versão final aprovada**  
  - **7.2 Indexar em histórico/KB corporativo**  
  - **Plano 7:** **7.1 > 7.2** (sequencial)

**Regras de Seleção (globais):**  
- Se **tempo de reunião < 15min** → priorizar **2/3 métricas mais críticas** (seleção).  
- Se **diretoria exige detalhe técnico** → anexar apêndice técnico do Lucas.  
- Se **audiência não técnica** → ocultar termos complexos e manter foco em impacto de negócio.

---

## Tabela — Objetivos/Operações × Input / Ação / Feedback / Problemas / Recomendações

| **Objetivos / Operações** | **Input** | **Ação** | **Feedback** | **Problemas** | **Recomendações** |
|---|---|---|---|---|---|
| **0. Consolidar relatório OSINT** | Relatório técnico | Executar Plano 0 | Relatório executivo gerado | Foco técnico demais | Estrutura executiva obrigatória |
| **1. Importar achados técnicos** | Relatório técnico | Selecionar partes úteis | Dados filtrados | Excesso de detalhes técnicos | Criar checklist de seções mínimas |
| **2.1 Definir KPIs de risco** | Achados validados | Escolher métricas principais | Lista de KPIs | KPI irrelevante | Lista pré-aprovada de indicadores |
| **2.2 Avaliar impacto no negócio** | Riscos técnicos | Traduzir p/ impacto financeiro/reputacional | Impacto documentado | Falta de contexto de negócio | Consultar área de compliance |
| **3.1 Estruturar tópicos** | KPIs + achados | Criar sumário | Estrutura pronta | Texto longo | Usar bullet points |
| **3.2 Adaptar vocabulário** | Sumário técnico | Reescrever linguagem | Texto claro | Jargão técnico | Treinamento em linguagem executiva |
| **4.1 Eliminar jargão** | Sumário | Revisar termos | Texto simplificado | Termos não compreensíveis | Glossário comum |
| **4.2 Validar clareza** | Versão preliminar | Revisão equipe | Feedback recebido | Falta de alinhamento | Revisão obrigatória c/ dupla função |
| **5.1 Criar slides** | Sumário | Gerar apresentação | Slides prontos | Slides poluídos | Modelo padrão corporativo |
| **5.2 Inserir gráficos** | KPIs/impactos | Criar gráficos | Gráficos prontos | Gráficos confusos | Paleta oficial + dashboard |
| **6.1 Expor sumário executivo** | Relatório executivo | Apresentar | Feedback da diretoria | Tempo curto | Treinamento em pitch executivo |
| **6.2 Responder dúvidas** | Perguntas da diretoria | Esclarecer | Feedback anotado | Falta de preparo | Sessão Q&A preparada |
| **7.1 Salvar versão final** | Relatório executivo | Salvar | Arquivo gerado | Perda de versão | Versionamento obrigatório |
| **7.2 Indexar histórico** | Documento | Registrar em KB | Documento indexado | Dificuldade em buscar | Indexação padronizada |

---

## Observações didáticas
- Estrutura **idêntica ao HTA do Lucas**, mas o **foco em 6.x é executivo**, não técnico.  
- **Planos** indicam ordem, paralelismo e seleção de métricas conforme contexto.  
- **Tabela** mostra problemas comuns (ex.: jargão técnico, excesso de slides) e recomendações (ex.: glossário, modelo padrão).

# GOMS-KLM — Marina (Gestora de Segurança)

**Goal 0:** Consolidar relatório OSINT em versão executiva e apresentá-lo à diretoria

---

## Goal 1: Importar achados técnicos
### Method 1.A: Receber relatório técnico
- OP 1.A.1: [P] Mover cursor até e-mail/módulo de relatórios  
- OP 1.A.2: [B] Clicar em "Baixar relatório técnico"  
- OP 1.A.3: [R] Aguardar download  
- OP 1.A.4: [M] Validar que arquivo baixado está correto  

### Method 1.B: Selecionar seções relevantes
- OP 1.B.1: [K] Abrir arquivo e navegar até seções técnicas  
- OP 1.B.2: [P] Destacar achados críticos  
- OP 1.B.3: [B] Copiar para documento executivo  
- OP 1.B.4: [M] Validar se a seleção é suficiente para gestores  
- **Selection Rule:** Se relatório tiver excesso de dados → priorizar apenas severidade alta

---

## Goal 2: Selecionar métricas (KPIs)
### Method 2.A: Definir indicadores de risco
- OP 2.A.1: [P] Mover cursor até campo de indicadores  
- OP 2.A.2: [K] Inserir número de incidentes  
- OP 2.A.3: [K] Inserir severidade média  
- OP 2.A.4: [M] Pensar se métricas são adequadas  

### Method 2.B: Avaliar impacto no negócio
- OP 2.B.1: [K] Escrever breve descrição do impacto financeiro  
- OP 2.B.2: [K] Escrever impacto reputacional  
- OP 2.B.3: [M] Pensar se impacto traduz riscos técnicos em estratégicos  
- **Selection Rule:** Se diretoria exigir → incluir também riscos de compliance

---

## Goal 3: Redigir sumário executivo
### Method 3.A: Estruturar tópicos
- OP 3.A.1: [K] Escrever tópicos principais (3–5 bullet points)  
- OP 3.A.2: [M] Pensar sobre clareza e objetividade  

### Method 3.B: Adaptar vocabulário
- OP 3.B.1: [K] Reescrever frases técnicas em linguagem executiva  
- OP 3.B.2: [M] Revisar se texto é compreensível para não técnicos  
- **Selection Rule:** Se jargão ainda estiver presente → voltar a OP 3.B.1

---

## Goal 4: Revisar clareza
### Method 4.A: Eliminar termos técnicos
- OP 4.A.1: [P] Revisar texto linha por linha  
- OP 4.A.2: [K] Substituir termos complexos por equivalentes simples  

### Method 4.B: Validar com equipe
- OP 4.B.1: [P] Enviar versão preliminar para equipe  
- OP 4.B.2: [R] Aguardar feedback  
- OP 4.B.3: [M] Ajustar conforme comentários  

---

## Goal 5: Preparar material de apresentação
### Method 5.A: Criar slides
- OP 5.A.1: [P] Abrir software de apresentação  
- OP 5.A.2: [K] Inserir título da apresentação  
- OP 5.A.3: [K] Inserir tópicos do sumário executivo  

### Method 5.B: Inserir gráficos e dashboards
- OP 5.B.1: [P] Selecionar botão "Adicionar gráfico"  
- OP 5.B.2: [K] Escolher tipo (barra, pizza, linha)  
- OP 5.B.3: [R] Visualizar gráfico gerado  
- OP 5.B.4: [M] Validar se gráfico comunica bem a métrica  
- **Selection Rule:** Se gráfico confuso → trocar tipo de visualização  

---

## Goal 6: Apresentar à diretoria
### Method 6.A: Expor sumário
- OP 6.A.1: [P] Abrir apresentação em tela cheia  
- OP 6.A.2: [K] Falar tópicos principais  
- OP 6.A.3: [M] Pausar para avaliar reação da diretoria  

### Method 6.B: Responder dúvidas
- OP 6.B.1: [M] Interpretar pergunta feita pela diretoria  
- OP 6.B.2: [K] Responder com clareza  
- OP 6.B.3: [R] Esperar reação/feedback  
- **Selection Rule:** Se pergunta exigir detalhe técnico → anexar relatório de Lucas

---

## Goal 7: Arquivar versão final
### Method 7.A: Salvar relatório executivo
- OP 7.A.1: [P] Mover cursor até "Salvar como PDF"  
- OP 7.A.2: [B] Clicar em exportar  
- OP 7.A.3: [R] Aguardar arquivo ser gerado  

### Method 7.B: Indexar em histórico corporativo
- OP 7.B.1: [P] Acessar sistema de gestão documental  
- OP 7.B.2: [K] Inserir título e palavras-chave  
- OP 7.B.3: [B] Clicar em “Publicar/Arquivar”  
- OP 7.B.4: [M] Validar se documento foi indexado corretamente  

---

## Legenda (KLM)
- **K (Keying):** Digitar no teclado (≈0.2s por tecla)  
- **P (Pointing):** Mover cursor até alvo na tela (≈1.1s)  
- **B (Button press):** Clicar botão do mouse (≈0.1s)  
- **H (Homing):** Alternar mão entre teclado e mouse (≈0.4s)  
- **M (Mental preparation):** Pensar/preparar próxima ação (≈1.2s)  
- **R (Response):** Tempo de resposta do sistema (variável)  

---

### Observação
Esse GOMS-KLM da Marina cobre **todo o processo de transformar o relatório técnico em executivo**.  
- Cada **Goal** é detalhado em **Methods e Operators KLM**.  
- Incluímos **Selection Rules** para tratar casos práticos (prazo curto, gráficos confusos, perguntas inesperadas).  
- Útil para demonstrar como a **gestora interage com a interface e aplica raciocínio** até a entrega final.



# ConcurTaskTree - Marina (Consolidar Relatório Executivo)

T0: Consolidar Relatório Executivo

T0 =
    T1 >> T2 >> (T3 || T4) >> T5 >> T6

Onde:

- T1: Importar achados técnicos (tarefa do sistema)  
- T2: Selecionar métricas (tarefa do usuário)  
- T3: Redigir sumário executivo (tarefa do usuário)  
- T4: Revisar linguagem (tarefa interativa)  
- T5: Preparar apresentação (tarefa do usuário + sistema)  
- T6: Apresentar à diretoria (tarefa do usuário)  

### Relações:
- T1 >> T2 → só é possível selecionar métricas após importar os dados.  
- T2 >> (T3 || T4) → após a seleção, pode-se redigir e revisar em paralelo.  
- (T3 || T4) >> T5 → ambos devem estar finalizados antes da preparação da apresentação.  
- T5 >> T6 → apresentação depende da preparação dos materiais.  


_________________


## Entrega 6 - 22/09/2025 [Em andamento]

### Protótipo em Papel
(Inserir imagens/fotos dos protótipos desenhados à mão.)

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

### 3.1 Entrevista
- **Objetivo:** entender de forma detalhada as tarefas, dificuldades e o que os usuários esperam da ferramenta.
- **Como aplicar:** conversa de 30 a 45 minutos, presencial ou online, com gravação de áudio se a pessoa autorizar.
- **Roteiro:** perguntas sobre rotina de trabalho, etapas mais demoradas, pontos de erro, informações que gostaria de ver no relatório final.

### 3.2 Questionário
- **Objetivo:** confirmar em mais pessoas quais são as maiores necessidades e problemas.
- **Como aplicar:** formulário on-line (por exemplo Google Forms) com perguntas simples de múltipla escolha e algumas abertas; tempo de resposta de 5 a 8 minutos.
- **Exemplo de perguntas:** cargo e tempo de experiência, ferramentas que usa, grau de dificuldade em cada etapa (escala de 1 a 5), quais indicadores são mais importantes no relatório.

### 3.3 Grupo de discussão
- **Objetivo:** reunir analistas e gestores para debater e decidir o que é mais importante no sistema.
- **Como aplicar:** encontro de 1 hora com 6 a 8 participantes, mediado por um facilitador; anotar ou gravar com autorização.
- **Roteiro:** conversar sobre as tarefas mais comuns, maiores dificuldades e quais recursos consideram indispensáveis.

### 3.4 Observação do trabalho
- **Objetivo:** ver como o analista realmente trabalha no dia a dia para descobrir detalhes que não aparecem em entrevistas.
- **Como aplicar:** acompanhar a pessoa durante cerca de 1 hora enquanto ela faz uma investigação de teste; anotar etapas, erros e tempo gasto, pedindo sempre consentimento.

---

### Checklist de cuidado ético
- Apresentar termo de consentimento com objetivo, tempo e contato.
- Garantir que os dados serão guardados em local seguro e apagados no prazo combinado.
- Não coletar senhas ou dados reais de clientes.
- Deixar claro que a pessoa pode sair da pesquisa a qualquer momento.

---

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
  - **Redução de 40%** no tempo de coleta manual (comparado ao processo atual).  
  - **Taxa de sucesso ≥ 90%** na execução de varreduras sem falhas.  
  - **Tempo médio para gerar relatório ≤ 5 minutos** após término da coleta.  
  - **Satisfação ≥ 80%** em questionários de usabilidade (SUS ou escala 1–5).  


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
