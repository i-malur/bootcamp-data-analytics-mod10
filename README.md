# Correlação e Regressão

## Cenário
Trabalhamos em uma empresa de revenda de veículos usados. O sucesso da empresa depende fortemente da precificação adequada dos veículos. Caso o preço seja muito alto, o carro não vende. Se for muito baixo, a empresa perde dinheiro. Como parte da equipe de dados, recebemos uma base de dados com informações sobre carros vendidos nos últimos anos, com o objetivo de entender quais fatores mais impactam no preço de venda. A empresa espera que identifiquemos as variáveis mais relevantes e proponha uma análise baseada em correlações e modelos preditivos simples.

## Variáveis
* id: Identificador único do veículo
* make: Marca do carro (ex: Ford, Toyota)
* model: Modelo do carro
* year: Ano de fabricação
* price: Preço de venda do carro
* mileage: Quilometragem (km rodados)
* engine_size: Tamanho do motor (em litros)
* fuel_type: Tipo de combustível (gasolina, diesel, elétrico)
* transmission: Tipo de transmissão (manual, automática)
* doors: Número de portas
* color: Cor do carro
* tax: Taxa anual de imposto veicular
* mpg: Milhas por Galão(indicador de eficiência de combustível)
* sold_date: Data de venda do veículo

### Variáveis renomeadas
```py
df_carros = df_carros.rename(columns={
    'id': 'id',
    'make': 'marca',
    'model': 'modelo',
    'year': 'ano',
    'price': 'preco',
    'mileage': 'quilometragem',
    'engine_size': 'tamanho_motor',
    'fuel_type': 'tipo_combustivel',
    'transmission': 'transmissao',
    'doors': 'portas',
    'color': 'cor',
    'tax': 'imposto',
    'mpg': 'consumo_mpg',
    'sold_date': 'data_venda'
})
```

## Questões
1. Análise de Correlação
* Calcule a correlação entre as variáveis numéricas e o preço do carro
(price).
* Quais variáveis estão mais correlacionadas com o preço?
* Quais estão menos correlacionadas?
  
2. Análise das 5 Variáveis Mais Correlacionadas   
Para as cinco variáveis com maior correlação com o preço:
* Plote histograma e boxplot de cada variável.
* Plote o scatterplot (gráfico de dispersão), com price no eixo Y e a
variável no eixo X.
* Faça uma regressão linear simples, utilizando cada variável como
preditora (X) e o preço como resposta (Y). Interprete os coeficientes e
o R².

## Tecnologias usadas:
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)

```py
print('Feito com carinho 🌹')
```

