# Mapas de Calor — exemplos

Dois mapas de calor **na mesma página**, cada um demonstrando um tipo diferente
de escala de cor.

**Todos os dados são fictícios**, gerados só para demonstrar as visualizações.

## Ver online

https://marialauramarqui.github.io/mapa-de-calor/

| Exemplo | O que mostra | Escala |
|---|---|---|
| Pedidos por dia da semana e hora | volume de pedidos, dia × hora (08h–21h) | **sequencial** — uma cor só, claro → escuro |
| Variação do faturamento por categoria | variação % vs. ano anterior, categoria × mês | **divergente** — duas cores + cinza neutro no zero |

## Por que duas escalas diferentes

- **Sequencial** é para *magnitude*: só existe "mais" e "menos", o zero não é especial.
  Uma cor só, variando em claridade. Rainbow nunca.
- **Divergente** é para *polaridade*: existe um lado bom e um lado ruim de um valor de
  referência (aqui, o zero). Duas cores opostas com um **cinza neutro** no meio — o meio
  precisa parecer "nada", por isso não leva cor.

## Detalhes de implementação

- Arquivo único de HTML/CSS/JS puro, sem nenhuma dependência externa
- O valor é impresso **dentro de cada célula** e repetido no tooltip do hover
- Botão **Ver tabela** em cada exemplo, com os mesmos números — a leitura nunca
  depende só da cor
- Tema claro e escuro, com paleta própria para cada um (não é inversão automática),
  seguindo o sistema e com alternância manual
