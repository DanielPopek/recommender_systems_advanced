# Recommender systems advanced

#### O projekcie
Repozytorium zawiera implementacje oraz porównanie czterech modeli sytemów rekomendacyjnych:
* Model oparty o klasteryzację **K-means**
* Model **Bayesian Personalized Ranking** wykorzystujący informacje o akcjach użytkowników
* Model sekwencyjny 
* Model **MLP** wykorzystujący sieci głębokie

#### Prezentacja
Tutaj znajduje się link do prezentacji: https://docs.google.com/presentation/d/1C7cNc14DFr3N2ksRQBIT2nhdkYzMKQsg0CSbdkqOnIs/edit?fbclid=IwAR0BFHT_GvkQZ2JZWu6kQuWgNDyCNNeBwzKgx30RGhhgXvzOysdXY-PbvyA#slide=id.g7f498dcb5a_8_56

#### Zbiór danych
Jako zbiór danych wykorzystano zbiór danych MovieLens zawieracjący 100 000 ocen (1-5) od 943 
użytkowników dla 1682 filmów. Każdy użytkownik ma co najmniej 20 ocenionych filmów.

#### Metoda ewaluacji
Do ewaluacji zaimplementowanych modeli wykorzystano strategie leave-one-out oraz metryki Hit Ratio *(HR)* i 
Normalized Discounted Cumulative Gain *(NDCG)*.

#### Wyniki ewaluacji modeli

Metryka\Model | K-means | BPR | Sequential | MLP
--------------|---------|-----|------------|----
HR | 0.1463 | 0.6214 | 0.1962 | 0.5705
NDCG| 0.0587 | 0.3461 | 0.1008 | 0.3107

#### Powiązane publikacje
1. [MLP model](https://www.comp.nus.edu.sg/~xiangnan/papers/ncf.pdf)
2. [Implicit BPR recommender](https://medium.com/radon-dev/implicit-bayesian-personalized-ranking-in-tensorflow-b4dfa733c478)
