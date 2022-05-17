# eBook Errata

Você encontra aqui no GitHub as correções já efetuadas.

#### BIG_T3_Classificacao_e_Metricas.ipynb

2022.05.17 Erro no cálculo direto de precisão e recall divergindo do classification_report do scikit-learn. (obrigado ao aluno *Marcos Torres* por apontar o problema)

**Erro**

> TP, **FP, FN,** TN = cm.ravel()

**Correção** 

> TP, **FN, FP,** TN = cm.ravel()

