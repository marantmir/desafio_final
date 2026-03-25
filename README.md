<p align="center">
  <img src="imgs/app_docker.png" width="500" height="450">
  <img src="imgs/app_streamlit.png" width="500" height="450">
</p>

# Projeto Acadêmico de Previsão de Preços de Carro

Este projeto visa prever o preço de carros com base em diversas características. A previsão é realizada usando técnicas de aprendizado de máquina, onde foi construido um modelo preditivo treinado em um conjunto de dados relevante.

## Características do Projeto
- **Modelo:** Utiliza algoritmos de aprendizado de máquina como regressão linear, árvore de decisão, entre outros.
- **Dados:** Dados que incluem características dos carros como ano, modelo, quilometragem, e muito mais.
- **Resultados:** O modelo fornece previsões de preços com métricas de desempenho como MAE, RMSE.

## Desenvolvimento

### Análise Exploratória

A primeira etapa desse projeto foi a análise exploratória dos dados, onde identificou a existência de dados ausentes, dados com valores extremos (outliers) e dados indevidos com a coluna onde foi encontrado. Nessa foram identificados padrões de valores de venda em função das colunas de dados existentes.

### Modelagem

Ao final dessa etapa o dataset gerado foi salvo e se iniciou a etapa de modelagem.
Nessa etapa os dados deverão ser tratados para que o modelo possa usar no treinamento e a avaliação seja feita.
Foram treinados e avaliados 7 modelos de reggressão.
Foram geradas 4 métricas e mais duas colunas com informações geradas durante o treinamento.
Um dataset com todos treinamentos, métricas e dados gerados é apresentado no final.
O GrdidSearch foi aplicado ao melhor modelo para identificar os melhores hiperparametros.

#### Deploy

Foi implementada uma aplicação web com a lib Streamlit. A aplicação esta hospedada no site streamlit.io.
Acesso: [🔗 Desafio Final Previsao de Valor de Carro](https://desafiofinal.streamlit.app/)

#### Docker

A mesma aplicação pode ser executada localmente na linha do terminal através do streamlit ou através do docker que foi implementado. Para sua execução é preciso ter o Docker Desktop instalado no seu ambiente.

Esta implementação fez  uso da lib FastAPI, onde um servidor espera requisitos POST na porta 8000 e devolve os valores previstos para os dados obtidos numa interface web do Streamlit.



## Como Executar o Projeto
1. Clone o repositório:
```bash
git clone https://github.com/silviolima07/desafio_final.git
```
2. Navegue até o diretório do projeto:
```bash
cd desafio_final
```
3. Instale as dependências:
```bash
pip install -r requirements.txt
```
4. Execute o app.py do streamlit para rodar localmente:
```bash
streamlit run app.py
```
5. Ou acesse o app ja implementado na cloud do Streamlit.io:
[🔗 Desafio Final Previsao de Valor de Carro](https://desafiofinal.streamlit.app/)

7. Pode também usar a imagem docker criada, antes abra o docker desktop local:
```bash
docker-compose up --build
```


## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou relatar problemas.

## Licença
Este projeto está sob a licença MIT.
