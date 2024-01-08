# Como provisionar um cluster EKS com ênsafe à FinOps !

Quando recebemos alguma demanda para provisionar mais recursos em um provedor, qualquer que seja ele: AWS, GCP ou Azure, com ferramentas de IaC como Terraform e CI/CD, tendo muitos benefícios dispostos, em alguns momentos temos certas dificuldades para estimar com precisão os custos de uma nuvem.

Os provedores de nuvem podem ter estruturas de custos complexas que estão em constante mudança, claro que é simples de configurar alertas de faturamento, mas não há garantias de que eles funcionarão com mais detalhes, os alertas podem acontecer durante o fim de semana fazendo-nos "passar" pelo nosso orçamento em poucas horas.

Falando nisso, qual o custo de provisionar um Kubernetes na AWS ? Encontrei uma ferramenta bacana e quero mostrar o resultado do que ela pode trazer para o ecossistema de um ambiente de cloud, para tanto fiz alguns testes com o Infracost e fiquei bastante feliz pelo resultado:

<img width="769" alt="Infracost01" src="https://github.com/SlackMaker/EKSCluster/assets/42175054/3077f386-24b4-49d1-953a-fb93f2b438de">
<img width="519" alt="Infracost02" src="https://github.com/SlackMaker/EKSCluster/assets/42175054/9f5de69c-671e-4008-a3de-4a9d3679ff72">

Fontes:
- https://developer.hashicorp.com/terraform/tutorials/kubernetes/eks
- https://www.infracost.io/
