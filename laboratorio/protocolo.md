# Laboratório Gemini 4

1. Execute cada tarefa ao menos três vezes por modelo em sessões novas, usando os mesmos dados, ferramentas, prazo e limite de tentativas. Registre superfície, modelo real, esforço e data.
2. Avalie a saída com a régua abaixo. Marque cada tentativa, incluindo correções e falhas. Use dados fictícios em ferramentas externas e peça confirmação antes de qualquer ação externa.
3. Compare a taxa de entregas válidas, a mediana do tempo total e o custo por entrega aprovada. Se não houver aprovação, marque o custo por entrega como indisponível. Se a interface não informar tokens ou custo, deixe o campo vazio. Use o valor faturado quando disponível.
4. Calcule custo por entrega somando o custo de todas as tentativas de um modelo para uma tarefa e dividindo pelo número de execuções aprovadas. Conte uma aprovação por execução, mesmo que tenha havido várias tentativas. Não trate custo ausente como zero.

## Pedidos e critérios

| Tarefa | Pedido para copiar e testar | Aceite |
| --- | --- | --- |
| Tabela de comprovantes | Use os documentos fictícios abaixo. Entregue CSV com id, data ISO e valor em centavos. Aponte duplicatas e separe itens sem valor. | Três linhas válidas, um item incompleto, uma duplicata. Total válido de 3170 centavos. |
| Página de pedidos | Crie uma página offline que mostre os comprovantes abaixo, filtre por status e salve o último filtro localmente. Inclua testes manuais. | Abre offline, funciona pelo teclado, mostra os totais corretos, guarda o último filtro e cabe em tela de 375 px. |
| Jogo curto 3D | Crie uma cena navegável por teclado com três objetos colecionáveis e reinício. Use arte original e dependências explicitamente listadas. | Abre sem erro, funciona com teclado, termina em três itens e reinicia sem deixar estado residual. |
| SVG | Desenhe um pássaro original em SVG, com asas animadas e opção de movimento reduzido. | XML válido, sem recursos externos, legível redimensionado, animação desativada com preferência por movimento reduzido. |
| Agentes | Divida a construção da página acima em planejamento, implementação e verificação. Registre a passagem do trabalho e a prova final. | Mesmo aceite da página. Compare agente único e coordenação multiagente em rodadas distintas. |
| Computer use | Em uma página local fictícia, crie um pedido com o ID C-103, filtre por esse ID e confirme o total antes de simular envio. | ID correto, total registrado, sem ações externas. Conte desvios e correções. |
| Cena 3D | Construa uma pequena sala com iluminação, câmera navegável e três objetos clicáveis. | Os três objetos reagem, a câmera não atravessa paredes, a cena toca no navegador e mostra a taxa de quadros. |

### Dados fictícios para os comprovantes

| ID | Data | Valor |
| --- | --- | --- |
| C-101 | 19/11/2026 | R$ 12,40 |
| C-102 | 19/11/2026 | R$ 9,30 |
| C-101 | 19/11/2026 | R$ 12,40 |
| C-103 | 20/11/2026 | R$ 10,00 |
| C-104 | 20/11/2026 | ausente |
