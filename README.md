# LAB-AI-900-DIO
Neste LAB, praticamos a criação de reconhecimento facial, identificação de dados em documentos e também o reconhecimento de elementos em imagens.

# Desenvolvimento do Lab
Antes iniciarmos o Lab, no Azure Machine Learning Studio, acessamos a página Automated ML (em Authoring). Posteriormente, criamos um novo trabalho de ML automatizado, respeitando as seguintes etapas:

### Configurações básicas:
- **Nome do trabalho:** mslearn-bike-automl
- **Novo nome do experimento:** mslearn-bike-rental
- **Descrição:** Aprendizado de máquina automatizado para previsão de aluguel de bicicletas
- **Marcadores:** nenhum

### Tipo de tarefa e dados:
- **Tarefa:** Regressão
- **Conjunto de dados:** Aluguel de bicicletas
- **Tipo de dados:** Tabular
- **Fonte de dados:** [URL da Web](https://aka.ms/bike-rentals)

### Configuração da tarefa:
- **Coluna de destino:** Aluguéis (inteiro)
- **Métrica primária:** raiz do erro quadrático médio normalizado
- **Modelos permitidos:** RandomForest e LightGBM

### Limites:
- **Máximo de testes:** 3
- **Máximo de testes simultâneos:** 3
- **Máximo de nós:** 3
- **Limite de pontuação da métrica:** 0,085 (finalizar o trabalho caso a pontuação da métrica de erro quadrático médio normalizado for igual ou inferior a 0,085).
- **Tempo limite:** 15
- **Tempo limite de iteração:** 15

# Resultados
Após execução das etapas supracitadas, foram encontradas as seguintes métricas:

### Métricas:
- **Variância explicada:** 0.78586
- **Erro absoluto de média:** 187.87
- **Erro de percentual absoluto de média:** 37.053
- **Erro mediano absoluto:** 115.76
- **Erro absoluto de média normalizado:** 0.055126
- **Erro mediano absoluto normalizado:** 0.033967
- **Erro de quadrado de média de raiz normalizado:** 0.089914
- **Erro de log de quadrado de média raiz normalizado:** 0.057918
- **Pontuação R2:** 0.78586
- **Erro de raiz do valor quadrático médio:** 306.43
- **Erro de log de raiz do valor quadrático médio:** 0.40752
- **Correlação de Spearman:** 0.91851
