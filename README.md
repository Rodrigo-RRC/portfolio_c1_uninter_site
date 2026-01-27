# 🌐 Portfólio C1 - UNINTER

Este projeto consiste em um site pessoal desenvolvido como parte da **atividade prática da disciplina Ferramentas de Desenvolvimento Web**, no curso de **Tecnologia em Ciência de Dados** pela UNINTER.

---

## 🔗 Link do site publicado

Acesse o site do portfólio em:
👉 [https://rodrigo-rrc.github.io/portfolio_c1_uninter_site/](https://rodrigo-rrc.github.io/portfolio_c1_uninter_site/)

---

## 🗂️ Estrutura do projeto

- `index.html` — Página inicial com boas-vindas e introdução
- `sobre.html` — Página com informações pessoais
- `formacao.html` — Página com trajetória acadêmica
- `portfolio.html` — Links e descrições de projetos
- `contato.html` — Formulário de contato
- `css/estilo.css` — Estilo visual aplicado a todo o site
- `.gitignore` — Arquivo de controle do Git

---

## 👨‍💻 Tecnologias utilizadas

- HTML5
- CSS3
- Git e GitHub Pages

---

## 🧠 Autor

**Rodrigo Ribeiro Carvalho**  
João Pessoa – PB  
Curso: Tecnologia em Ciência de Dados – UNINTER

---

> Este portfólio foi pensado para ser simples, limpo e funcional — com navegação clara e estrutura bem organizada. A entrega inclui o código fonte versionado no GitHub e a publicação funcional via GitHub Pages.

Model Card Llama-3.1 70BModel Card Model Card Llama-3.1Llama-3.1  70B70B

1. Informações Essenciais e Uso Pretendido (Intended Use)1. Informações Essenciais e Uso Pretendido (Intended Use)1. Informações Essenciais e Uso Pretendido (Intended Use)

| Campo | Descrição |
| --- | --- |
| Nome do Modelo | Llama-3.1 70B |
| Versão | 3.1 |
| Visão Geral/Limitações | Objetivo: Modelo de linguagem multilíngue, ajustado por instruções, otimizado para diálogo e chat.  Uso Pretendido: Comercial e pesquisa em múltiplas línguas.  Limitações: Uso proibido se violar leis ou a Política de Uso Aceitável. Não deve ser usado isoladamente, mas sim como parte de um sistema de IA com salvaguardas. Exemplos de salvaguardas incluem: monitoramento de saída, filtros, supervisão humana. Limitações conhecidas do modelo incluem: alucinações, vieses, desempenho menor em certas línguas menos representadas, sensibilidade a instruções adversas (prompt injection), etc. |
| Criadores/Equipe | Meta |
| Data da Última Atualização | 24 de julho de 2024 |
| Tags | Geração de Texto, Transformers, PyTorch, Llama, Conversacional, Inferência de Geração de Texto |
| Licença | Llama 3.1 Community License |
| Origem do Modelo | Externo, vide https://huggingface.co/meta-llama/Llama-3.1-70B-Instruct e https://www.llama.com/docs/model-cards-and-prompt-formats/llama3_1 Termos da licença e política de uso disponíveis em https://huggingface.co/meta-llamahttps://huggingface.co/meta-llama |

2. Dados de Treinamento e Fonte (Data Provenance)22. . Dados de Treinamento e Fonte (Data Provenance)Dados de Treinamento e Fonte (Data Provenance)

| Campo | Descrição |
| --- | --- |
| Dataset(s) Utilizado(s) | Pré-treinamento: Aproximadamente 15 trilhões de tokens de dados online públicos. Ajuste Fino (Fine-tuning): Inclui mais de 25 milhões de exemplos gerados sinteticamente, além de datasets de instrução públicos |
| Pré-condições do Dataset | Corte de Conhecimento (Knowledge Cutoff): dezembro de 2023 |
| Multimodalidade Suportada | Modelo de apenas texto (text in/text out). Suporta Texto Multilíngue como entrada e Texto e Código Multilíngue como saída |

3. Detalhes Técnicos e Arquitetura33. . Detalhes Técnicos e ArquiteturaDetalhes Técnicos e Arquitetura

| Campo | Descrição |
| --- | --- |
| Arquitetura do Modelo | Modelo de linguagem autorregressivo com arquitetura Transformer otimizada. Versões ajustadas usam SFT e RLHF. Utiliza Grouped-Query Attention (GQA). |
| Procedimento de Treinamento | Treinamento realizado em clusters de GPU personalizados da Meta. Utilizou um total cumulativo de 39.3 milhões de horas de GPU (hardware H100-80GB) para toda a coleção Llama 3.1 |
| Nível de Automação | Não detalhado nas fontes |

4. Métricas de Desempenho e Avaliação44. . Métricas de Desempenho e AvaliaçãoMétricas de Desempenho e Avaliação

| Campo | Descrição |
| --- | --- |
| Métricas de Desempenho | Principais métricas: Acurácia, F1-Score, Exact Match (Question and Answer) e Pass@1 (código) |
| Benchmark Scores | Benchmarks (70B-Instruct, 5-shot): MMLU 83.6; ARC-Challenge 94.8; HumanEval (código) 80.5; API-Bank (ferramentas) 90.0. Para português (MMLU 5-shot): ~ 80 (avaliação externa). |
| Limitações Conhecidas | O modelo pode produzir respostas imprecisas, tendenciosas ou censuráveis, especialmente em domínios sensíveis ou línguas com menor representação no treinamento |
| Métricas de Robustez e Privacidade | Avaliações contínuas de robustez via red teaming com especialistas (cibersegurança, IA responsável). Foco em riscos críticos: CBRNE, segurança infantil, habilitação de ataques cibernético |

5. Considerações Éticas, Riscos e Mitigações55. . Considerações Éticas, Riscos e MitigaçõesConsiderações Éticas, Riscos e Mitigações

| Campo | Descrição |
| --- | --- |
| Considerações Éticas | Valores centrais: abertura, inclusividade e utilidade, respeitando a dignidade e autonomia dos usuários. |
| Riscos Ambientais, Sociais e de Conformidade (ESG) | Ambiental: ~11.390 tCO₂eq (coleção Llama 3.1). Social: riscos críticos em CBRNE, segurança infantil, ataques cibernéticos. Conformidade: uso proibido para atividades ilegais, assédio, fraude e exercício não licenciado de profissões reguladas. |
| Ações de Mitigação | Mitigações: fine-tuning de segurança, ferramentas Llama Guard 3, Prompt Guard e Code Shield, além da aplicação da Política de Uso Aceitável. |
| Pós-condições | O modelo pode reduzir a carga de trabalho no desenvolvimento de sistemas de IA seguros, desde que acompanhado de salvaguardas e testes específicos. |

6. Orientações de Uso e Implantação66. . Orientações de Uso e ImplantaçãoOrientações de Uso e Implantação

| Campo | Descrição |
| --- | --- |
| Diretrizes de Uso Responsável | Uso deve estar em conformidade com a Licença Comunitária Llama 3.1 e a Política de Uso Aceitável. Desenvolvedores devem adaptar e validar a segurança para seus casos específicos |
| Contexto Operacional/Ambiental | Deve ser implantado como parte de um sistema de IA com salvaguardas adicionais. Requer a biblioteca transformers (versão >= 4.43.0) para inferência conversacional. Suporta otimizações de memória usando bitsandbytes (carregamento em 8-bit ou 4-bit). |
| Instruções Acionáveis | Exemplos de código disponíveis para uso com transformers e para Tool Use via chat templates. |
| Mecanismos de Feedback | Reportes podem ser feitos via GitHub (issues), canais de segurança/abuso e e-mail indicado na documentação oficial |

