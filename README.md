# ⛽ Análise de Preços de Combustíveis  
### Série Histórica — 10/05/2004 a 28/06/2024

---

## 🧠 Descrição Geral

Este projeto apresenta uma análise da **evolução dos preços de combustíveis no Brasil ao longo de 20 anos** (2004–2024), utilizando os dados oficiais disponibilizados pela **ANP – Agência Nacional do Petróleo, Gás Natural e Biocombustíveis**.

O objetivo é permitir que o usuário **compare preços em diferentes recortes geográficos**, entenda o comportamento histórico dos combustíveis e explore diferenças entre **regiões, estados, cidades, bairros, revendas e bandeiras**.

O relatório foi desenvolvido integralmente no **Power BI**.

📊 **Acesse o relatório completo:**  
👉 [Clique aqui para visualizar](https://app.powerbi.com/view?r=eyJrIjoiZTY3MWZlZjgtYWY5Yi00MWEwLThkYjMtYmZjMTFiNDJkN2ZiIiwidCI6IjYzOTc3ZmU3LTAwNjgtNDI0ZC05YTAyLTNmYTg3MGQ5ZGE5MyJ9)

---

## 📌 Fonte

Este BI utiliza dados disponibilizados pela **Agência Nacional do Petróleo, Gás Natural e Biocombustíveis (ANP)**, vinculada ao portal do Governo Federal.

O site disponibiliza preços praticados por revendedores de diversos produtos (como GLP P13), mas **este relatório utiliza apenas os combustíveis automotivos**:

- Diesel  
- Diesel S10  
- Diesel S50  
- Etanol  
- Gasolina  
- Gasolina aditivada  
- GNV  

🔗 Fonte oficial:  
https://www.gov.br/anp/pt-br/centrais-de-conteudo/dados-abertos/serie-historica-de-precos-de-combustiveis

---

## 🎯 Objetivo

Ao abastecer, muitas vezes surgem perguntas como:

> “Será que o preço da gasolina é mais barato no bairro vizinho?”  
> “Há variação de preços dentro do meu bairro?”  
> “O preço médio no interior é mais caro do que na capital?”

Assim, este BI foi criado para permitir ao usuário comparar:

- ▪ Diferenças de preços entre regiões do país  
- ▪ Diferenças entre estados  
- ▪ Preço médio estadual vs. preço médio nacional  
- ▪ Capital x interior  
- ▪ Diferenças de preço entre cidades (mais cara, mais barata e diferença)  
- ▪ Diferenças entre bairros de uma mesma cidade  
- ▪ Diferenças entre revendas (postos)  
- ▪ Diferenças entre bandeiras (marcas/distribuidoras)  
- ▪ Quais bandeiras estão presentes em mais territórios  
- ▪ Variação percentual entre anos  
- ▪ Comparação entre evolução do preço dos combustíveis e dólar  

---

## 📝 Observações

Alguns pontos importantes:

- ▪ Os dados são coletados **semanalmente** por uma empresa contratada pela ANP.  
- ▪ Nem todas as cidades possuem registros.  
- ▪ Mesmo em cidades com coleta, **nem todos os bairros e revendas** possuem dados.  
- ▪ Em muitos casos, há informações de um bairro/revenda apenas em alguns meses do ano.  
- ▪ Ainda assim, trata-se de uma amostra ampla e realista, considerando a fonte oficial.

Sobre o comparativo com o dólar:

- ▪ Vários fatores influenciam o preço dos combustíveis (estratégias da Petrobras/governo, conflitos internacionais, impostos, decisões da OPEP, etc.).  
- ▪ O gráfico que compara evolução do combustível com o dólar **não afirma causalidade**, mas mostra que a taxa de câmbio tem influência relevante.

---

## 🗺️ Estrutura do BI

A lógica analítica foi estruturada em ordem **macro → micro**:

- ▪ País / Regiões  
- ▪ Estados  
- ▪ Cidades  
- ▪ Bairros  

Também há páginas dedicadas a:

- ▪ Comparação entre bandeiras  
- ▪ Evolução histórica dos preços  

A métrica principal utilizada foi o **preço médio**.

---

## 🚀 Melhorias Futuras

Alguns pontos identificados para uma futura versão:

- ▪ Padronização de nomes de bairros (ex.: *Enseada do Suá* vs *Enseada da Suá* em Vitória/ES).  
- ▪ Tratar cidades que pertencem à região metropolitana como parte da capital na comparação “capital x interior”.  
  - Ex.: Vila Velha (ES), Guarulhos (SP), Contagem (MG), Camaçari (BA).  
- ▪ Automatizar o BI para atualizar os dados semestralmente.  
- ▪ Criar página dedicada à análise de outliers.

---

## 🔍 Insights

Conforme descrito em “Objetivos”, as possibilidades de análise são amplas.  
A seguir, alguns dos principais achados (com foco inicial em gasolina e no estado/cidade natal do autor — Vitória, ES):

### 🔹 Regiões e Estados
- ▪ Em **9 dos últimos 10 anos**, a **Região Norte** teve o primeiro ou segundo preço mais caro.  
- ▪ A **Região Sudeste** foi a que mais vezes apareceu entre os preços mais baratos.  
- ▪ No Sudeste, entre 2015–2022, a ordem sempre foi (do mais caro ao mais barato):  
  **RJ → MG → ES → SP**.  
- ▪ Em 2023 e 2024, o **ES se tornou o estado com o valor mais caro do Sudeste**.  
- ▪ Em 2024, o preço médio do ES foi **R$ 0,26 (4,65%)** mais caro que SP.  

### 🔹 Estado vs. Brasil
- ▪ De 2015 a 2021, o ES ficou sempre muito próximo da média nacional.  
- ▪ Nos últimos 3 anos, passou a ser **mais caro** que a média do país.

### 🔹 Capital x Interior (Vitória/ES)
- ▪ Nos últimos 20 anos, Vitória **sempre foi mais barata** que o interior.  
- ▪ A diferença aumentou nos últimos anos.  
- ▪ Em 2023, por exemplo, o valor médio na capital capixaba foi R$ 0,28 (4,92%) mais barato que no interior. 

📝 *Observação:*  
O ES tem 78 municípios, mas **de 2018 a 2024 apenas 10 cidades possuem dados**.

### 🔹 Comparação entre Cidades
- ▪ Ao comparar o valor entre as cidades do ES, observa-se que não só Vitória, mas de modo geral as cidades da região metropolitana costumam ter valores mais baratos do que as cidades do interior.   

### 🔹 Bairros
- ▪ Em Vitória (2024), há **R$ 0,32 de diferença** entre o bairro mais barato e o mais caro.  
- ▪ Em 2022, a diferença foi **R$ 1,82**, a maior dos últimos 10 anos.

### 🔹 Bandeiras
- ▪ 34% das revendas são **Bandeira Branca (posto independente que não tem uma marca ou bandeira associada).**.  
- ▪ **Ipiranga**, **Vibra** e **Raízen** representam ~61% das revendas.  
- ▪ **Ale**, **Alesat**, **Ipiranga**, **Raízen** e **Vibra** estão presentes em todas as regiões.  
- ▪ Apenas a **Vibra** está em **todos os estados** e presente em **400 cidades**.  
- ▪ No ES,  
  - Vibra → mais revendas  
  - Ipiranga → presente em mais cidades  
- ▪ Em Vitória, há uma diferença de R$ 0,32 entre o preço médio da bandeira mais cara (Ale) e da mais barata (Alesat).

### 🔹 Evolução Histórica (2004–2024) no país
- ▪ Preço médio aumentou **R$ 3,64 (+170,09%)**.  
- ▪ Maior salto anual: **2020 → 2021 (+37,62%)**.  
- ▪ 2004–2014: +40,65%  
- ▪ 2015–2024: +72,54%  
- ▪ Valor mais alto da série: **R$ 6,32 em 2022**.

---
