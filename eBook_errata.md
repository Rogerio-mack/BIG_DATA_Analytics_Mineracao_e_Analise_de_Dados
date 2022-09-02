# eBook Errata

Você encontra aqui no GitHub as correções já efetuadas.

#### BIG_T3_Classificacao_e_Metricas.ipynb

2022.05.17 Erro no cálculo direto de precisão e recall divergindo do classification_report do scikit-learn. (obrigado ao aluno *Marcos Torres* por apontar o problema)

**Erro**

> TP, **FP, FN,** TN = cm.ravel()

**Correção** 

> TP, **FN, FP,** TN = cm.ravel()


#### BIG_T4_Knn_CV_GridSearch.ipynb

2022.05.20 Erro no texto da conclusão do segundo exemplo de Knn, Empréstimos *Default Yes/No*. Após a normalização o resultado muda para *conceder* o empréstimo. (obrigado à *profa. Carla Pacheco* por apontar o problema)

**Erro**

> Como você pode ver o resultado agora é outro e a classe prevista do empréstimo será *Default Yes* (zeros), com probabilidade de $2/3$ e, portanto, **não** deveríamos conceder esse empréstimo.  

**Correção** 

> Como você pode ver o resultado agora é outro e a classe prevista do empréstimo será *Default Yes* (zeros), com probabilidade de $2/3$ e, portanto, deveríamos conceder esse empréstimo.  

#### BIG_T4_Knn_CV_GridSearch.ipynb

2022.09.02 Acrescentada a **Nota Técnica:** *Normalizar com X ou X_train* esclarecendo o uso mais correto dos procedimentos de normalização e a simplificação empregada nos exemplos do livro (obrigado à *profa. Carla Pacheco* por apontar essa necessidade).
