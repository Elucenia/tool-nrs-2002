<!-- ELUCENIA technical documentation · nrs-2002 · pt-BR · no clinical/professional/rights approval -->

# NRS-2002

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/nrs-2002)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Prejuízo do estado nutricional

`estado`

- `0` — Ausente: estado nutricional normal
- `1` — Leve: perda de peso \> 5% em 3 meses ou ingestão de 50 a 75% da necessidade na última semana
- `2` — Moderado: perda \> 5% em 2 meses, ou IMC 18,5 a 20,5 com estado geral comprometido, ou ingestão de 25 a 60%
- `3` — Grave: perda \> 5% em 1 mês (\> 15% em 3 meses), ou IMC \< 18,5 com estado geral comprometido, ou ingestão de 0 a 25%

### Gravidade da doença (aumento das necessidades)

`gravidade`

- `0` — Ausente: necessidades nutricionais normais
- `1` — Leve: fratura de quadril, doença crônica com complicação aguda (cirrose, DPOC, hemodiálise, diabetes, câncer)
- `2` — Moderada: cirurgia abdominal de grande porte, AVC, pneumonia grave, neoplasia hematológica
- `3` — Grave: traumatismo craniano, transplante de medula óssea, UTI com APACHE II \> 10

### Idade ≥ 70 anos

`idade`

## Edição do método

NRS 2002/ESPENKondrup 2003:2 domínios 0–3, idade≥70+1, total 0–7

## Fórmula documentada

Escore = prejuízo do estado nutricional (0 a 3) + gravidade da doença (0 a 3) + 1 ponto se idade ≥ 70 anos. Total de 0 a 7.

Escore ≥ 3: risco nutricional.

## Limites e população

O NRS-2002 é triagem de risco baseada na combinação de estado nutricional e gravidade da doença. Seu desenvolvimento discriminou grupos de estudos com maior probabilidade de benefício; um total não garante resposta individual nem prescreve via ou dose de suporte nutricional. Definições, elegibilidade e idade devem corresponder à versão.

## Referências

- [Kondrup J et al. Nutritional risk screening (NRS 2002): a new method based on an analysis of controlled clinical trials. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(02)00214-5)

- [Kondrup J et al. ESPEN guidelines for nutrition screening 2002. Clin Nutr, 2003.](https://doi.org/10.1016/S0261-5614(03)00098-0)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
