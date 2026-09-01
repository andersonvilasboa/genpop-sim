GenPop Sim v0.3.1 — versão auditada

Simulador didático de Genética de Populações, executado localmente no navegador e instalável como PWA.

Correções principais da v0.3:
- Amostragem Wright–Fisher mantida estritamente binomial e exata; N limitado a 2000 para preservar exatidão e desempenho.
- Validação explícita de N, gerações, frequências, taxas de migração e valores adaptativos.
- Correção do eixo p no gráfico de valor adaptativo médio (Wbar).
- Opção de visualizar frequências genotípicas antes ou após a seleção por viabilidade.
- Correção da condição de absorção do módulo de estrutura quando m > 0: a simulação só encerra em fixação global de A ou a.
- Seeds passam a ser geradas e exibidas automaticamente quando o campo é deixado vazio, permitindo reprodução das simulações.
- Matrizes N x migração e N x seleção também usam seed reprodutível.
- Matriz seleção + deriva informa fixação, perda e manutenção, além da geração média de fixação.
- Correção do Wbar final no módulo multialélico.
- CSVs ampliados com metadados e resultados adicionais.
- Cache do service worker atualizado para v0.3.1.

Nota científica sobre FST:
O módulo calcula FST teórico a partir de HS e HT nas populações simuladas, com demes igualmente ponderados. Ele não implementa um estimador amostral como Weir & Cockerham; portanto, valores negativos de estimadores empíricos não são esperados neste módulo.


ALTERAÇÃO PEDAGÓGICA v0.3
Os parâmetros numéricos não são preenchidos automaticamente nem apresentados como exemplos. O estudante deve interpretar a atividade e inserir manualmente os valores solicitados.


CORREÇÃO v0.3.1
- Corrigida a navegação entre módulos após a remoção dos botões de matrizes/presets.
- Removidas referências JavaScript a botões inexistentes, que interrompiam a inicialização da interface.
- Removida a simulação automática ao abrir o aplicativo, pois os campos agora exigem preenchimento manual.
- Metadados internos atualizados para v0.3.1.
