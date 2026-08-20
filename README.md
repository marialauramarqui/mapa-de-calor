# Mapas de Calor — exemplos

Dois mapas de calor **na mesma página**, mostrando quando usar cada tipo de cor.

**Todos os dados são fictícios**, gerados só para demonstrar as visualizações.

## Ver online

https://marialauramarqui.github.io/mapa-de-calor/

| Exemplo | O que mostra | Cor |
|---|---|---|
| Pedidos por dia da semana e hora | volume de pedidos, dia × hora (08h–21h) | **sequencial** — uma cor só, claro → escuro |
| Atingimento da meta de vendas por loja | % da meta batido, loja × mês | **semáforo** — vermelho, amarelo e verde |

## Por que só um dos dois usa semáforo

Vermelho-amarelo-verde carrega julgamento: diz que um lado é ruim e o outro é bom.
Isso só faz sentido quando existe de fato um alvo — aqui, os 100% da meta.

No mapa de pedidos não existe alvo nenhum: 140 pedidos numa sexta à noite não é
"verde", é só um número maior. Pintar aquilo de vermelho e verde inventaria um juízo
que o dado não tem. É a diferença entre *medir* e *avaliar*.

## Vermelho e verde e daltonismo

Vermelho e verde são exatamente o par que a maioria dos daltônicos não separa. Para
o semáforo não depender da cor, cada faixa tem:

- **nome** (Crítico, Abaixo, Atenção, Na meta, Acima) e **limite** explícito na legenda
- **símbolo próprio** (▼ ▽ ◆ △ ▲) impresso dentro da célula
- o **número** escrito na própria célula, mais a tabela com os mesmos valores

Todas as cinco faixas passam de 3:1 de contraste contra o fundo nos dois temas, e o
texto de cada célula passa de 4,5:1 contra a cor da sua faixa.

## Detalhes de implementação

- Arquivo único de HTML/CSS/JS puro, sem nenhuma dependência externa
- As cores de estado são fixas: não mudam entre tema claro e escuro
- Botão **Ver tabela** em cada exemplo
- Tema claro e escuro, seguindo o sistema e com alternância manual
