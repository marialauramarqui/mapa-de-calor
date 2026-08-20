# Mapa de Calor — Pedidos por Dia e Hora

Mapa de calor de volume de pedidos, cruzando **dia da semana × hora do dia** (08h às 21h).

**Todos os dados são fictícios**, gerados só para demonstrar a visualização.

## Ver online

https://marialauramarqui.github.io/mapa-de-calor/

## Como foi feito

- HTML/CSS/JS puro, arquivo único, sem dependências externas
- Escala **sequencial de uma cor só** (azul, claro → escuro): claro = menor volume, escuro = maior
- Valor impresso dentro de cada célula + tooltip no hover — a leitura não depende só da cor
- Botão **Ver tabela** com os mesmos números, para leitura acessível
- Tema claro e escuro (segue o sistema, com alternância manual)
