# new-bot
Novo projeto de automação de trade baseado em dados de inflação e taxas de juros. Que fazem impacto imediatos na cotação dos indices americanos e ouro.

- ### CPI MENSAL
    Sempre na segunda semana do mês, é divulgado o CPI do mês anterior. Geralmente ás 8:30 AM Washington, DC.
    O CPI mensal (MoM) tende a ter um impacto mais imediato e forte na cotação dos mercados quando é anunciado, mas o CPI anual (YoY) define a tendência de longo prazo.
    Por que o CPI mensal (MoM) tem mais impacto imediato?
    1. Surpresa do mercado 🎭

        ◦ O mercado já precifica uma expectativa antes da divulgação. __Se o CPI mensal vem diferente do esperado, a reação é forte e imediata.__ 

        ◦ Exemplo: Se a expectativa era 0,2% MoM, mas sai 0,4%, os mercados podem despencar porque indica inflação persistente → Fed pode manter juros altos por mais tempo. 

    2. Apostas de curto prazo em juros (FED) 🏦

        ◦ Operadores do mercado acompanham o CPI mensal para ajustar suas apostas sobre o próximo movimento do Federal Reserve (Fed) na taxa de juros. 

        ◦ Se o CPI sobe mais que o esperado → Apostas de juros mais altos → Ações caem, dólar sobe. 

        ◦ Se o CPI vem mais baixo → Apostas de cortes de juros → Ações sobem, dólar cai. 

    3. Reação dos algorítmicos e traders institucionais 

        ◦ A maioria dos robôs e traders de alta frequência operam em cima da surpresa do CPI mensal, gerando volatilidade extrema logo nos primeiros segundos após a divulgação. 

    ### Mas e o CPI Anual (YoY)?

    • Importante para tendências de longo prazo 📉📈 
        ◦ Se o CPI anual mostra uma tendência de queda consistente, o mercado precifica cortes de juros no futuro → Ações sobem, cripto dispara. 
        ◦ Se continua alto, o Fed pode manter juros elevados → Mercado cai. 

    • Menos volatilidade no dia do anúncio, pois os investidores já acompanham essa tendência nos meses anteriores. 

Resumo: Qual CPI influencia mais na cotação quando sai a notícia?

    🔹 CPI Mensal (MoM) → Impacto imediato no mercado, movimenta day traders e robôs.

    🔹 CPI Anual (YoY) → Define tendências de longo prazo, mas não costuma gerar picos de volatilidade na hora da divulgação.

    Se você quer operar no momento da divulgação do CPI, o CPI Mensal (MoM) é o dado mais relevante. 🚀📊

## O que analisar:
    Captar dados do cpi desde 2000 até 2025. Armazenar valores com valores de expectativas, datas e horas exatas e verificar quais resultados teve nas cotações dos indices americanos e do ouro.

Vou me reter inicialmente o CPI mas, vários outros indicadores econômicos geram um impacto forte e imediato nas cotações, parecido com o **CPI mensal (MoM)**. Os principais são:  

---

### 🔥 **1. PCE (Personal Consumption Expenditures) – Inflação preferida do Fed**
- 📅 **Periodicidade**: Mensal  
- 🏦 **Impacto**: Alto  
- 🎯 **Por que importa?** O **PCE** é o indicador de inflação **favorito do Federal Reserve** e pode influenciar diretamente as decisões sobre juros.  
- 📉 **Reação do mercado**:  
  - Se o PCE vier **acima do esperado** → **Bolsa cai**, dólar sobe, juros futuros sobem.  
  - Se vier **abaixo do esperado** → **Bolsa sobe**, dólar cai, apostas em cortes de juros aumentam.  
- 🔗 [Site do PCE - BEA](https://www.bea.gov/data/personal-income-saving/personal-income)  

---

### 📈 **2. Relatório de Emprego (Payroll - Nonfarm Payrolls, NFP)**
- 📅 **Periodicidade**: Mensal (primeira sexta-feira do mês)  
- 🏦 **Impacto**: Muito Alto 🚨  
- 🎯 **Por que importa?** Mede a criação de empregos nos EUA (exceto setor agrícola). Afeta diretamente a política do Fed.  
- 📉 **Reação do mercado**:  
  - Se os empregos aumentam muito → Economia forte → **Bolsa cai**, dólar sobe (Fed pode manter juros altos).  
  - Se os empregos crescem menos que o esperado → Economia desacelera → **Bolsa sobe**, dólar cai.  
- 🔗 [Relatórios do Payroll - BLS](https://www.bls.gov/news.release/empsit.toc.htm)  

---

### 🏠 **3. PMI (Purchasing Managers’ Index)**
- 📅 **Periodicidade**: Mensal  
- 🏦 **Impacto**: Alto  
- 🎯 **Por que importa?** Mede a atividade da indústria e do setor de serviços. Se o PMI mostra crescimento forte, pode significar inflação futura.  
- 📉 **Reação do mercado**:  
  - PMI forte → Economia aquecida → **Bolsa cai**, dólar sobe (Fed pode manter juros altos).  
  - PMI fraco → Economia desacelerando → **Bolsa sobe**, dólar cai (expectativa de corte de juros).  
- 🔗 [PMI nos EUA - ISM](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/)  

---

### 💵 **4. Decisão de Taxa de Juros do Federal Reserve (FOMC)**
- 📅 **Periodicidade**: A cada **6 semanas**  
- 🏦 **Impacto**: Máximo 🚨🚨🚨  
- 🎯 **Por que importa?** Define a taxa de juros dos EUA e as expectativas para os próximos meses.  
- 📉 **Reação do mercado**:  
  - **Alta inesperada de juros** → **Bolsa cai**, dólar sobe, cripto despenca.  
  - **Corte de juros ou tom dovish** → **Bolsa sobe**, dólar cai, cripto dispara.  
- 🔗 [Calendário do FOMC](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm)  

---

### 🏠 **5. Índices do Mercado Imobiliário (Housing Data)**
- 📅 **Periodicidade**: Mensal  
- 🏦 **Impacto**: Moderado  
- 🎯 **Por que importa?** Dados como **construção de casas novas, vendas de imóveis e preços dos imóveis** afetam a percepção sobre a economia.  
- 📉 **Reação do mercado**:  
  - Mercado imobiliário forte → **Bolsa pode cair**, pois sugere inflação persistente.  
  - Mercado imobiliário fraco → **Bolsa pode subir**, pois sugere desaceleração econômica.  
- 🔗 [Dados imobiliários - Census.gov](https://www.census.gov/construction/nrs/index.html)  

---

### **🚀 Resumo: Principais Indicadores que Movem o Mercado Como o CPI**
| Indicador | Periodicidade | Impacto | O que afeta? |
|-----------|-------------|---------|--------------|
| **CPI Mensal (MoM)** | Mensal | 🔥🔥🔥 | Inflação, política do Fed |
| **PCE (Inflação preferida do Fed)** | Mensal | 🔥🔥🔥 | Política monetária |
| **Payroll (NFP - Emprego)** | Mensal | 🚨🚨🚨 | Força do mercado de trabalho |
| **PMI (Atividade Econômica)** | Mensal | 🔥🔥 | Crescimento e inflação futura |
| **FOMC (Taxa de Juros do Fed)** | A cada 6 semanas | 🚨🚨🚨 | Política de juros |
| **Mercado Imobiliário (Housing Data)** | Mensal | 🔥 | Economia real, consumo |

Se quiser acompanhar esses dados e entender como operar com base neles, posso te ajudar a criar uma estratégia. Quer montar um **calendário de eventos econômicos** para operar? 📅📊🚀