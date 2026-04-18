# Tech Challenge - Tópicos 1 e 2

## 1. Entendimento do Negócio

- **Qual problema de negócio está sendo resolvido?**
> R: Atualmente, a empresa atua de forma **reativa**, pois só toma conhecimento da insatisfação do cliente após a finalização da jornada de compra, por meio da pesquisa. O desafio é transformar essa postura. Ou seja, identificar sinais de insatisfação antes para que a empresa possa agir de forma **proativa** antes mesmo de receber o feedback negativo no NPS.
- **Por que o NPS é importante para um e-commerce?**
>  R: O NPS é uma métrica fundamental para mensurar a percepção do cliente sobre o produto/atendimento e entrega. Além de indicar a lealdade, ele reflete o potencial de um cliente promotor divulga a marca espontaneamente, gerando novos negócios sem custo para a empresa. Por outro lado, o NPS ajuda a identificar danos causados por detratores que poderiam afastar futuros compradores.
- **Quais áreas poderiam se beneficiar desses insights?**
> R: Todas as áreas que funcionam como pontos de contato (ancoragem) com o cliente podem se beneficiar:
    - **Logística:** Identificar se o atraso na entrega é o principal causador de notas baixas para ajustar processos operacionais.
    - **Atendimento:** Perceber falhas na resolução de chamados e treinar equipes para melhorar a eficiência.
    - **Marketing e Produto:** Utilizar o feedback para entender se a qualidade e o preço do produto estão alinhados com a promessa da marca.
- **Quais indicadores de mercado poderiam complementar essa análise?**
> R: O NPS isolado pode conter informações subjetivas ou imprecisas. Para uma análise robusta, ele deve ser cruzado com dados objetivos:
    - **SLA Logístico:** Cruzar a percepção do cliente com o prazo real de entrega (ex: validar se uma reclamação de atraso condiz com o tempo de entrega prometido).
    - **Benchmarks do Setor:** Comparar o desempenho da empresa com a concorrência.
    - **Histórico de Pedidos:** Diferenciar insatisfações técnicas (erro no produto) de erros operacionais ou de expectativas do próprio cliente no momento da compra.

---

## 2. Definição da Target

Avaliação do entendimento conceitual sobre a variável alvo do problema.

- **Qual variável representa a satisfação do cliente?**
> R: Para medir a satifação do cliente nessa análise, podemos olhar duas variaveis principais presentes nos dados: o `nps_score` e o `cast_internal_score`, ambos em uma escala de 0 a 10.
- **Por que ela foi escolhida?**
> R: O `nps_score` é a variável alvo principal, pois quantifica a lealdade do cliente e a sua disposição em recomendar a marca após toda a jornada. O `csat_internal_score` funciona como um indicador complementar de satisfação pontual. Ele nos permite analisar se o atendimento recebido foi bem avaliado pelo cliente, independentemente de problemas que possam ter ocorrido em outras etapas.
- **Em que momento da jornada essa informação é coletada?**
> R: A coleta ocorre apenas ao final da jornada de venda, após o cliente ter percorrido todo o processo (compra, pagamento e entrega), capturando a percepção total.
- **Existe algum risco de usar essa variável de forma inadequada?**
> R: O principal risco é o **viés de resposta**, visto que muitos clientes não respondem à pesquisa. Isso pode gerar uma métrica baseada apenas nos "extremos" (clientes muito satisfeitos ou muito insatisfeitos), ignorando a opinião da maioria e mascarando a realidade da operação.
> R: Vazamento de dados: É um risco técnico alto, pois ocorre quando utilizamos informações que só estariam disponíveis depois ou junto com a nota do NPS para tentar prevê-la. Se utilizarmos apenas dados gerados após a insatisfação estar consolidada, o modelo perderá seu poder de antecipação e torna-se apenas um espelho do que já aconteceu.
