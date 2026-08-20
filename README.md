# Mapas de Calor — exemplos

Dois mapas de calor **na mesma página**, mostrando duas formas diferentes de
desenhar a mesma ideia.

**Todos os dados são fictícios**, gerados só para demonstrar as visualizações.

## Ver online

https://marialauramarqui.github.io/mapa-de-calor/

| Exemplo | O que mostra | Como codifica o valor |
|---|---|---|
| Pedidos por dia da semana e hora | volume de pedidos, dia × hora (08h–21h) | **cor da célula** — escala sequencial, claro → escuro |
| Peças vendidas por categoria e mês | quantidade vendida, categoria × mês | **tamanho da bolinha** — área proporcional ao valor |

## Quando usar cada um

- A **célula colorida** preenche a grade inteira, então funciona bem para enxergar
  blocos e faixas — o padrão salta aos olhos mesmo de longe.
- A **bolinha** deixa o fundo respirar e compara valores individuais com mais
  precisão, porque o olho lê diferença de tamanho melhor do que diferença de tom.
  Em compensação, os padrões amplos ficam menos evidentes.

Regra prática: *densidade* pede célula, *comparação ponto a ponto* pede bolinha.

## Detalhes de implementação

- Arquivo único de HTML/CSS/JS puro, sem nenhuma dependência externa
- Na bolinha, o **diâmetro é proporcional à raiz quadrada** do valor — é a área que
  precisa ser proporcional, não o diâmetro; usar o diâmetro direto exageraria as
  diferenças
- Todas as bolinhas têm a mesma cor: quem carrega o valor é o tamanho, então gastar
  a cor também seria redundante
- Botão **Ver tabela** em cada exemplo, com os mesmos números — a leitura nunca
  depende só do desenho
- Tema claro e escuro, com paleta própria para cada um, seguindo o sistema e com
  alternância manual
