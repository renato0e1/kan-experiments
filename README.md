# kan-experiments

Redes de Kolmogorov–Arnold: Uma Avaliação Experimental

Autor: Renato França de Almeida - PPGEEC EMC/UFG

Implementação dos experimentos em DRL realizados com MLP (Multilayer Perceptron) e redes derivadas da KAN – FastKAN (Fast Kolmogorov-Arnold Network) e KKAN (Kurková-Kolmogorov-Arnold Network) – utilizando os simuladores LunarLander-v3 e CartPole-v1. Esses notebooks fundamentam a pesquisa desenvolvida no Programa de Pós-graduação em Engenharia Elétrica e de Computação (PPGEEC) da Universidade Federal de Goiás (UFG) que fundamenta Dissertação de Mestrado deste Programa e Artigo Científico submetido ao CBA 2026 - Congresso Brasileiro de Automática (https://sites.usp.br/cba2026/).

_Abstract_: Este trabalho investiga Redes Kolmogorov–Arnold rápidas (FastKAN) e Kurková-Kolmogorov-Arnold (KKAN) como aproximadores de valor-ação em Deep Q-Learning no ambiente LunarLander -v3. A metodologia emprega retorno n-step, exploração ε-greedy, buffer de replay e clipping de gradiente. Enquanto a FastKAN prioriza eficiência, a KKAN utiliza polinômios de Chebyshev para garantir estabilidade espectral e capturar sutilezas da função Q, superando limitações das splines. Resultados indicam que estas derivações KAN proporcionam aprendizado estável, baixo custo computacional e desempenho competitivo. O estudo conclui que tais arquiteturas são promissoras para Aprendizado por Reforço Profundo, unindo interpretabilidade e eficácia na aproximação de funções complexas.


### LunarLander-v3

Notebooks de treinamento individual:
#### LunarLander/LunarLanderMLP_9_18.ipynb
#### LunarLander/LunarLanderFastKAN_10_14.ipynb
#### LunarLander/LunarLanderKKAN_2_16.ipynb

Notebooks de plotagem dos resultados sumarizados:
#### LunarLander/plot/mlp-saida.txt
#### LunarLander/plot/fastkan-saida.txt
#### LunarLander/plot/kkan-saida.txt
#### LunarLander/plot/plot_resultados_1_4_cartpole.ipynb


### CartPole-v1

Notebooks de treinamento individual:
#### CartPole/CartPoleMLP_1_7.ipynb
#### CartPole/CartPoleFastKAN_1_9.ipynb
#### CartPole/CartPoleKKAN_1_7.ipynb

Notebooks de plotagem dos resultados sumarizados:
#### CartPole/plot/mlp-saida.txt
#### CartPole/plot/fastkan-saida.txt
#### CartPole/plot/kkan-saida.txt
#### CartPole/plot/plot_resultados_1_4_cartpole.ipynb


Para gerar o treinamento individual dos modelos, execute nos notebooks principais as etapas (1) a (4) e, para cada semente (42, 160, 198, 254 e 2026), execute (5) Execução e (6) Resultados. 

Para observar os resultados sumarizados das sementes, execute o notebook plot_resultados_1_4_cartpole.ipynb relativo a cada simulador, que fará uso dos respectivos arquivos .txt de saída dos treinamentos individuais.





