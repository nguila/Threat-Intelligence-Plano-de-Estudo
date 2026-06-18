# Threat Intelligence – Plano de Estudo (10 Semanas, 3h/sem) + Cheat Sheet de Labs

Este repositório contém um plano de estudo de 10 semanas para aprender **Cyber Threat Intelligence (CTI)** dedicando cerca de **3 horas por semana**, mais uma **cheat sheet** com laboratórios e recursos práticos.

## Índice

- [Secção 1 – Plano de 10 semanas](#secção-1--plano-de-10-semanas-3-horas-por-semana)
  - [Semanas 1–2: Nível 1 – Fundamentos](#semanas-12-nível-1--fundamentos)
  - [Semanas 3–4: Nível 2 – Ciclo de Inteligência & Processo](#semanas-34-nível-2--ciclo-de-inteligência--processo)
  - [Semanas 5–6: Nível 3 – Dados Reais](#semanas-56-nível-3--dados-reais)
  - [Semanas 7–8: Nível 4 – Comportamento & MITRE ATTCK](#semanas-78-nível-4--comportamento--mitre-attck)
  - [Semanas 9–10: Nível 5 – Mini Workflow de CTI](#semanas-910-nível-5--mini-workflow-de-cti)
- [Secção 2 – Cheat Sheet de Labs](#secção-2--cheat-sheet-de-laboratórios-e-recursos-práticos)

---

## Secção 1 – Plano de 10 Semanas (3 Horas por Semana)

Este plano assume cerca de **3 horas de estudo por semana**. O objetivo é ir dos fundamentos até conseguires montar um pequeno workflow de CTI por tua conta.

### Semanas 1–2: Nível 1 – Fundamentos

Objetivo: perceber o que é Threat Intelligence e dominar o vocabulário básico.

#### Semana 1 (≈3h) – O que é CTI?

**Estudo (≈1,5–2h)**

- Ver 1–2 vídeos/introduções a CTI (por exemplo, cursos gratuitos de CTI) para perceber:
  - O que é CTI.
  - Tipos de CTI (tático, operacional, estratégico).
  - Para que é usada no dia a dia.

**Prática (≈1h)**

- Escrever 1 página (ou 10–15 pontos) em português a explicar:
  - O que é CTI.
  - Quem a usa.
  - 3 problemas concretos que ajuda a resolver.

**Marco**

- Consegues explicar CTI em linguagem simples a alguém não técnico (por exemplo, um amigo ou familiar).

#### Semana 2 (≈3h) – Dados, Indicadores e Inteligência

**Estudo (≈1–1,5h)**

- Rever os conceitos de IOC, IOA, TTP e a diferença entre:
  - Dado em bruto
  - Indicador
  - Inteligência

**Prática (≈1,5–2h)**

- Juntar 10–15 exemplos:
  - Notícias de cibersegurança
  - Linhas de log (podem ser inventadas)
  - IPs/domínios
- Para cada exemplo, classificar como:
  - Dado
  - IOC
  - Inteligência  
  E escrever 1 frase a justificar a escolha.

**Pergunta de autoavaliação**

- Consigo explicar a diferença entre um IOC e um TTP em apenas 1 frase?

---

### Semanas 3–4: Nível 2 – Ciclo de Inteligência & Processo

Objetivo: passar a olhar para CTI como **processo** (ciclo de inteligência), e não só como feeds ou ferramentas.

#### Semana 3 (≈3h) – Ciclo de Inteligência

**Estudo (≈1,5h)**

- Estudar as 6 fases do ciclo de inteligência:
  - Direção
  - Recolha
  - Processamento
  - Análise
  - Disseminação
  - Feedback

**Prática (≈1,5h)**

- Desenhar o ciclo.
- Para cada fase, escrever 1 exemplo concreto, usando um cenário simples:
  - Ex.: phishing a clientes de uma loja online em Portugal.

**Marco**

- Consegues dizer as 6 fases de cabeça, sem consultar apontamentos.

#### Semana 4 (≈3h) – Requisitos & Fontes

**Estudo (≈1–1,5h)**

- Aprender a escrever **requisitos de inteligência**:
  - São as perguntas específicas que a CTI deve responder.

**Prática (≈1,5–2h)**

- Definir 3–5 requisitos de inteligência para uma organização fictícia.
- Criar uma tabela:
  - Requisito → Fontes possíveis (blogs, feeds, relatórios, OSINT) → Motivo.

**Pergunta de autoavaliação**

- Sei dizer qual é a pergunta que quero responder antes de abrir uma ferramenta nova?

---

### Semanas 5–6: Nível 3 – Dados Reais

Objetivo: conseguir transformar dados e IOCs em notas de inteligência úteis.

#### Semana 5 (≈3h) – Ler Relatórios & Extrair IOCs

**Estudo (≈1–1,5h)**

- Ler 1 relatório de incidente (ou artigo técnico) sobre um ataque real:
  - Blog de fornecedor de segurança
  - Relatório público de incidente

**Prática (≈1,5–2h)**

- Criar uma tabela:
  - IOC | Tipo (IP, domínio, hash, ficheiro, etc.) | Onde surgiu no relatório | Porque é relevante.
- Opcional:
  - Usar ferramentas públicas (VirusTotal, URLScan, AbuseIPDB) para acrescentar 1–2 linhas de contexto a alguns IOCs.

**Nota de segurança**

- Usa apenas IOCs públicos de relatórios.
- Não envies dados sensíveis teus ou de empresas reais.

**Marco**

- Já consegues pegar num texto técnico e extrair uma lista organizada de IOCs com contexto básico.

#### Semana 6 (≈3h) – Nota Analítica Curta

**Estudo (≈1–1,5h)**

- Ver 1 exemplo de relatório CTI curto (ou apresentação) para perceber a estrutura:
  - Resumo
  - Detalhes importantes
  - IOCs principais
  - Recomendações

**Prática (≈1,5–2h)**

- Usando o relatório da semana 5, escrever 5–10 pontos que respondam:
  - O que aconteceu?
  - Quem foi visado?
  - Que IOCs são mais importantes?
  - O que um defensor deve fazer a seguir?

**Pergunta de autoavaliação**

- Um analista de SOC conseguiria criar uma regra ou alerta concreto a partir da tua nota?

---

### Semanas 7–8: Nível 4 – Comportamento & MITRE ATT&CK

Objetivo: descrever ataques em termos de **comportamentos** (tácticas e técnicas), não só em listas de IOCs.

#### Semana 7 (≈3h) – Introdução ao ATT&CK & Tácticas

**Estudo (≈1,5–2h)**

- Explorar a matriz MITRE ATT&CK:
  - Ver as tácticas (Initial Access, Execution, Persistence, etc.).
  - Ver algumas técnicas associadas a cada táctica.

**Prática (≈1–1,5h)**

- Escolher 3 tácticas.
- Para cada uma, escolher 1 técnica.
- Para cada técnica, escrever:
  - “O atacante faz X usando esta técnica; o defensor pode Y para detetar ou mitigar”.

**Marco**

- Consegues dar pelo menos 3 exemplos claros de técnicas ATT&CK e de como defenderes‑te delas.

#### Semana 8 (≈3h) – Mapear Relatório para ATT&CK

**Estudo (≈1,5–2h)**

- Pegar num relatório (pode ser o da semana 5 ou um novo) e sublinhar as frases que descrevem **comportamentos**:
  - Como o atacante obteve acesso.
  - Como se movimentou na rede.
  - Como executou código, etc.

**Prática (≈1–1,5h)**

- Mapear pelo menos 2–3 desses comportamentos para técnicas ATT&CK.
- Para cada técnica, escrever 1–2 recomendações defensivas específicas:
  - Logs a ativar
  - Regras a criar
  - Controlos a reforçar

**Pergunta de autoavaliação**

- Consigo contar a história do ataque quase sem mencionar IPs ou domínios, só falando em tácticas e técnicas?

---

### Semanas 9–10: Nível 5 – Mini Workflow de CTI

Objetivo: correr um pequeno **ciclo de CTI completo** e produzir um relatório acionável.

#### Semana 9 (≈3h) – Planear & Recolher

**Estudo (≈1h)**

- Rever rapidamente:
  - Requisitos de inteligência
  - Ciclo de inteligência
  - ATT&CK
  - Tipos de fontes

**Prática (≈2h)**

- Escolher um tema bem focado:
  - Ex.: campanha de phishing específica, um malware comum, ou um grupo APT concreto.
- Escrever 3 perguntas de inteligência sobre esse tema.
- Recolher 3–5 fontes públicas (posts de blog, relatórios, avisos CERT, etc.).
  - Para cada fonte, anotar:
    - Data
    - Quem publicou
    - 3–5 pontos principais

**Marco**

- Ficas com um pequeno “dossiê” de fontes, todas sobre o mesmo tema.

#### Semana 10 (≈3h) – Analisar & Escrever Relatório

**Estudo (≈1–1,5h)**

- Rever exemplos e boas práticas de relatórios CTI:
  - Estrutura clara
  - Linguagem orientada a ação
  - Recomendações concretas e priorizadas

**Prática (≈1,5–2h)**

- Usar as fontes da semana 9 para identificar padrões:
  - Tácticas e técnicas usadas
  - Tipo de alvo
  - Infraestrutura recorrente
  - IOCs comuns
- Mapear, se possível, 2–3 comportamentos para ATT&CK.
- Escrever um relatório de 1–2 páginas (ou 15–25 pontos) com:
  - Escopo/perguntas
  - Principais conclusões
  - Comportamentos mais relevantes
  - 5–10 recomendações priorizadas

**Pergunta de autoavaliação final**

- Um defensor ou gestor conseguiria tomar decisões práticas só com base no teu relatório?

---

## Secção 2 – Cheat Sheet de Laboratórios e Recursos Práticos

Usa esta lista para escolher labs e plataformas práticas de acordo com o teu nível atual.

### Nível 1 – Fundamentos

- **ArcX – Cyber Threat Intelligence 101** (curso grátis, introdutório de CTI)  
  [https://arcx.io/courses/cyber-threat-intelligence-101](https://arcx.io/courses/cyber-threat-intelligence-101)  

- **TryHackMe – Intro to Cyber Threat Intel** (sala/lab introdutório de CTI)  
  [https://tryhackme.com/room/cyberthreatintel](https://tryhackme.com/room/cyberthreatintel)  

- **Cybrary – Intro to Cyber Threat Intelligence** (curso de introdução a CTI)  
  [https://www.cybrary.it/course/intro-cyber-threat-intelligence](https://www.cybrary.it/course/intro-cyber-threat-intelligence)  

### Nível 2 – Ciclo de Inteligência & OSINT básico

- **ArcX – vídeos sobre o ciclo de inteligência** (incluídos no CTI 101).  
- **CyberDefenders – labs de OSINT/Intel iniciais** (plataforma de desafios blue team)  
  [https://cyberdefenders.org](https://cyberdefenders.org)  

- **GitHub – Awesome Threat Intelligence** (lista de feeds, ferramentas e recursos de CTI)  
  [https://github.com/hslatman/awesome-threat-intelligence](https://github.com/hslatman/awesome-threat-intelligence)  

### Nível 3 – IOCs, Enriquecimento & Notas CTI

- **TryHackMe – Intro to Cyber Threat Intel** (rever a parte de enriquecimento de IOCs)  
  [https://tryhackme.com/room/cyberthreatintel](https://tryhackme.com/room/cyberthreatintel)  

- **Ferramentas de reputação / enriquecimento** (para testar com IOCs de relatórios públicos):  
  - VirusTotal  
  - URLScan  
  - AbuseIPDB  

- **MISP – materiais de treino com dados estruturados de threat intel**  
  [https://github.com/MISP/misp-training](https://github.com/MISP/misp-training)  

### Nível 4 – MITRE ATT&CK & Comportamentos

- **MITRE – ATT&CK for Cyber Threat Intelligence Training** (série de módulos online)  
  [https://attack.mitre.org/resources/learn-more-about-attack/training/cti/](https://attack.mitre.org/resources/learn-more-about-attack/training/cti/)  

- **YouTube – How to Use the MITRE ATT&CK Framework for CTI** (vídeo explicativo)  
  [https://www.youtube.com/watch?v=a8SazLVJQ4o](https://www.youtube.com/watch?v=a8SazLVJQ4o)  

- **Blue Team Labs Online – investigações e desafios blue team**  
  [https://blueteamlabs.online](https://blueteamlabs.online)  

### Nível 5 – Workflow de CTI & Projetos

- **CyberDefenders – desafios mais avançados** (OSINT, threat hunting, incident response)  
  [https://cyberdefenders.org](https://cyberdefenders.org)  

- **MISP – plataforma de threat intel + materiais de treino**  
  - Site oficial: [https://misp.github.io/misp-website/index.html](https://misp.github.io/misp-website/index.html)  
  - Treino: [https://github.com/MISP/misp-training](https://github.com/MISP/misp-training)  

- **Blue Team Labs Online – relatórios CTI a partir de investigações**  
  [https://blueteamlabs.online](https://blueteamlabs.online)  
  > Sugestão: no final de cada investigação, tenta sempre escrever uma pequena “threat intel note”.
