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

2023.06.14 Adequando o texto que informa de modo errado a ação do código que vem em seguida (obrigado ao aluno ***Giuliano***, do curso de Data Science, por apontar o problema!) 

**Erro** 

O percentual é pequeno e assim vamos simplesmente excluir os dados ausentes.

**Correção** 

O percentual é pequeno e poderíamos talvez excluir os dados ausentes, mas vamos optar por fazer o *input* dos dados ausentes pelo valor médio.

#### BIG_T4_Knn_CV_GridSearch.ipynb

2023.11.22 Alterado de **hot_encode.categories_** para **list(hot_encode.categories_[0])** 

No hot encode da seção Empregando Valores Categóricos que passou a dar erro. Provável mudança da forma de trabalho das bibliotecas. No formato anterior era empregado uma array e não uma lista. Obrigado ao aluno *Victor* e à professora *Carla Pacheco* por apontarem essa necessidade.

