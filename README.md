# Mapas de Calor — exemplos

Dois mapas de calor em HTML puro, cada um demonstrando um **tipo diferente de escala de cor**.

**Todos os dados são fictícios**, gerados só para demonstrar as visualizações.

## Ver online

| Exemplo | O que mostra | Escala |
|---|---|---|
| [Volume por dia e hora](https://marialauramarqui.github.io/mapa-de-calor/) | pedidos por dia da semana × hora (08h–21h) | **sequencial** — uma cor só, claro → escuro |
| [Variação por categoria](https://marialauramarqui.github.io/mapa-de-calor/variacao.html) | variação % do faturamento vs. ano anterior, por categoria × mês | **divergente** — duas cores + cinza neutro no zero |

## Por que duas escalas diferentes

- **Sequencial** é para *magnitude*: só existe "mais" e "menos", o zero não é especial.
  Uma cor só, variando em claridade. Rainbow nunca.
- **Divergente** é para *polaridade*: existe um lado bom e um lado ruim de um valor de
  referência (aqui, o zero). Duas cores opostas com um **cinza neutro** no meio — o meio
  precisa parecer "nada", por isso não leva cor.

## Detalhes de implementação

- HTML/CSS/JS puro, um arquivo por exemplo, sem nenhuma dependência externa
- O valor é impresso **dentro de cada célula** e repetido no tooltip do hover
- Botão **Ver tabela** com os mesmos números — a leitura nunca depende só da cor
- Tema claro e escuro, com paleta própria para cada um (não é inversão automática),
  seguindo o sistema e com alternância manual
