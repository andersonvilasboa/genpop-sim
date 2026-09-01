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
