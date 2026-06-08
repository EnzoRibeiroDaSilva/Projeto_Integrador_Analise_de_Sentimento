#  O Peso das Palavras - Análise Exploratória de Avaliações de Clientes - Orientador Felipe Camargo

##  Fonte dos Dados

Projeto desenvolvido utilizando o banco de dados oficial disponibilizado pela **AWS** em parceria com o **SENAI Suíço-Brasileiro** para atividades acadêmicas.

---

##  Problema de Negócio

Em marketplaces digitais, clientes avaliam produtos por meio de notas (de 1 a 5 estrelas) e comentários textuais. Entretanto, nem sempre a nota atribuída é coerente com o conteúdo do comentário, o que pode dificultar a interpretação real da satisfação do cliente.

Diante desse cenário, surge a necessidade de analisar a relação entre as avaliações numéricas e os comentários, buscando identificar padrões de comportamento, tendências e possíveis inconsistências nas percepções dos consumidores.

---

##  Objetivo

Investigar os dados de avaliações de clientes para compreender a relação entre os comentários textuais e as notas atribuídas, identificando:

* Padrões de comportamento dos consumidores;
* Tendências de satisfação e insatisfação;
* Possíveis inconsistências entre comentários e avaliações;
* Insights relevantes para interpretação da experiência do cliente.

---

##  Descrição do Banco de Dados

O conjunto de dados fornecido pela AWS possui **9 tabelas**:

```text
vendedores.csv
produtos.csv
pedidos.csv
pagamentos.csv
itens_pedidos.csv
geolocalizacao.csv
clientes.csv
avaliacoes.csv
tabela_auxiliar.csv
```

###  Observação

A tabela `tabela_auxiliar.csv` contém a tradução de termos presentes no dataset original.

---

##  Linguagens Utilizadas

### Python

Principal linguagem utilizada para:

* Manipulação e limpeza dos dados;
* Análise exploratória;
* Tratamento de informações;
* Criação de visualizações gráficas;
* Implementação de modelos de análise de sentimento.

##  Bibliotecas Utilizadas

### Pandas

Biblioteca utilizada para manipulação, tratamento e análise de dados tabulares.

### NumPy

Utilizada para operações matemáticas e análises estatísticas.

### Matplotlib

Ferramenta para criação de gráficos e visualizações de dados.

### Seaborn

Biblioteca de visualização baseada no Matplotlib, utilizada para gerar gráficos mais intuitivos e esteticamente agradáveis.

### WordCloud

Utilizada para gerar nuvens de palavras, facilitando a visualização dos termos mais frequentes nos comentários.


---

##  Modelos de Análise de Sentimento

### Vader

**VADER (Valence Aware Dictionary and sEntiment Reasoner)** é uma ferramenta de Processamento de Linguagem Natural (PLN) baseada em léxico, amplamente utilizada para classificação de sentimentos em textos.

Principais características:

* Classificação de sentimentos em positivo, negativo ou neutro;
* Excelente desempenho em textos curtos;
* Boa interpretação de gírias, abreviações e emojis;
* Muito utilizada em análises de redes sociais.

### leIA

**leIA (Léxico para Inferência Adaptada)** é uma adaptação voltada para a língua portuguesa, permitindo análises de sentimento mais adequadas ao contexto brasileiro.

### Transformers

Biblioteca desenvolvida pela Hugging Face e considerada o padrão da indústria para aplicações modernas de Inteligência Artificial.

Permite trabalhar com modelos como:

* BERT;
* GPT;
* LLaMA;
* Entre outros.

Além do Processamento de Linguagem Natural (PLN), também oferece recursos para:

* Visão computacional;
* Processamento de áudio;
* Classificação de textos;
* Geração de conteúdo.

---

## Conclusão

O presente projeto teve como objetivo analisar a relação entre as avaliações numéricas e os comentários textuais realizados pelos clientes de um marketplace, utilizando técnicas de **Análise Exploratória de Dados (EDA)** e **Processamento de Linguagem Natural (PLN)**.

A partir da integração das diferentes tabelas disponibilizadas pela AWS e pelo SENAI Suíço-Brasileiro, foi possível construir uma base consolidada contendo informações de pedidos, produtos, pagamentos, vendedores, clientes e avaliações. Após as etapas de limpeza, tratamento e padronização dos dados, foram aplicados três modelos distintos de análise de sentimento: **VADER**, **LeIA** e **Transformers**.

Os resultados demonstraram uma forte relação entre as notas atribuídas pelos clientes e os sentimentos identificados nos comentários. Em geral, avaliações com notas mais elevadas apresentaram sentimentos positivos, enquanto avaliações com notas mais baixas foram associadas a sentimentos negativos. Além disso, observou-se divergência entre os modelos utilizados, evidenciando diferentes interpretações dos textos analisados.

Também foram identificados casos de incoerência entre a nota atribuída e o conteúdo textual do comentário, revelando situações em que a avaliação numérica não representa completamente a percepção expressa pelo cliente. Aproximadamente **10% das avaliações analisadas** apresentaram sentimentos opostos ao score informado, reforçando a importância da análise textual como complemento às métricas tradicionais de satisfação.

As análises de frequência de palavras e as nuvens de palavras permitiram identificar os principais fatores relacionados à satisfação e à insatisfação dos consumidores, fornecendo informações relevantes para a tomada de decisões. Da mesma forma, a análise por categoria de produto possibilitou identificar segmentos com melhor percepção por parte dos clientes.

Dessa forma, conclui-se que a utilização de técnicas de **Ciência de Dados**, **Análise de Sentimentos** e **PLN** proporciona uma visão mais completa da experiência dos consumidores, permitindo compreender não apenas as notas atribuídas, mas também os sentimentos expressos nos comentários. Os resultados obtidos demonstram o potencial dessas ferramentas para apoiar estratégias de melhoria contínua, gestão da qualidade, aprimoramento da experiência do cliente e aumento da satisfação em ambientes de marketplace ou em qualquer contexto que utilize avaliações como indicador de desempenho.

---

##  Autores

Este projeto foi desenvolvido por:

* **Igor Maurílio** — GitHub: https://github.com/igoormaurilio
* **Enzo Ribeiro Silva** — GitHub: https://github.com/EnzoRibeiroSilva


Projeto desenvolvido como parte das atividades acadêmicas do **SENAI Suíço-Brasileiro**, utilizando dados disponibilizados pela **AWS** para fins educacionais e de pesquisa em Ciência de Dados.

