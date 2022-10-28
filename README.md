# Desafio Técnico DevOps Sênior

Esse é um desafio feito para conhecer um pouco mais de cada candidato a vaga de DevOps na Varsomics. Não se trata de um teste objetivo, capaz de gerar uma nota ou uma taxa de acerto, mas sim de um estudo de caso com o propósito de conhecer os conhecimentos, experiências e modo de trabalhar de um cadidato. Sinta-se livre para desenvolver sua solução para o problema proposto.

## Descrição

Para esse desafio assumiremos que você candidato, trabalha em uma empresa fictícia do ramo da bioinformática. Vocês estão planejando o desenvolvimento de uma nova aplicação web que realiza análises de **espectrometria de massas** de proteínas. A aplicação em questão permite que o usuário faça o upload de diversos arquivos por amostra (um arquivo por proteína na amostra) e, o mesmo, pode realizar a análise de diferentes amostras ao mesmo tempo em conjunto com outros usuários que utilizarão a aplicação.

Seu objetivo neste desafio é desenvolver uma solução que abranja todos os recursos necessários para o provisionamento desta aplicação em um ambiente cloud, utilizando, em todas as etapas, ferramentas e serviços presentes na AWS. Abaixo temos mais informações sobre a aplicação e entregas esperadas ao final do desafio.

## Detalhes da Aplicação

Abaixo listamos os requisitos que a sua solução deve comportar para o ambiente da aplicação apresentada anteriormente. Detalhes adicionas da problemática também serão fornecidos a seguir.

- A aplicação em questão será separa em um front-end desenvolvido utilizando o framework Django do python e uma API controladora do serviço desenvolvida utilizando o framework FastAPI também do python. O servidor da API e eventuais outros serviços gerenciados pela aplicação devem ser deployados utilizando Kubernetes.
- A parte da análise de espectrometria de massas será realizada por step functions e AWS Batch, esses serviços serão invocados pela API da aplicação. O fluxo de análise será submetido por demanda de acordo com as solicitações realizadas na aplicação.
- Após a análise dos dados métricas devem ser armazenadas num banco de dados relacional.
- Essas métricas serão disponibilizadas para o usuário final em uma dashboard. Para isso, os dados deverão ser processados e alocados em um cluster do Redshift.

## Entrega

1. Deverá ser feito um diagrama dessa infraestrutura de forma a exemplificar a solução proposta.
2. Deverá ser feito um documento com a descrição passo a passo do provisionamento dessa solução.
3. Deverá ser organizada uma apresentação visual que será realizada pelo candidato no dia de sua avaliação.

Boa sorte!

#### NÃO É NECESSÁRIO SUBIR O RECURSOS EM ALGUM CONTA AWS PRÓPRIA, SOMENTE A DESCRIÇÃO DOS PASSOS É NECESSÁRIA!
