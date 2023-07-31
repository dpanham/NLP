# Análise de Sentimentos com a Base IMDB

Este repositório apresenta uma análise de sentimentos realizada com uma base de dados do IMDB, que é uma base popularmente conhecida por catalogar informações de filmes e programas de TV. Aqui, nos concentramos em avaliações de filmes feitas por usuários.

## Descrição da Base de Dados

A base de dados contém avaliações de filmes feitas por usuários, onde cada avaliação é classificada como positiva ou negativa. 

🔗 Para mais detalhes sobre a base, você pode acessá-la diretamente no Kaggle através [deste link](https://www.kaggle.com/datasets/luisfredgs/imdb-ptbr).

## Pré-processamento

Atualmente, a base foi utilizada em sua forma crua, sem tratamentos iniciais típicos em processamento de linguagem natural (NLP). Isso inclui etapas como remoção de _stop words_, lematização, correção ortográfica, entre outros. Essas etapas de pré-processamento serão implementadas em futuras atualizações para potencializar a precisão dos modelos de classificação utilizados.

## Abordagem de Modelagem

Para a análise inicial, os textos foram tokenizados gerando o "bag of words". A partir desse formato, dois modelos de classificação foram empregados para prever se uma avaliação foi positiva ou negativa.

Adicionalmente, para avaliar o desempenho do modelo GPT como classificador de sentimento, foi utilizada a API da OpenAI.

## Métrica de Avaliação

O desempenho dos classificadores foi mensurado utilizando a métrica de acurácia. Esta métrica quantifica a proporção de acertos dos modelos em relação ao total de avaliações.

## Considerações Importantes

- A chave de API (`API_KEY`) da OpenAI foi configurada via variável de ambiente. Se você planeja executar o código em seu ambiente local, certifique-se de configurar a `API_KEY` corretamente em seu sistema.
  
- A base de dados encontra-se no repositório, mas foi compactada para otimização de espaço. O arquivo está em formato `.zip` e localizado na pasta `imdb`.

---

Espero que este repositório forneça insights valiosos sobre a análise de sentimentos com a base IMDB! Se tiver dúvidas ou sugestões, sinta-se à vontade para contribuir.
