Tarefa 1: Análise Descritiva e Transformação da Variável Resposta
A primeira etapa focou em tornar a variável resposta (renda) mais adequada para modelos lineares, que possuem pressupostos de normalidade e homocedasticidade.
1. Estrutura de Correlação Inicial
Matriz de Correlação: A correlação inicial foi examinada para variáveis quantitativas (idade, tempo_emprego, qt_pessoas_residencia, renda).
Identificação: A variável tempo_emprego demonstrou ser a mais correlacionada com renda.

2. Tratamento de Outliers e Assimetria
Problema: A variável renda exibia uma distribuição altamente assimétrica (concentração na cauda inferior e outliers na cauda superior), o que violaria os pressupostos de um modelo de regressão linear.
Solução: Foi aplicada a Transformação Logarítmica Natural ($\mathbf{Log(Renda) = \ln(Renda)}$).
Resultado: A transformação logarítmica estabilizou a variância e reduziu a assimetria, resultando em uma distribuição mais próxima do ideal para a modelagem.

Tarefa 2: Anáise Inferencial e Poder Preditivo
Esta etapa utilizou a Inferência Estatística para verificar se a diferença de $Log(\text{Renda})$ entre os grupos (quem possui vs. quem não possui) é estatisticamente significante.
1. Metodologia: Intervalo de Confiança (IC 95%)
Para cada grupo (True/False de posse de imóvel/veículo), calculou-se a média do $Log(\text{Renda})$ e seu respectivo Intervalo de Confiança de 95%. O cálculo dependeu diretamente do Erro Padrão (EP).
A amostra grande ($N \approx 15.000$) resultou em um EP muito pequeno, conferindo alta precisão às estimativas.
Em ambos os casos (posse_de_imovel e posse_de_veiculo), o IC 95% dos grupos True e False não se sobrepôs.
Inferência: A diferença de renda observada é estatisticamente significante ($\alpha = 0.05$). Rejeitamos a hipótese nula de que a média de renda é igual entre os grupos.

Tarefa 3: Análise de Estabilidade Temporal
Estabilidade Temporal: As médias de $Log(\text{Renda})$ para cada grupo (ex: True) permaneceram estáveis (linhas horizontais) ao longo dos meses. Os ICs mensais se sobrepuseram, confirmando a estabilidade.
Diferença Consistente: A diferença entre os grupos (True vs. False) permaneceu estatisticamente significativa em todos os meses (ICs não se sobrepõem), mantendo o alto poder preditivo.
As relações preditivas são extremamente estáveis, o que confere alta confiança na longevidade e na manutenção da performance do futuro modelo de previsão de renda.



