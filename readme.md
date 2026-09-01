# Rastro Clima

Calculadora de pegada de carbono pessoal, com referências brasileiras.

## Como usar

Abra o arquivo `index.html` em qualquer navegador. Não precisa de servidor, build ou instalação — é uma página única (HTML + CSS + JS).

## O que ela faz

Você preenche um formulário com 4 blocos:

- **Mobilidade** — km de carro e transporte público por semana, voos por ano
- **Energia** — consumo médio de luz (kWh/mês) e moradores na casa
- **Alimentação** — padrão alimentar (de vegano a carnívoro)
- **Resíduos** — nível de separação de recicláveis

O painel à direita atualiza em tempo real: total estimado em toneladas de CO₂e/ano, comparação com a média nacional (2,2 t/pessoa/ano) e detalhamento por categoria.

Há também 3 atalhos de perfil (urbano sem carro, rotina média, casa com carro) para preencher tudo de uma vez.

## Metodologia

Os fatores de emissão usados são aproximações educativas, não um inventário oficial:

| Área | Fator |
|---|---|
| Carro | 0,19 kg CO₂e/km |
| Transporte público | 0,06 kg CO₂e/km |
| Eletricidade | 0,08 kg CO₂e/kWh (matriz majoritariamente hídrica) |
| Voos | 250–1.400 kg/ano conforme frequência/distância |
| Dieta | 650–2.100 kg/ano conforme padrão |
| Resíduos | 90–320 kg/ano conforme separação |

Todos os valores estão comentados no `<script>` do `index.html`, em `FACTOR_*` e `*_KG`, caso queira ajustá-los.

## Estrutura do arquivo

Tudo em um único `index.html`:
- CSS no `<head>` (tema "Atlas Botânico": marfim, verde escuro, serifada + sans)
- HTML da página
- JavaScript no fim do `<body>`, sem dependências externas
