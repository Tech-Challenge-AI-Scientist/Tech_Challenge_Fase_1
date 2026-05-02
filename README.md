# Tech Challenge Fase 1 - Case NPS Preditivo

## Kick Off Tech Challenge:

📄 [Visualizar kick off](https://github.com/Tech-Challenge-AI-Scientist/Tech_Challenge_Fase_1/blob/main/docs/1IAST_Fase%201_Tech_Challenge.pdf?raw=true)

## Apresentação e Pitch do Projeto:

### Apresentação:

📊 [Visualizar apresentação](./docs/Tech_Challenge.pptx)

### Pitch
https://youtu.be/_JQkkD8b5fo

## Objetivo do Projeto:
O NPS é uma métrica fundamental para mensurar a percepção do cliente sobre o produto/atendimento e entrega. Além de indicar a lealdade, ele reflete o potencial de um cliente promotor divulga a marca espontaneamente, gerando novos negócios sem custo para a empresa. Por outro lado, o NPS ajuda a identificar danos causados por detratores que poderiam afastar futuros compradores.

Atualmente, a empresa atua de forma reativa, pois só toma conhecimento da insatisfação do cliente após a finalização da jornada de compra, por meio da pesquisa. O desafio é transformar essa postura. Ou seja, identificar sinais de insatisfação antes para que a empresa possa agir de forma proativa antes mesmo de receber o feedback negativo no NPS.

📄 [Entendimento do Negócio](./docs/entendimento_negocio_target.md)

## Descrição da Base de Dados:

### Dicionário de Dados
● customer_id: Identificador único do cliente;

● order_id: Identificador único do pedido;

● customer_age: Idade do cliente;

● customer_region: Região geográfica do cliente;

● customer_tenure_months: Tempo de relacionamento do cliente com a
empresa (em meses);

● order_value: Valor total do pedido;

● items_quantity: Quantidade de itens no pedido;

● discount_value: Valor de desconto aplicado ao pedido;

● payment_installments: Número de parcelas do pagamento;

● delivery_time_days: Tempo total de entrega (em dias);

● delivery_delay_days: Quantidade de dias de atraso na entrega;

● freight_value: Valor do frete;

● delivery_attempts: Número de tentativas de entrega;

● customer_service_contacts: Número de contatos do cliente com o
atendimento;

● resolution_time_days: Tempo para resolução de problemas (em dias);

● complaints_count: Número de reclamações registradas pelo cliente;

● repeat_purchase_30d: Indica se houve recompra em até 30 dias após o
pedido (0 = não, 1 = sim);

● csat_internal_score: Score interno de satisfação do cliente;

● nps_score: Nota de satisfação do cliente (NPS), variando de 0 a 10, coletada
após a experiência de compra.

## Metodologia Utilizada

## Como reproduzir os resultados:
### Estrutura de diretórios:

- **data:** dados em formato .csv
- **docs:** arquivos de texto, documentação e apresentação
- **eda:** análise exploratória dos dados
- **prediction:** algoritmos de machine learning para predição

### Pré-requisitos
- Python 3.12+
- Git

### Instalação e configuração do projeto

No seu terminal (Powershell ou Bash):

1. Clone o repositório
```bash
   git clone git@github.com:Tech-Challenge-AI-Scientist  Tech_Challenge_Fase_1.git
   cd Tech-Challenge-AI-Scientist
```

2. Crie e ative o ambiente virtual
```bash
   python -m venv venv
```
 
-  No Linux/Mac:
```bash
   source venv/bin/activate
```
   
-  No Windows:
```bash
   venv\Scripts\activate
```

3. Instale as dependências
```bash
   pip install -r requirements.txt
```
