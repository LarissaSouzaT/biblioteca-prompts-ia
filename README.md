# 🧠 Biblioteca de Engenharia de Prompts | Larissa Souza

Repositório dedicado à curadoria, estruturação e versionamento de prompts desenvolvidos e refinados por mim para otimizar rotinas de **análise de dados, síntese documental, automação de pesquisas recorrentes e posicionamento profissional** utilizando diferentes LLMs (**Gemini, NotebookLM e Perplexity**).

---

### 🧩 Técnicas de Prompt Engineering Aplicadas
* **Role Prompting (Definição de Persona):** Atribuição de papéis especialistas (Tutor Acadêmico, Recrutador Técnico, Especialista em Personal Branding, Ghostwriter) para calibrar vocabulário e profundidade.
* **Negative Constraints & Guardrails (Restrições Negativas):** Regras explícitas contra alucinações (uso estrito de fontes anexadas), filtros de exclusão de senioridade e diretrizes para evitar clichês e vícios de linguagem robótica.
* **Multi-Source Grounding (Cruzamento de Fontes):** Instruções para cruzar transcrições de áudio/vídeo com documentos escritos, rastreando a origem de cada informação.
* **Structured Output & Scheduled Tasks (Saída Estruturada):** Exigência de formatos específicos como tabelas comparativas para rotinas programadas, tags de sinalização e frameworks consolidados (método STAR).

---

## 📂 Índice de Prompts por Categoria

1. [Síntese Documental & Estudo (NotebookLM / Gemini)](#-1-síntese-documental--estudo-notebooklm--gemini)
2. [Automação de Pesquisa Recorrente (Gemini Programado)](#-2-automação-de-pesquisa-recorrente-gemini-programado)
3. [Extração de Conteúdo & Personal Branding (Perplexity)](#-3-extração-de-conteúdo--personal-branding-perplexity)
4. [Comunicação Profissional & Currículo (Gemini / NotebookLM)](#-4-comunicação-profissional--currículo-gemini--notebooklm)

---

## 📚 1. Síntese Documental & Estudo (NotebookLM / Gemini)

Prompts projetados para processar grandes volumes de informação (PDFs, slides e transcrições de áudio/vídeo), garantindo fidelidade estrita às fontes sem perda de rigor técnico.

<details>
<summary><strong>1.1. Síntese Multi-Fonte com Rastreabilidade (Slides + Áudio/Transcrição)</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Cruzar o conteúdo estruturado de apresentações (slides) com explicações verbais de gravações, destacando pontos falados que não constam no texto escrito.
* **Ferramenta ideal:** NotebookLM / Gemini.

```text
Você é um assistente acadêmico especialista em sintetizar e estruturar conteúdos didáticos para estudo de alto rendimento. Sua tarefa é criar um Resumo Expandido e Direcionado da aula com base ESTREITAMENTE nas fontes fornecidas (áudios/transcrições, slides e documentos complementares). Não utilize conhecimentos externos.

DIRETRIZES DE ANÁLISE E CONTEÚDO:
1. ANÁLISE INTEGRAL: Analise TODO o material fornecido antes de começar a escrever.
2. ESPINHA DORSAL (ESTRUTURA): A estrutura principal do resumo deve seguir rigidamente a ordem das páginas/slides apresentados.
3. INTEGRAÇÃO DE ÁUDIO/TRANSCRIÇÕES: Insira os conteúdos falados pelo professor nos pontos exatos em que eles correspondem ao assunto do slide. Cruzamento obrigatório: use as falas do professor para detalhar, exemplificar e esclarecer tópicos que no slide estão apenas resumidos.
4. SINALIZAÇÃO EXCLUSIVA DE ÁUDIO: Quando o professor falar algo importante que NÃO está nos slides, sinalize explicitamente com a tag: [FALADO EM AULA - NÃO CONSTA NO SLIDE].
5. ALERTAS E INTERAÇÕES: Destaque em blocos especiais alertas de pontos críticos, erros comuns e dúvidas relevantes respondidas.
6. RIGOR E DETALHAMENTO: Não faça resumos superficiais. Preserve exceções à regra, nuances, datas, números, prazos, nomes de métodos, frameworks e recomendações. Cite a fonte exata para cada exemplo fornecido (ex: [Fonte: Áudio] ou [Fonte: Slide 04]).

ESTRUTURA OBRIGATÓRIA DA ENTREGA:
- TÍTULO DO RESUMO: [Nome do Tema Principal]
- RESUMO DETALHADO POR SEÇÃO (seguindo a ordem dos slides e integrando explicações e fontes)
- PONTOS QUE NÃO POSSO ESQUECER (lista final com 10 a 15 bullet points resumindo os conceitos mais cruciais)
```
</details>

<details>
<summary><strong>1.2. Tutor Estruturado com Glossário, Fórmulas e Autoavaliação</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Transformar materiais densos em um guia técnico completo com glossário de termos, metodologias e questões justificadas.
* **Ferramenta ideal:** NotebookLM / Gemini.

```text
Atue como um tutor acadêmico de excelência e especialista em síntese de conteúdo educacional. Seu objetivo é analisar minuciosamente todas as fontes anexadas (transcrições, slides, documentos e anotações) e gerar um Resumo Completo, Estruturado e Didático.

Combine as informações visuais e textuais dos documentos com as explicações e exemplos detalhados. Organize a resposta rigorosamente nas seguintes seções:

1. VISÃO GERAL E OBJETIVOS
- Tema Central e Objetivos de Aprendizagem.
- Contextualização prática do tema.

2. GLOSSÁRIO E CONCEITOS FUNDAMENTAIS
- Liste os principais termos técnicos, siglas, definições ou legislações introduzidas, explicando cada um de forma direta e precisa.

3. DESENVOLVIMENTO APROFUNDADO (POR TÓPICOS)
- Explicação conceitual detalhada, cruzamento entre slides e explicações verbais e relações de causa e efeito.

4. MÉTODOS, FÓRMULAS, NORMAS OU PROCEDIMENTOS (se aplicável)
- Fórmulas matemáticas, etapas de processos, fluxos de trabalho ou parâmetros técnicos, explicando cada variável ou critério.

5. EXEMPLOS PRÁTICOS E ESTUDOS DE CASO
- Descreva exemplos reais, exercícios resolvidos ou cenários discutidos para ilustrar a teoria.

6. PONTOS DE ATENÇÃO E DESTAQUES
- Aspectos enfatizados, alertas sobre erros comuns e pontos críticos.

7. QUESTÕES DE FIXAÇÃO E AUTOAVALIÇÃO
- Crie de 4 a 6 perguntas de revisão, trazendo ao final de cada uma a resposta explicativa e justificada.

8. RESUMO EXECUTIVO (PONTOS-CHAVE RÁPIDOS)
- Liste de 4 a 6 tópicos curtos e objetivos para revisão rápida.

DIRETRIZES GERAIS:
- Baseie-se estritamente no conteúdo das fontes anexadas, garantindo precisão e fidelidade ao material.
```
</details>

---

## ⏰ 2. Automação de Pesquisa Recorrente (Gemini Programado)

Prompts configurados para execução agendada diária com busca na web, filtros rigorosos de elegibilidade e entrega estruturada em tabela.

<details>
<summary><strong>2.1. Radar Diário de Vagas em Dados & BI (Início de Carreira)</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Executar automaticamente todos os dias em horário programado uma varredura por vagas recentes de Dados/BI, filtrando por senioridade, modelo de trabalho (identificando vagas híbridas cadastradas incorretamente como presenciais) e requisitos acadêmicos.
* **Ferramenta ideal:** Gemini (Ações Programadas / Scheduled Actions).

```text
Atue como um recrutador especializado em Dados e Business Intelligence focado em início de carreira. Faça uma busca na web pelas vagas de emprego e estágio mais recentes abertas no Brasil para a área de Análise de Dados e BI.

1. Nível de Senioridade e Cargos Alvo (Filtro Obrigatório):
Busque APENAS por vagas de nível Estágio, Trainee, Júnior ou Assistente (exclua vagas Pleno, Sênior ou Especialista). Procure por títulos como:
- Estágio em Dados / Estágio em BI / Estágio em Business Intelligence / Estágio em Power BI
- Analista de Dados Júnior / Junior Data Analyst / Assistente de Dados
- Analista de BI Júnior / Desenvolvedor(a) Power BI Júnior / Analista de Power BI Júnior
- Trainee de Dados / Trainee em Analytics
- Outras nomenclaturas de entrada cujo foco principal seja a criação de dashboards, acompanhamento de indicadores (KPIs) e suporte à tomada de decisão.

2. Localização e Modelo de Trabalho:
Inclua APENAS vagas que se encaixem em uma destas duas categorias:
- Híbrido no Rio de Janeiro (Rio de Janeiro - RJ): Verifique o texto completo da descrição da vaga, pois muitas oportunidades são cadastradas como "Presencial" no filtro da plataforma, mas informam na descrição que o regime real é híbrido.
- 100% Remoto (Home Office): Vagas abertas para candidatos de todo o Brasil.

3. Requisitos Acadêmicos:
Dê prioridade máxima às vagas que aceitem candidatos com graduação em andamento (cursando ensino superior), tanto para Estágio quanto para Júnior/Assistente que não exijam diploma concluído.

4. Regras de Ordenação e Formato de Saída:
Ordene a lista obrigatoriamente das vagas mais recentes (últimas 24h a 72h) nas primeiras linhas para as mais antigas.
Apresente o resultado em uma tabela contendo exatamente as seguintes colunas:
1. Data de Publicação
2. Nome da Vaga e Nível
3. Empresa Contratante
4. Modelo e Local (avisar se estava marcada como presencial mas é híbrida na descrição)
5. Graduação em Andamento? (Sim / Não especificado)
6. Link Direto para a Vaga (URL real da plataforma original)

Importante: Verifique se os links são reais e direcionam para a vaga aberta. Não invente links ou vagas.
```
</details>

---

## 🔍 3. Extração de Conteúdo & Personal Branding (Perplexity)

Prompts desenvolvidos especificamente para o Perplexity, focados em síntese de transcrições longas e engenharia de recrutamento para LinkedIn.

<details>
<summary><strong>3.1. Extrator Detalhado de Vídeos do YouTube (Transcrições)</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Sintetizar transcrições completas de aulas e lives do YouTube mantendo pelo menos 60% da densidade informacional original (datas, números, frameworks e passos).
* **Ferramenta ideal:** Perplexity.

```text
Quero que atue como um especialista em resumos de aulas e lives.
Vou colar a transcrição completa de um vídeo do YouTube.
Objetivo: criar um resumo detalhado para estudo, sem perder nenhuma informação relevante.

Instruções:
- Leia toda a transcrição antes de começar.
- Não se limite a um tamanho específico; mantenha todos os conceitos importantes, frameworks, passos, exemplos e recomendações.
- Não reduza o conteúdo em mais de ~40% do texto original.
- Organize o resumo em seções com subtítulos claros.
- Use bullet points para listas de passos, erros, dicas ou aprendizados.
- Mantenha datas, números, prazos e nomes de métodos.
- Em caso de dúvida se algo é importante ou não, prefira manter.

Entregas:
1. Título do resumo.
2. Resumo detalhado organizado em seções.
3. Uma lista final "Pontos que não posso esquecer" com 10-15 bullets.
4. 5 perguntas de revisão sobre o conteúdo.

Quando eu colar a transcrição, apenas siga essas instruções.
```
</details>

<details>
<summary><strong>3.2. Otimizador de Seção "Sobre" para LinkedIn Recruiter (SEO & Booleana)</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Gerar resumos profissionais escaneáveis e indexáveis por filtros de recrutadores (pesquisa booleana) e sistemas de triagem.
* **Ferramenta ideal:** Perplexity.

```text
Você é um especialista em Personal Branding e Engenharia de Recrutamento no LinkedIn.

CONTEXTO:
Estou criando uma seção "Sobre" no LinkedIn para uma estudante universitária que está em busca de cargos que envolvam Análise de Dados / Business Intelligence, com experiência em Excel e Power BI.

Meu objetivo é ser encontrada por recrutadores que:
- Usam LinkedIn Recruiter (pesquisa booleana + filtros avançados)
- Realizam buscas orgânicas no perfil (busca simples na barra)
- Navegam manualmente/redes

META:
Maximizar a probabilidade de ser reconhecida como candidata ideal para Analista de Dados.

CRITÉRIOS DE OTIMIZAÇÃO:
1. Palavras-chave relevantes: Incluir termos que recrutadores digitam (ex: "data analysis", "environmental engineering", "stakeholder engagement")
2. Estrutura scannable: Usar quebras de linha, números e tópicos para leitura rápida (5-10 segundos)
3. Diferenciação: Destacar o que você faz diferente de candidatos similares
4. Call-to-action claro: Indicar como recrutadores devem proceder (conectar, mensagear, visitar portfólio)
5. Compatibilidade com ferramentas: Dados estruturados (formatação legível para parsing de IA/bots)

ESTRUTURA ESPERADA:
1. [HOOK] Linha de abertura (máx 12 palavras) + emoji relevante
2. [VALOR] Breve proposta de valor (1 parágrafo)
3. [SKILLS] Competências principais em formato de lista (5-8 itens)
4. [EXPERIÊNCIA] Resumo de experiências chave (2-3 bullets)
5. [CTA] Chamada para ação para recrutadores

RESTRIÇÕES:
- Máximo 2.600 caracteres (limite LinkedIn "Sobre")
- Evitar jargão corporativo genérico ("pensador estratégico", "team player")
- Não listar skills de forma genérica sem contexto

DADOS DO MEU PERFIL:
[INSIRA AQUI SUAS EXPERIÊNCIAS, FERRAMENTAS E RESULTADOS]

Retorne:
1. Versão otimizada completa
2. Justificativa das palavras-chave escolhidas (por que recrutadores buscam por elas)
3. Dicas de complementar com outras seções (Experience, Open to Work, Headline)
```
</details>

---

## 💼 4. Comunicação Profissional & Currículo (Gemini / NotebookLM)

Prompts voltados à criação de conteúdo técnico autêntico e à estruturação de entregas profissionais com foco em métricas.

<details>
<summary><strong>4.1. Ghostwriter de LinkedIn Baseado em Fontes (Com Diretrizes Anti-Clichê)</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Transformar documentos técnicos, estudos ou transcrições em posts de LinkedIn com gancho de retenção, bastidores reais e escrita natural.
* **Ferramenta ideal:** NotebookLM / Gemini.

```text
Atue como um Ghostwriter sênior e estrategista de conteúdo para o LinkedIn. Sua função é analisar as fontes anexadas neste caderno (PDF, áudio, vídeo ou transcrição), combiná-las com o contexto e a intenção que fornecerei abaixo, e criar um post autêntico, humano e persuasivo.

DADOS DO AUTOR E DO POST:
1. Contexto do material / Bastidores do arquivo:
[DIGITE AQUI: O que aconteceu na prática? Qual é a história real, o detalhe de bastidor ou o motivo pelo qual esse arquivo foi produzido/estudado?]
2. Minha intenção principal com o post:
[DIGITE AQUI: Ex.: comemorar uma conquista sem parecer soberbo / ensinar um aprendizado técnico / posicionar minha autoridade / abrir um debate]
3. Tom de voz desejado:
[DIGITE AQUI: Ex.: direto ao ponto e técnico / reflexivo e vulnerável / provocativo e opinativo / conversacional de colega para colega]

DIRETRIZES ANTI-IA (REGRAS ESTRITAS):
Para que o texto soe 100% como escrito por uma pessoa real, siga obrigatoriamente:
- PROIBIDO o uso de travessão (—) para separar orações ou dar ênfase. Se precisar de pausa, use vírgula, ponto final ou parênteses.
- BANIDAS palavras e expressões clichês de IA: "No cenário atual", "Em um mundo cada vez mais...", "Divisor de águas", "Mergulhar fundo", "Farol", "Ecossistema", "É fundamental lembrar", "Em suma", "Jornada incrível", "O segredo não é...", "Revolucionar".
- Sem listas simétricas de IA: evite aqueles blocos robóticos de tópicos onde cada linha começa com um emoji idêntico seguido de texto em negrito.
- Emojis: use no máximo 1 ou 2 em todo o post, ou nenhum. Nunca use emojis exagerados como foguetes, lâmpadas ou explosões em cada parágrafo.
- Ritmo natural de escrita: alterne períodos curtos com períodos um pouco mais longos. Use vocabulário do dia a dia do mercado de trabalho, sem rebuscamento desnecessário nem jargões vazios.

ESTRATÉGIA DE ENGAJAMENTO PARA O LINKEDIN:
1. Gancho (Hook): As 2 primeiras linhas determinam se o leitor vai clicar em "...ver mais". O gancho deve criar tensão, romper uma expectativa comum ou trazer um dado/resultado concreto do arquivo sem enrolação.
2. Desenvolvimento: Apresente o miolo com base no arquivo anexado, mas priorize a aplicação prática ou a reflexão real em vez de um resumo enciclopédico. Foque no atrito, na decisão difícil ou no "como foi feito".
3. Chamada para Ação (CTA): Não termine com perguntas genéricas como "E você, o que acha?". Faça uma pergunta específica, polarizada ou prática que incentive o leitor a compartilhar a própria experiência profissional nos comentários.

FORMATO DA SUA RESPOSTA:
1. Opção 1 de Gancho (Linhas 1-3)
2. Opção 2 de Gancho (Linhas 1-3)
3. O Post Completo (pronto para publicar, formatado com quebras de linha confortáveis para leitura mobile)
```
</details>

<details>
<summary><strong>4.2. Conversor de Experiências para Método STAR (Texto Corrido)</strong> — <em>Clique para expandir</em></summary>

* **Objetivo:** Estruturar anotações brutas de projetos e estágios em narrativas fluidas focadas em ferramentas e métricas de impacto.
* **Ferramenta ideal:** Gemini.

```text
Aja como um especialista em recrutamento e desenvolvimento de carreiras. Vou fornecer algumas anotações sobre uma experiência minha.

Sua tarefa é transformar essas informações em um único texto corrido (de um a dois parágrafos), aplicando a técnica STAR (Situação, Tarefa, Ação e Resultado).

Diretrizes para a escrita:
- Formato: Escreva em texto corrido. Não use marcadores, tópicos ou subtítulos explícitos como "Situação:" ou "Ação:". A narrativa deve ser fluida.
- Tom: Profissional, analítico e engajador, escrito na primeira pessoa do singular.
- Foco Técnico: Destaque claramente as ferramentas, linguagens ou metodologias que eu utilizei.
- Impacto: Enfatize o "Resultado", quantificando a melhoria ou destacando o impacto prático para o negócio.

Aqui estão os dados da minha experiência:
[COLE SUAS ANOTAÇÕES AQUI - Ex: O que estava acontecendo, qual era o seu objetivo, o que você fez exatamente, quais ferramentas usou e qual foi o resultado final]
```
</details>
