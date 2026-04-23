# Análise de Inadimplência em Cartões de Crédito

## Descrição do Projeto
Este projeto analisa o comportamento de clientes para identificar padrões associados à inadimplência e gerar insights estratégicos aplicáveis à gestão de risco e prevenção de perdas. A análise demonstra como o uso do crédito e o ciclo de vida do cliente influenciam o risco de default, provando que o comportamento é, muitas vezes, mais preditivo que a renda isolada.

## Objetivos
- Identificar fatores demográficos e financeiros associados à inadimplência;

- Avaliar a eficiência da concessão de limites vs. o uso real do cartão;

- Gerar recomendações práticas para políticas de crédito e modelos de risco.

## Metodologia e Ferramentas
- Utilizando Python (Pandas, NumPy, Seaborn e Matplotlib), a análise foi conduzida em etapas:

- Limpeza e Exploração: Tratamento de dados e análise de variáveis isoladas.

- Análise Cruzada: Correlação entre Faixa Etária, Salário e Taxas de Inadimplência.

- Comportamento de Uso: Avaliação da relação entre Limite de Crédito e Volume de Transações.

- Consolidação: Geração de insights para tomada de decisão de negócio.

## Principais Insights (Findings)
### 1. O Paradoxo do Risco: Idade vs. Renda
Segmento Resiliente: Jovens (até 35 anos) com renda média ($40K - $60K) representam o menor risco da carteira, com apenas 9% de inadimplência.

O Ponto de Atenção: O maior risco está concentrado no público 55+ com alta renda ($120K+), onde a taxa de inadimplência atinge 20%, desafiando modelos que associam automaticamente alta renda a baixo risco.

Sinal de Alerta: A ausência de dados cadastrais (renda "na") correlaciona-se diretamente com um risco elevado (>18%).

### 2. Comportamento e Eficiência de Crédito
Exposição Ineficiente: Identificamos clientes de alto risco com limites elevados (>$30.000) que realizam poucas transações. Isso indica capital imobilizado com alta exposição desnecessária.

Estresse Financeiro: Clientes com limites baixos, mas alta frequência de uso (>100 transações/ano), mostram sinais de superendividamento.

Interação com o Banco: O número de contatos e interações é o sinal comportamental mais forte; inadimplentes tendem a usar menos o produto antes do default ou apresentar sinais de estresse em múltiplos canais.

## Recomendações Estratégicas
Refinamento de Modelos: Incorporar variáveis comportamentais e idade como pesos negativos para limites agressivos em perfis seniores.

Fidelização Estratégica: Priorizar a expansão de crédito e retenção no público jovem de classe média ($40K-$60K), o grupo de maior fidelidade e pagamento.

Otimização de Limites: Reduzir limites ociosos de clientes no grupo de risco para melhorar os indicadores de PDD (Provisão para Devedores Duvidosos).

Enriquecimento Cadastral: Mitigar o volume de dados não informados para reduzir pontos cegos na análise de risco.

## Conclusão
Modelos tradicionais baseados apenas em dados cadastrais são insuficientes. A verdadeira inteligência de crédito reside na incorporação de variáveis comportamentais (frequência de uso, histórico de transações e interações), permitindo antecipar riscos de forma mais precisa e rentável.
