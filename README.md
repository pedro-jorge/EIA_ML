por

# **Prediction of Residential Energy Consumption Using Machine Learning**

## Resumo

Esse trabalho utiliza modelos clássicos de aprendizado de máquina, Random Forest e Gradient Boost, na predição do consumo residencial de energia nos EUA a partir de informações de dados geográficos, de demanda e de preço, levando em consideração a interpretabilidade. O melhor resultado individual é utilizando Random Forest sem dados temporais, com RMSE 56.73 e R² 0.97.

Todo o trabalho pode ser reproduzido rodando o arquivo `main.ipynb`, um Jupyter Notebook com todos o passo a passo e comentários do que foi feito.

---

## Objetivos

- Executar a predição do consumo residencial de energia;
- Comparar Random Forest e Gradient Boost;
- Identificar a interpretabilidade desses modelos;
- Comparar com uma abordagem de rede neural Multilayer Perceptron.

---

### Fontes de dados (`data/`)

| Arquivo                                                     | Descrição                                                                                            |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| `Average_prices_of_electricity_to_ultimate_customers.csv` | Preço médio da eletricidade para os consumidores finais. Deve ser filtrado para o setor residencial. |
| `Cooling_degree_days_by_census_division.csv`              | Valores de graus-dia de resfriamento por região censitária dos EUA.                                  |
| `Heating_degree_days_by_census_division.csv`              | Valores de graus-dia de aquecimento por região censitária dos EUA.                                   |
| `Residential_sector_energy_consumption.csv`               | Consumo de energia por parte do setor residencial.                                                     |
|                                                             |                                                                                                        |

## Instalação do ambiente

```Shell
conda env create -f env.yml
```

```Shell
conda activate <env_name>
```

## Tecnologias

- **Python 3.12.13**
- **Sciki-Learn 1.9.0** — Random Forests
- **XGBoost** — Gradient Boost
