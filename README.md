# 1.0 Sobre o AVC

De acordo com a Organização Mundial da Saúde (OMS), o AVC é a 2ª causa de morte no mundo, responsável por aproximadamente 11% do total de mortes.

Este conjunto de dados é usado para prever se um paciente tem probabilidade de desenvolver AVC com base nos parâmetros de entrada como sexo, idade, várias doenças e tabagismo. Cada linha dos dados fornece informações relevantes sobre o paciente.

# 2.0 Desafio de negócio 

- Qual é o contexto? Classificar se o paciente pode ter AVC ou não .

- Por que fazer uma classificação se o paciente tem AVC? Para auxiliar o profissional da saúde com  o diagnóstico dos pacientes.

- Quem é a parte interessada do projeto? Profissionais de saúde

- Qual é o formato?

- Granularidade? Por paciente 
- Tipo de problema? Problema de classificação 
- Como vamos entregar? Bot Telegram, Streamlit ou Google Sheets (Vou decidir mais para frente qual o melhor forma de apresentar a solução)

## 3.0 Estratégia de Solução
Minha estratégia para resolver esse desafio foi:

**Etapa 01.** Coleta dos dados: Nesta etapa o objetivo coletar os dados do kaggle.
**Etapa 02.** Descrição dos dados: Nesta estapa o objetivo é usar métricas estatísticas para identificar dados fora do escopo do negócio
**Etapa 03.** Feature Engineering: Derivar novos atributos com base nas variáveis originais para descrever melhor o fenômeno que será modelado
**Etapa 04.** Filtragem de Dados: Filtrar as linhas e selecione as colunas que não contenham informações para modelagem que não correspondam ao escopo
**Etapa 05.** Análise Exploratória de Dados: Para esta etapa o objetivo é explorar os dados para entender melhor o impacto das variáveis no aprendizado do modelo e encontrar insights.
**Etapa 06.** Preparação dos Dados: Prepare os dados para que os modelos de aprendizados de máquina possam aprender o comportamento específico.
**Etapa 07.** Seleção de Recursos: Seleção dos atributos mais significativos para treinar o modelo.
**Etapa 08.** Machine Learning: Treinamento de Machine Learning.
**Etapa 09.** Hyperparamenter Fine Tunning: Escolha os melhores valores para cada um dos parâmetros do modelo selecionado na etapa anterior.
**Etapa 10.** Interpletação do desempenho do modelo em valores de negócios: converta o desempenho do modelo de aprendizado de máquina em um resultado de negócios.
**Etapa 11.** Deploy do modelo: Publicar o modelo em um ambiente de nuvem para que outras pessoas ou serviços possam usar os resultados para melhorar a decisão de negócios.

# 4.0 O conjunto de dados

<b>id:</b> identificador único
<b>gênero:</b> "Masculino", "Feminino" ou "Outro"
<b>idade:</b> idade do paciente
<b>hipertensão:</b> 0 se o paciente não tem hipertensão, 1 se o paciente tem hipertensão
<b>doença cardíaca:</b> 0 se o paciente não tem doenças cardíacas, 1 se o paciente tem doença cardíaca
<b>nunca_casou:</b> "Não" ou "Sim"
<b>work_type:</b> "filhos", "Govt_jov", "Nunca_trabalhou", "Privado" ou "Autônomo"
<b>Residence_type:</b> "Rural" ou "Urbano"
<b>avg_glucose_level:</b> nível médio de glicose no sangue
<b>bmi:</b> índice de massa corporal
<b>smoking_status:</b> "anteriormente fumado", "nunca fumado", "fuma" ou "Desconhecido" *
<b>AVC:</b> 1 se o paciente teve um AVC ou 0 se não

<b>Nota: "Desconhecido" em smoking_status significa que a informação não está disponível para este paciente.</b>

# 5.0 Referências

[Fatores de Risco](http://www.redebrasilavc.org.br/para-pacientes-e-falimiares/fatores-de-risco/)
[Hábitos para prevenir acidentes Vascular Cerebral](https://planin.com/sbn-recomenda-mudanca-de-habitos-para-prevenir-acidente-vascular-cerebral-avc/)
[5 Hábitos que favorecem o AVC](https://coris.med.br/5-habitos-que-favorecem-o-avc/)