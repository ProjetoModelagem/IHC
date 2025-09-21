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

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/7012ec32-692b-4b5e-9142-4fc67e3988f9" />


---

### Persona – Autor: Guilherme de Abreu  
**Nome:** Marina Souza  
**Idade:** 32 anos  
**Profissão:** Gerente de Segurança da Informação  
**Objetivos:** ter relatórios claros para apresentar.  
**Dores:** perda de tempo procurando dados manuais, dificuldade em consolidar informações.  
**Expectativas:** ferramenta confiável, relatórios com linguagem executiva, métricas visuais.  

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/75428df1-a853-483c-9700-f919bbb93828" />


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



#### 2) GOMS – Relatório OSINT Técnico

## Goal (G0)
**Produzir relatório OSINT técnico confiável.**

---

## Sub-goals
- **G1**: Preparar alvo e fontes  
- **G2**: Coletar dados  
- **G3**: Validar resultados  
- **G4**: Classificar riscos  
- **G5**: Montar relatório técnico  
- **G6**: Revisar e exportar  

---

## Operators (KLM)
- **K**: Keystroke (digitação)  
- **P**: Point (apontar/clicar)  
- **M**: Mental (decisão, reflexão, análise)  
- **Rᴿ**: Resposta do sistema  

---

## Método Exemplo – G2 (Coleta)
1. **Abrir módulo de coletas** (P)  
2. **Selecionar APIs** (P M)  
3. **Inserir alvo** (K M)  
4. **Iniciar varredura** (P)  
5. **Monitorar progresso** (Rᴿ M)  

---

## Selection Rules
- **Se prazo é curto** → priorizar fontes rápidas.  
- **Se coleta falha** → reexecutar fonte alternativa.  

---

## Explicação da Funcionalidade
O modelo **GOMS** detalha cada ação de Lucas, desde cliques até análises mentais.  
Ele evidencia:  
- Onde o tempo é gasto no processo.  
- Como decisões (selection rules) influenciam a fluidez da execução.  
- A relação entre interação humana e resposta do sistema para garantir eficiência.  


#CTT - ConcurTaskTrees
```ctt
Realizar_OSINT =
  Preparar_Alvo >> 
  (Configurar_Fontes ||| Disparar_Coleta) >> 
  Monitorar_Execucao >> 
  Validar_Achados >> 
  Classificar_Risco >> 
  Montar_Relatorio_Tecnico >> 
  Revisar_Exportar

Validar_Achados = Deduplicar >> Correlacionar >> Evidenciar
Montar_Relatorio_Tecnico = Template_Tecnico >> Inserir_Evidencias
```

**Explicação da funcionalidade: O CTT mostra a possibilidade de tarefas em paralelo (ex.: configurar fontes enquanto coleta roda). Esse modelo ajuda a otimizar multitarefa e prever gargalos no fluxo de Lucas.


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


#### 2) GOMS – Relatório Executivo

#### Goal (G0)
**Produzir resumo executivo claro e convincente.**

---

#### Sub-goals
- **G1**: Importar achados  
- **G2**: Selecionar KPIs estratégicos  
- **G3**: Redigir sumário executivo  
- **G4**: Revisar linguagem  
- **G5**: Preparar material de apoio  
- **G6**: Apresentar à diretoria  

---

#### Operators (KLM)
- **K**: Keystroke (digitação)  
- **P**: Point (apontar/clicar)  
- **M**: Mental (decisão, reflexão, análise)  
- **S**: Preparar slides  

---

#### Método Exemplo – G3 (Redação)
1. **Listar tópicos de maior impacto** (M K)  
2. **Reescrever em linguagem executiva** (K M)  
3. **Inserir exemplos visuais** (P K)  

---

#### Selection Rules
- **Se audiência é executiva** → reduzir detalhes técnicos.  
- **Se reunião é estratégica** → destacar impacto financeiro.  

---

#### Explicação da funcionalidade
O modelo **GOMS** de Marina mostra a cadeia de ações **mentais e motoras** necessárias para transformar achados técnicos em **insights de negócio**.  
Ele destaca a importância das **decisões de comunicação**, que influenciam diretamente a clareza e a efetividade da mensagem ao público executivo.

### 3) CTT – ConcurTaskTrees

```ctt
Sintetizar_Relatorio_Executivo =
  Importar_Achados >> 
  Selecionar_KPIs >> 
  Redigir_Sumario_Exec >> 
  Revisar_Linguagem >> 
  Preparar_Apresentacao >> 
  Apresentar_Diretoria

Selecionar_KPIs = (Risco_Severidade ||| Nº_Incidentes ||| Tempo_Resposta)
Preparar_Apresentacao = Criar_Slides >> Inserir_Graficos
```

#### Explicação da funcionalidade 
O CTT mostra que Marina pode selecionar múltiplas métricas em paralelo antes de compor o sumário executivo.
Ele também evidencia a importância da revisão da linguagem, garantindo que a diretoria compreenda os riscos e indicadores sem jargão técnico, transformando relatórios técnicos em insights estratégicos.

_________________


## Entrega 6 - 22/09/2025 [Em andamento]

### Protótipo em Papel
(Inserir imagens/fotos dos protótipos desenhados à mão.)

---

## Entrega 7 - 29/09/2025 [Em andamento]

### 1) Identificação de Necessidades dos Usuários e Requisitos de IHC
- *Que dados coletar?*
- *De quem coletar?*

### 2) Aspectos Éticos
(Justificar com conceitos da disciplina — ex.: LGPD, privacidade, consentimento informado, etc.)

### 3) Ferramentas de Coleta de Dados  
#### 3.1) Nome do instrumento e objetivo  
#### 3.2) Como aplicar  
#### 3.3) Instrumento (link do formulário, roteiro de entrevista, etc.)

---

## Entrega 8 - 06/10/2025 [Em andamento]

### 1) Características da Plataforma
- *Descrição do Software:*  
- *Descrição do Hardware:*  
- *Lista de Capacidades da Plataforma (com explicação):*  
- *Lista de Restrições da Plataforma (com explicação):*

### 2) Princípios Gerais do Projeto
(Tabela com princípios + links + justificativa — ex.: LGPD, Acessibilidade, ISO 9241.)

### 3) Metas de Usabilidade
- *Qualitativas:*  
- *Quantitativas:*  
(Definir metas com justificativa e porcentagem.)

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
