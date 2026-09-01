# Changelog

## v0.3.1

- Corrigida a troca entre os cinco módulos no aplicativo instalado e no navegador.
- Removidas referências JavaScript aos botões `runMatrix` e `runDSMatrix`, eliminados na v0.3; essas referências interrompiam a execução do script antes do registro dos eventos das abas.
- Removida a execução automática de Deriva genética ao abrir o aplicativo, incompatível com a opção pedagógica de campos sem valores predefinidos.
- Atualizada a constante interna de versão para `0.3.1`.
- Atualizado o cache da PWA para `genpop-sim-v0.3.1`.

## v0.3.0
- Removidos todos os botões de preenchimento automático (presets) associados aos Estudos Dirigidos.
- Removidos os valores numéricos predefinidos dos campos de parâmetros; o estudante deve preencher manualmente os parâmetros antes de simular.
- Removidos também os atalhos/matrizes específicos dos Estudos Dirigidos que executavam combinações de parâmetros automaticamente, evitando exemplos ou valores sugeridos na interface.
- Mantidos os modelos matemáticos, validações, seeds, gráficos, CSVs e demais correções científicas da v0.2.
- Atualizado o cache da PWA para `genpop-sim-v0.3.0`.

# GenPop Sim — Changelog

## v0.2.0 — versão auditada

- Mantida amostragem Wright–Fisher estritamente binomial e exata; `N` passa a ser limitado a 2.000 para evitar a aproximação normal silenciosa usada na v0.1.
- Adicionada validação explícita dos parâmetros de entrada.
- Corrigida a escala do eixo `p` no gráfico de valor adaptativo médio (`W̄ × p`).
- Adicionada escolha entre frequências genotípicas antes e após a seleção por viabilidade.
- Corrigida a condição de parada por absorção no módulo de estrutura quando `m > 0`.
- Seeds agora são geradas e exibidas automaticamente quando o campo é deixado vazio.
- Matrizes `N × migração` e `N × seleção` passam a usar seed reprodutível.
- A matriz seleção + deriva passa a informar fixações, perdas, manutenção e geração média de fixação.
- Corrigido o cálculo/relato de `W̄` final no módulo multialélico.
- CSVs ampliados com metadados, parâmetros, seed e resultados adicionais.
- Valores adaptativos multialélicos passam a impedir entradas negativas.
- Cache PWA atualizado para `genpop-sim-v0.2.0`.

## Nota sobre FST

O módulo calcula `FST = (HT - HS) / HT` diretamente a partir das frequências populacionais simuladas, com demes igualmente ponderados. Não se trata de um estimador amostral como Weir & Cockerham; valores negativos associados a estimadores empíricos não são modelados.
