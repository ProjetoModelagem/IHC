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


## Entrega 4 - 08/09/2025 [Em andamento]

### 1) Cenário de Análise/Problema
(Descrever situação real que gera dificuldade para o usuário. É uma "história triste", não contém solução, apenas o problema.)

### 2) Questões de Refinamento
(Questões que ajudam a detalhar melhor o problema descrito.)

### 3) Refinamento do Cenário Análise/Problema
(Texto revisado e mais claro do cenário de problema, considerando as questões de refinamento.)

---

## Entrega 5 - 15/09/2025 [Em andamento]

### Análise de Tarefas

#### 1) HTA (Hierarchical Task Analysis)
(Colocar o diagrama + explicação da funcionalidade.)

#### 2) GOMS
(Colocar o diagrama + explicação da funcionalidade.)

#### 3) CTT (ConcurTaskTrees)
(Colocar o diagrama + explicação da funcionalidade.)

---

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
