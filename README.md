# 🚗 Análise de Perfil de Leads e Tráfego de Veículos

## 📋 Sobre o Projeto
Este projeto contém um conjunto de análises focadas em entender o perfil demográfico dos potenciais clientes (leads) e o comportamento de visitação de produtos em uma plataforma de vendas de veículos. 

O objetivo principal é extrair *insights* valiosos sobre quem são os clientes e quais produtos mais atraem a atenção deles. A extração e o tratamento dos dados foram realizados em **SQL**, enquanto a análise final e a visualização foram estruturadas em **Microsoft Excel**, auxiliando na tomada de decisão estratégica para equipes de Marketing e Vendas.

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** SQL (PostgreSQL / compatível)
* **Visualização e Análise:** Microsoft Excel (Tabelas Dinâmicas e Gráficos)
* **Técnicas SQL:** `JOINs`, `CTEs`, `CASE WHEN`, funções de data e agregações analíticas.

---

## 📈 Visualização de Dados (Integração com Excel)
Após a extração dos dados formatados via SQL, os resultados foram exportados para o Excel para a construção de tabelas e cruzamentos dinâmicos. Essa abordagem permite uma leitura mais visual e rápida por parte das áreas de negócio.

> ### 🖼️ Dashboard / Tabela de Resultados
> Abaixo, você pode visualizar a consolidação dos dados processados:
> 
> ![Tabela de Análise de Leads no Excel](NOME_DA_SUA_IMAGEM.png)
> 
> *Nota: Para visualizar a imagem acima, salve o print do seu Excel na pasta raiz do projeto e substitua "NOME_DA_SUA_IMAGEM.png" pelo nome do arquivo.*

---

## 🗄️ Estrutura de Dados Analisada
O projeto utiliza as seguintes tabelas principais:
* **`sales.customers`**: Dados cadastrais (nascimento, renda, profissão).
* **`sales.funnel`**: Registro de visitas às páginas dos produtos.
* **`sales.products`**: Catálogo de veículos (marca, modelo, ano).
* **`temp_tables.ibge_genders`**: Tabela auxiliar para classificação de gênero por nome.

---

## 📊 Principais Análises e Queries

O script SQL está dividido em categorias que alimentam as planilhas:

### 1. Perfil Demográfico dos Leads
* **Gênero:** Volume de leads divididos entre homens e mulheres.
* **Status Profissional:** Representatividade percentual de cada categoria (CLT, Autônomo, etc.).
* **Faixa Etária:** Distribuição percentual em grupos de idade (ex: 20-40, 40-60).
* **Faixa Salarial:** Classificação por capacidade financeira em intervalos de R$ 5.000.

### 2. Comportamento de Visitação (Veículos)
* **Novos vs. Seminovos:** Regra de negócio definida como: Novos (até 2 anos) e Seminovos (acima de 2 anos).
* **Interesse por Idade:** Quebra das visitas em faixas de idade do veículo a cada 2 anos.
* **Modelos Mais Populares:** Ranking de visitas por marca e modelo.

---

## 🚀 Como Executar
1. Execute o script `.sql` no seu editor (DBeaver, pgAdmin, etc.).
2. Exporte os resultados das queries para formato `.csv` ou `.xlsx`.
3. Utilize o arquivo **Excel** incluído neste repositório para importar os dados e atualizar os gráficos automaticamente.

---
