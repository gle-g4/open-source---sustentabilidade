# 🌿 Rastro Clima

> Calculadora de pegada de carbono pessoal interativa, adaptada ao contexto e às referências do Brasil.

[![Acesse a Aplicação](https://img.shields.io/badge/🚀_Acesse_o_projeto-GitHub_Pages-2e7d32?style=for-the-badge)](https://gle-g4.github.io/open-source---sustentabilidade/)
[![Licença](https://img.shields.io/badge/Licen%C3%A7a-MIT-blue.svg?style=for-the-badge)](#-licença)
[![No Dependencies](https://img.shields.io/badge/Depend%C3%Aancias-Nenhuma-success?style=for-the-badge)](#-tecnologias)

---

## 📌 Sobre o Projeto

O **Rastro Clima** é uma ferramenta simples, visual e direta para conscientização ambiental. Com base em hábitos do dia a dia, a aplicação estimativa a quantidade de dióxido de carbono equivalente ($\text{CO}_2\text{e}$) emitida anualmente por uma pessoa no Brasil.

- 🌐 **Online e sem instalação:** Roda diretamente no navegador via [GitHub Pages](https://gle-g4.github.io/open-source---sustentabilidade/).
- ⚡ **Zero dependências:** Construído com tecnologia Web padrão (HTML, CSS e JS puros).
- 🎨 **Design cuidadoso:** Interface responsiva com o tema *"Atlas Botânico"* (tons de marfim e verde escuro, tipografia refinada).

---

## ✨ Funcionalidades

- **Cálculo em tempo real:** O painel de resultados é atualizado instantaneamente conforme você altera as respostas.
- **Formulário categorizado:** Avaliação dividida em 4 pilares do cotidiano:
  - 🚗 **Mobilidade:** Quilometragem semanal de carro e transporte público, além de voos anuais.
  - 💡 **Energia:** Consumo médio de eletricidade ($\text{kWh/mês}$) e número de moradores na residência.
  - 🥗 **Alimentação:** Padrão de dieta (do veganismo ao alto consumo de carne vermelha).
  - ♻️ **Resíduos:** Nível de separação e destinação de materiais recicláveis.
- **Atalhos de Perfil:** Preenchimento rápido com um clique para perfis típicos:
  - *Urbano sem carro*
  - *Rotina média brasileira*
  - *Casa com carro*
- **Comparativo com a Média Nacional:** Gráficos e indicadores que comparam seu resultado direto com a média do brasileiro (~2,2 t $\text{CO}_2\text{e}$/ano).

---

## 🚀 Como Executar Localmente

Como o projeto é contido em um **único arquivo estático**, você não precisa do Node.js, gerenciadores de pacote ou servidor web.

1. Clone ou baixe este repositório:
   ```bash
   git clone [https://github.com/GLE-G4/open-source---sustentabilidade.git](https://github.com/GLE-G4/open-source---sustentabilidade.git)

```

2. Navegue até a pasta do projeto e abra o arquivo `index.html` em qualquer navegador (Chrome, Firefox, Edge, Safari).

---

## 📊 Metodologia e Fatores de Emissão

> **Nota:** Os fatores utilizados são aproximações com fins **educativos e de conscientização**, não constituindo um inventário de emissões oficial (como o *GHG Protocol*).

A matriz energética brasileira possui particularidades (como a predominância da fonte hídrica na eletricidade), que foram consideradas no modelo:

| Categoria | Parâmetro | Fator de Emissão Adotado |
| --- | --- | --- |
| **Transporte Individual** | Carro a gasolina/flex | `0,19 kg CO₂e / km` |
| **Transporte Coletivo** | Ônibus / Metrô | `0,06 kg CO₂e / km` |
| **Energia Elétrica** | Matriz Brasileira | `0,08 kg CO₂e / kWh` |
| **Aviação** | Viagens aéreas | `250 kg` a `1.400 kg CO₂e / ano` |
| **Alimentação** | Dieta (Vegana a Carnívora) | `650 kg` a `2.100 kg CO₂e / ano` |
| **Resíduos** | Destinação do lixo | `90 kg` a `320 kg CO₂e / ano` |

*Caso deseje ajustar ou personalizar esses valores, todos os parâmetros estão declarados de forma legível e comentada no bloco `<script>` do `index.html` sob as variáveis `FACTOR_*` e `*_KG`.*

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura semântica e acessível.
* **CSS3:** Estilização com CSS Variables, Flexbox/Grid e layout responsivo.
* **JavaScript (ES6+):** Lógica de cálculo, manipulação de DOM e reatividade sem frameworks.

---

## 🤝 Como Contribuir

Contribuições são super bem-vindas! Se você tem ideias para melhorar a precisão das estimativas, a acessibilidade do código ou a interface:

1. Faça um **Fork** do projeto.
2. Crie uma branch para a sua funcionalidade (`git checkout -b feature/nova-funcionalidade`).
3. Faça o **Commit** das suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Faça o **Push**Aqui está uma versão aprimorada do **README.md** para o projeto **Rastro Clima**. Ela foi reestruturada para tornar o repositório mais profissional, atraente e organizado no GitHub, destacando badges de status, recursos principais, captura de tela/link direto e instruções claras para novos contribuidores.

---

```markdown
# 🍃 Rastro Clima

> **Calculadora de pegada de carbono pessoal baseada no contexto e referências brasileiras.**

[![GitHub Pages](https://img.shields.io/badge/demo-online-brightgreen?style=flat-square&logo=github)](https://gle-g4.github.io/open-source---sustentabilidade/)
[![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-blue.style=flat-square)](LICENSE)
[![Zero Dependencies](https://img.shields.io/badge/depend%C3%AAncias-nenhuma-orange?style=flat-square)](index.html)

**[🔗 Acesse a aplicação online](https://gle-g4.github.io/open-source---sustentabilidade/)**

---

## 📌 Sobre o Projeto

O **Rastro Clima** é uma ferramenta web simples, acessível e educativa projetada para estimar a pegada individual de carbono (em **toneladas de CO₂e/ano**) com base nas particularidades do consumo e da matriz energética do Brasil.

Desenvolvido em página única (vanilla HTML/CSS/JS), o projeto não exige backend, compilação ou instalação de pacotes — tornando o código leve, rápido e fácil de estudar ou modificar.

---

## ✨ Funcionalidades

- **Cálculo em Tempo Real:** O painel lateral reage instantaneamente a cada campo alterado.
- **4 Pilares do Consumo Individual:**
  - **🚗 Mobilidade:** Quilometragem semanal em carro/transporte público e voos anuais.
  - **⚡ Energia:** Consumo médio de eletricidade (kWh/mês) proporcional ao número de moradores.
  - **🥗 Alimentação:** Padrões alimentares (de dieta vegana até alto consumo de carne).
  - **♻️ Resíduos:** Grau de separação e destinação de materiais recicláveis.
- **Perfis Pré-definidos:** Atalhos de um clique para simulação rápida (*Urbano sem carro*, *Rotina média*, *Casa com carro*).
- **Benchmarking Nacional:** Comparativo visual com a média brasileira de emissões (~2,2 t CO₂e/pessoa/ano).
- **Design "Atlas Botânico":** Interface limpa, responsiva e acessível com paleta em tons terrosos e tipografia serifada/sans.

---

## 🔬 Metodologia e Fatores de Emissão

Os cálculos utilizam aproximações educativas alinhadas ao contexto nacional (como o fator da matriz elétrica predominantemente renovável do Brasil):

| Categoria | Fator / Parâmetro de Referência |
|---|---|
| **Carro individual** | `0.19 kg CO₂e / km` |
| **Transporte Público** | `0.06 kg CO₂e / km` |
| **Energia Elétrica (SIN)** | `0.08 kg CO₂e / kWh` (Matriz hídrica/renovável) |
| **Viagens Aéreas** | `250 kg` a `1.400 kg CO₂e / ano` (conforme distância e frequência) |
| **Dieta Alimentar** | `650 kg` a `2.100 kg CO₂e / ano` (de vegano a carnívoro intensivo) |
| **Gestão de Resíduos** | `90 kg` a `320 kg CO₂e / ano` (conforme nível de reciclagem) |

> 💡 **Quer personalizar as constantes?** Todos os coeficientes estão centralizados e documentados no topo do script JavaScript dentro de `index.html` sob as variáveis `FACTOR_*` e `*_KG`.

---

## 🚀 Como Executar Localmente

Como a aplicação é composta por arquivos estáticos sem dependências externas:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/gle-g4/open-source---sustentabilidade.git

```

2. **Abra a aplicação:**
Basta dar um duplo clique no arquivo `index.html` ou abri-lo diretamente em qualquer navegador moderno.

---

## 📂 Arquitetura do Código

A aplicação adota a simplicidade de um **Single File Component (SFC)** sem builds:

```text
.
└── index.html
    ├── CSS (<head>)      -> Design system "Atlas Botânico" (Grid, CSS Vars, Responsividade)
    ├── HTML (<body>)     -> Formulário e Dashboard de resultados
    └── JS (</html>)      -> Regras de cálculo, atalhos de perfil e atualização da DOM

```

---

## 🤝 Como Contribuir

Contribuições para ajustar os fatores de emissão, incluir novos perfis de consumo ou melhorar a acessibilidade da interface são muito bem-vindas!

1. Faça um **Fork** do projeto
2. Crie uma **Branch** para sua modificação (`git checkout -b feature/nova-funcionalidade`)
3. Faça **Commit** das alterações (`git commit -m 'Adiciona novo fator de emissão para biofórmulas'`)
4. Envie para o GitHub (`git push origin feature/nova-funcionalidade`)
5. Abra um **Pull Request**

---

## 📄 Licença

Este projeto está sob a licença [MIT](https://www.google.com/search?q=LICENSE) — sinta-se livre para usar, modificar e distribuir.

```

---

### Principais melhorias aplicadas:
1. **Badges informativos:** Adicionados no topo para dar um visual moderno de repositório open-source mantido.
2. **Link de Acesso Rápido:** Destacado no início para quem quer testar sem ler tudo.
3. **Seção de Funcionalidades:** Uso de ícones e tópicos claros para facilitar a leitura rápida (*scannability*).
4. **Instruções de Contribuição:** Adicionado um guia simples de Pull Request para incentivar outros desenvolvedores a colaborarem.
5. **Formatação e Estrutura:** Melhor organização dos títulos (H1, H2, H3) e blocos de código formatados.

```
