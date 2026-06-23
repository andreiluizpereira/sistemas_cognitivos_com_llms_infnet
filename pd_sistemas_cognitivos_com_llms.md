Olá, Andrei.

Este projeto consolida, na prática, os conhecimentos desenvolvidos na disciplina **Sistemas Cognitivos com Large Language Models**.

Ao longo da disciplina, você aprendeu a construir aplicações com LLMs usando Hugging Face, APIs de modelos de linguagem, modelos locais, técnicas de prompt engineering, embeddings semânticos, busca vetorial e pipelines RAG.

Agora, você deverá transformar esses conhecimentos em um sistema funcional, inspirado em uma situação real ou plausível, no qual um LLM seja usado como componente de uma solução cognitiva.

### Contexto

Aplicações baseadas em LLMs já fazem parte de muitos contextos profissionais: atendimento automatizado, análise de documentos, busca em bases internas, sumarização de conteúdo, triagem de solicitações, geração de respostas estruturadas, suporte a decisões e consulta a bases de conhecimento.

No entanto, construir uma aplicação com LLMs não significa apenas enviar uma pergunta para um modelo. Em aplicações reais, é preciso saber escolher modelos, estruturar prompts, controlar saídas, gerar embeddings, recuperar documentos relevantes, lidar com limitações de contexto, reduzir alucinações, proteger dados sensíveis e justificar decisões de arquitetura.

Neste projeto, você deverá construir uma aplicação que utilize LLMs como parte de um sistema. A solução deve demonstrar domínio técnico sobre o funcionamento do pipeline, e não apenas consumo superficial de uma API ou ferramenta pronta.

O projeto pode utilizar OpenAI, Hugging Face, modelos baixados localmente, GPT4All ou outra alternativa tecnicamente justificada. Você não precisa usar todas essas opções. O importante é que as escolhas sejam coerentes com o problema, com os recursos disponíveis e com as competências da disciplina.

### Questão do projeto

**Como você pode construir uma aplicação cognitiva com LLMs capaz de receber entradas em linguagem natural, acessar ou processar conhecimento externo, produzir respostas úteis ou estruturadas e justificar tecnicamente suas decisões de arquitetura?**

A partir dessa questão, defina um problema, escolha um corpus ou conjunto de documentos, implemente a solução e explique as decisões tomadas em cada etapa.

### Tarefa

Você deverá desenvolver uma aplicação funcional com LLMs em Python.

A solução deve representar um sistema aplicado, e não apenas uma sequência de testes isolados. Ela deve envolver entrada em linguagem natural, uso de modelo de linguagem, estratégia de prompting, geração ou interpretação de saída, recuperação de informação por embeddings e algum mecanismo de resposta fundamentada em documentos ou conhecimento externo.

O projeto pode ser aplicado a diferentes contextos, como:

*   assistente para consulta a documentos internos;
    
*   busca semântica em base de conhecimento;
    
*   análise e classificação de textos corporativos;
    
*   sumarização e triagem de documentos;
    
*   extração estruturada de informações;
    
*   assistente de suporte técnico;
    
*   chatbot para perguntas sobre manuais ou políticas;
    
*   análise de tickets, reclamações ou feedbacks;
    
*   assistente privado para documentos sensíveis;
    
*   sistema de perguntas e respostas com base em corpus próprio.
    

O cenário escolhido deve permitir avaliar tanto o uso de LLMs quanto a arquitetura do sistema construído.

### Corpus ou base de conhecimento

O projeto deve utilizar um corpus, conjunto de documentos ou base textual que permita testar as funcionalidades da aplicação.

Essa base pode ser composta por:

*   documentos públicos;
    
*   manuais técnicos;
    
*   FAQs;
    
*   páginas institucionais;
    
*   artigos;
    
*   políticas internas fictícias;
    
*   documentos próprios anonimizados;
    
*   textos sintéticos criados para simular um cenário real;
    
*   base pública de perguntas, respostas ou documentos.
    

A base deve ser suficiente para permitir consultas, recuperação de contexto, comparação de respostas e avaliação das estratégias de busca.

Caso utilize documentos próprios ou sensíveis, forneça uma versão anonimizada, sintética ou substituta que permita a avaliação pelo professor. A ausência de dados compartilháveis não justifica uma entrega incompleta.

### Construção do projeto

O projeto deve ser construída a partir de **5 pontos elegíveis**, alinhados às competências da disciplina. Em cada ponto, você deverá fazer escolhas técnicas compatíveis com o seu problema. Você não precisa utilizar todas as ferramentas citadas, mas precisa construir uma solução coerente, funcional e demonstrável.

1. **Aplicação NLP com LLMs e modelos pré-treinados**

A solução deve demonstrar uso de pelo menos um modelo pré-treinado para executar tarefas de linguagem natural relacionadas ao problema escolhido.

Você pode utilizar uma ou mais das seguintes abordagens:

*   Hugging Face transformers;
    
*   Hugging Face Inference API;
    
*   OpenAI API;
    
*   modelo baixado localmente;
    
*   GPT4All;
    
*   outro modelo ou provedor justificado.
    

Você pode implementar tarefas como:

*   classificação de texto;
    
*   geração de texto;
    
*   question answering;
    
*   sumarização;
    
*   extração de informação;
    
*   reescrita ou padronização de textos;
    
*   análise de instruções em linguagem natural.
    

Também devem ser discutidas escolhas relevantes de modelo, como diferença entre modelos encoder-only e decoder-only, uso de tokenização, parâmetros de geração, limitações observadas e adequação ao caso de uso.

O objetivo deste ponto é demonstrar que você sabe operar modelos de linguagem como componentes técnicos de uma aplicação, e não apenas chamar uma ferramenta pronta.

2. **Prompt engineering e saídas controladas**

A solução deve demonstrar uso planejado de prompts para orientar o comportamento do modelo.

Você deve aplicar e comparar técnicas de prompting adequadas ao problema (utilize pelo menos 3 técnicas associadas), como:

*   zero-shot prompting;
    
*   few-shot prompting;
    
*   chain-of-thought, quando fizer sentido;
    
*   prompts com papel, contexto, tarefa e formato de saída;
    
*   prompts para classificação, extração, resumo ou geração;
    
*   meta-prompting para melhorar instruções;
    
*   iteração de prompts com comparação entre versões.
    

A aplicação deve produzir algum tipo de saída controlada, como:

*   JSON;
    
*   tabela;
    
*   lista estruturada;
    
*   objeto Python;
    
*   classificação com justificativa;
    
*   resposta com campos definidos;
    
*   resumo padronizado.
    

Quando houver saída estruturada, você deve implementar algum tipo de validação, parsing ou tratamento de erro. O relatório deve mostrar como os prompts foram testados, ajustados e avaliados.

3. **Embeddings semânticos e recuperação de informação**

A solução deve utilizar embeddings para representar documentos, trechos, consultas ou respostas.

Você pode utilizar:

*   sentence-transformers;
    
*   embeddings de OpenAI;
    
*   embeddings do Hugging Face;
    
*   embeddings locais;
    
*   GPT4All ou nomic.embed.text();
    
*   outro modelo de embeddings justificado.
    

A recuperação pode ser implementada com uma ou mais estratégias:

*   busca vetorial por similaridade;
    
*   comparação por cosseno;
    
*   comparação por distância euclidiana;
    
*   busca híbrida com BM25 e recuperação densa;
    
*   uso de FAISS;
    
*   uso de ChromaDB;
    
*   outro vector store ou mecanismo justificado.
    

A solução deve incluir consultas de teste e análise dos resultados recuperados. Você deve discutir quando a recuperação funcionou bem, quando falhou e como isso afeta a qualidade da resposta final.

4. **Inferência local, remota ou privada**

A solução deve explicitar a estratégia de execução escolhida para o modelo.

Você pode optar por:

*   API cloud, como OpenAI ou Hugging Face;
    
*   modelo local baixado e executado na máquina;
    
*   GPT4All;
    
*   API local compatível com OpenAI;
    
*   combinação entre execução remota e local;
    
*   outra alternativa justificada.
    

Você não precisa usar GPT4All e outra forma de RAG ao mesmo tempo. Você também não precisa usar OpenAI, Hugging Face e modelo baixado simultaneamente. O importante é justificar a escolha feita.

O projeto deve discutir dimensões como:

*   privacidade;
    
*   custo;
    
*   latência;
    
*   disponibilidade;
    
*   controle;
    
*   facilidade de integração;
    
*   limitações de hardware;
    
*   dependência de internet;
    
*   risco de exposição de dados.
    

Caso utilize execução local, apresente evidências de funcionamento e limitações observadas. Caso utilize API externa, documente as dependências, variáveis de ambiente e cuidados para não expor chaves, tokens ou dados sensíveis.

5. **Pipeline RAG ou resposta fundamentada em conhecimento externo**

A solução deve incluir um mecanismo de resposta fundamentada em documentos, trechos recuperados ou conhecimento externo.

Você pode implementar um pipeline RAG completo ou uma variação tecnicamente equivalente. O sistema deve demonstrar como uma consulta é transformada em recuperação de contexto e como esse contexto é usado para gerar uma resposta.

Uma implementação típica pode incluir:

*   carregamento de documentos;
    
*   divisão em chunks;
    
*   geração de embeddings;
    
*   indexação em vector store;
    
*   recuperação top-k;
    
*   construção manual do prompt aumentado;
    
*   geração de resposta com base no contexto recuperado;
    
*   sessão de perguntas e respostas reproduzível.
    

Você pode utilizar:

*   ChromaDB;
    
*   FAISS;
    
*   GPT4All LocalDocs;
    
*   embeddings locais;
    
*   embeddings remotos;
    
*   modelo local;
    
*   API cloud;
    
*   outra solução justificada.
    

O projeto deve analisar pelo menos alguns aspectos do pipeline, como:

*   estratégia de chunking;
    
*   qualidade dos trechos recuperados;
    
*   comparação de respostas com e sem contexto;
    
*   caso de alucinação reduzida pelo uso de RAG;
    
*   ponto de falha mais provável;
    
*   limitação de contexto;
    
*   risco de prompt injection;
    
*   risco de vazamento de contexto;
    
*   controles de segurança propostos.
    

O objetivo deste ponto é demonstrar que você compreende a arquitetura de uma aplicação baseada em recuperação e geração, independentemente da ferramenta específica escolhida.

### Desenvolvimento da solução

O projeto deve ser desenvolvido em Python, preferencialmente em notebooks ou scripts organizados por etapa.

A solução deve ser construída de forma progressiva. Primeiro, defina o problema e a base de conhecimento. Depois, escolha o modelo ou provedor, estruture prompts, gere saídas controladas, implemente embeddings e recuperação, e finalize com uma resposta fundamentada em documentos ou contexto externo.

O professor deve conseguir reproduzir o projeto a partir dos arquivos entregues. Se o projeto utilizar APIs externas, documente as dependências, variáveis de ambiente e formas de configuração. Quando houver limitações de acesso, custo ou credenciais, forneça alternativa local, dados de teste, mock funcional ou instruções suficientes para validação.

Chaves reais, tokens, senhas e dados sensíveis não devem ser incluídos na entrega.

Código funcional, isoladamente, não é suficiente. A avaliação também considera a qualidade da análise, a coerência das decisões técnicas, a interpretação dos resultados, a segurança da solução e a capacidade de justificar escolhas de arquitetura.

### Entrega

Você deverá entregar três artefatos:

1.  **Código completo da aplicação**, organizado em notebooks ou scripts Python.
    
2.  **Pipeline RAG ou mecanismo equivalente de resposta fundamentada**, com README.md explicando como instalar dependências, preparar documentos, indexar a base e executar consultas.
    
3.  **Relatório técnico em PDF**, explicando o problema, a arquitetura, as decisões técnicas, os resultados, as limitações e os riscos de segurança.
    

Sugestão de organização dos arquivos:

*   c01\_modelos\_llm.ipynb;
    
*   c02\_prompting.ipynb;
    
*   c03\_embeddings\_busca.ipynb;
    
*   c04\_inferencia\_local\_ou\_remota.ipynb;
    
*   c05\_rag\_pipeline.ipynb;
    
*   requirements.txt;
    
*   README.md.
    

O relatório deve conter:

*   nome do aluno;
    
*   nome da disciplina;
    
*   título do projeto;
    
*   descrição do problema escolhido;
    
*   descrição do corpus ou base de conhecimento;
    
*   justificativa para uso de LLMs;
    
*   modelos, APIs ou ferramentas utilizadas;
    
*   tarefas NLP implementadas;
    
*   estratégia de prompting;
    
*   prompts utilizados e versões testadas;
    
*   estratégia de avaliação dos prompts;
    
*   uso de JSON, parsing ou saída estruturada;
    
*   modelos de embeddings utilizados;
    
*   estratégia de busca vetorial, híbrida ou equivalente;
    
*   exemplos de consultas e documentos recuperados;
    
*   estratégia de execução local, remota ou privada;
    
*   justificativa sobre privacidade, custo, latência e controle;
    
*   descrição do pipeline RAG ou mecanismo equivalente;
    
*   estratégia de chunking;
    
*   vector store ou mecanismo de recuperação utilizado;
    
*   exemplos de consultas e respostas;
    
*   análise de respostas com e sem contexto recuperado;
    
*   análise de falhas do pipeline;
    
*   riscos de segurança identificados;
    
*   controles propostos;
    
*   instruções de reprodução;
    
*   limitações da solução;
    
*   melhorias futuras
    

O arquivo PDF deve seguir o padrão:

nome\_sobrenome\_sistemas-cognitivos-linguagem-natural\_aplicacoes-llms.pdf

Exemplo:

ana\_silva\_sistemas-cognitivos-linguagem-natural\_aplicacoes-llms.pdf