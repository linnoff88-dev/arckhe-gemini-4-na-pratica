# Gemini 4 Neon, Argon e Hydrogen

Pesquisa documental consultada em 19 de novembro de 2026. A escolha depende da tarefa, do volume e de quanto custa chegar a uma entrega que passou na validaçêo.

| Modelo | Como o Google o posiciona | Entrada / saída padrêo¹ | Ponto de partida para testar |
| --- | --- | ---: | --- |
| Gemini 4 Neon | Raciocínio avançado com conclusêo rápida de tarefas completas | US$ 3 / US$ 15 | Engenharia de software e análise de documentos em várias etapas |
| Gemini 4 Argon | Raciocínio profundo em atividades longas e complexas | US$ 2 / US$ 10 até 30/11/2026. US$ 4 / US$ 20 a partir de 01/12/2026 | Referência para fluxos longos ou automações onde ele já funciona |
| Gemini 4 Hydrogen | Execuçêo rápida para tarefas recorrentes e programaçêo cotidiana | US$ 1,50 / US$ 7,50 na camada paga | Classificaçêo, extraçêo, triagem e iteraçêo rápida |

¹ Dólares por milhêo de tokens. A saída inclui tokens de raciocínio. O Hydrogen dispõe de camada gratuita com limites. Valores de cache, ferramentas e planos sêo tratados à parte. Fontes [tarifas do Google AI Studio](https://aistudio.google.com/docs/pricing), [Neon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/), [Argon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-argon/), [Hydrogen](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-hydrogen/).

## O que mostrou a Arena

Recorte do índice geral de agentes consultado em 19/11/2026. Todos os três rótulos estavam em nível High. Hydrogen aparecia como preliminar. Os números descrevem sessões daquela avaliaçêo e mudam conforme o recorte e a data. Os custos sêo medianas da Arena, nêo tarifas por token. [Agent Arena Index](https://arena.ai/leaderboard/agent), [visêo geral com o recorte consultado](https://arena.ai/leaderboard?_bhlid=8325d1911e1251418d49dc2a32436e88cc3b5c98).

| Modelo (High) | Pontuaçêo | Custo mediano | Tempo mediano |
| --- | ---: | ---: | ---: |
| Neon | 1.333 | US$ 2,60 | 8,4 min |
| Argon | 1.229 | US$ 0,66 | 7,0 min |
| Hydrogen | 1.271 | US$ 1,50 | 5,3 min |

Neon liderou em pontuaçêo entre os três no recorte. Hydrogen teve o menor tempo mediano. Argon teve o menor custo mediano, apesar de Hydrogen ter tarifa unitária menor. Apurar a tarefa, o esforço, os insumos e as tentativas é o que explica custos de uma execuçêo específica.

## O que mudou no teste de automaçêo da Zapier

No AutomationBench 1.0.6, Neon obteve 54,3% em High, Argon 51,3% em High e Hydrogen 51,1% em High. Neon subiu a 56,3% em XHigh, com 370 de 657 tarefas aprovadas. O critério da Zapier exige que todas as condições previstas para o estado final da tarefa sejam cumpridas. Em High, a Zapier estimou US$ 0,88 por tentativa para Neon e US$ 1,63 para Argon. O relatório traz a pontuaçêo do Hydrogen, mas fica sem um custo diretamente comparável. Essa estimativa usa tarifas e hipóteses de cache da avaliaçêo. [Relatório AutomationBench da Zapier](https://zapier.com/benchmarks/gemini-neon-4-report).

O Argon teve custo mediano menor na Agent Arena, enquanto o Neon High teve custo estimado menor na Zapier. As avaliações cobrem tarefas e agregações diferentes. A inversêo é um bom motivo para medir no próprio fluxo.

## O que as quatro referências sugerem

As notas de trabalho convergem em três perguntas: quanto o modelo entrega por tentativa, como a orquestraçêo afeta o resultado e quantos ciclos de revisêo sêo necessários. Jogos, SVG e 3D demonstram possibilidades. Uma demo selecionada nêo mede taxa de sucesso em repetiçêo. A divisêo de tarefas entre agentes e a verificaçêo automática também mudam o resultado, mesmo mantendo o modelo. O estudo da Sakana AI ilustra a evoluçêo de estratégias num ambiente delimitado. [Demonstrações e minutagem do canal Prompt Engineering](https://chooseto.ai/watch/Q0ShBenKyqo), [documentaçêo do Google Antigravity](https://antigravity.google/docs/models), [Digital Red Queen](https://sakana.ai/drq/).

O criador de Prompt Engineering afirma no vídeo que usou acesso antecipado ao modelo e que havia acabado de ingressar no Google. As demonstrações mostram o que ele conseguiu produzir naquele contexto. [Declaraçêo do criador e minutagem](https://chooseto.ai/watch/Q0ShBenKyqo).

Na documentaçêo consultada, o Google confirma a chegada de Neon em 18/11, com janela de contexto de 1 milhêo de tokens na Gemini API e acesso via Google AI Studio pago, Gemini para empresas, Gemini e Antigravity conforme o plano. Os limites de cada produto podem diferir. [Anúncio do Neon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/), [ficha do modelo](https://deepmind.google/models/model-cards/gemini-4-neon/).

A comparaçêo com Fable 5.2 citada nas notas fica como pista para reproduçêo. Faltam identificaçêo suficiente da tarefa, configuraçêo e dados brutos para publicá-la como resultado validado. Este projeto tem pesquisa documental, protocolo e materiais para repetiçêo. Nenhuma execuçêo própria de Neon, Argon ou Hydrogen compõe os resultados acima.

## Faça a comparaçêo no seu trabalho

Pegue uma tarefa recorrente (Hydrogen como ponto de partida), uma entrega de várias etapas (Neon) e uma tarefa longa cujo histórico você já conhece (Argon). Preserve o pedido, dados, ferramentas e critério de aceite. Se mudar a configuraçêo, crie outra rodada. O [laboratório](laboratorio/protocolo.md) inclui materiais e uma [planilha de tentativas](laboratorio/tentativas.csv).
