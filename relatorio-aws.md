# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 07 de Janeiro de 2026  
**Empresa:** Golden Order  
**Responsável:** Lucas Galvano de Paula

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa **Golden Order**, realizado por **[Seu Nome Completo]**. O objetivo do projeto foi elencar 3 serviços AWS estratégicos, visando a redução de custos imediatos e o aumento da segurança e conformidade dos dados sensíveis da companhia.

## Descrição do Projeto
O projeto de implementação foi estruturado em três pilares: eficiência de armazenamento, otimização de processamento e modernização de arquitetura.

### Etapa 1: Amazon S3 (Simple Storage Service)
- **Foco da ferramenta:** Repositório de dados durável e seguro.
- **Descrição de caso de uso:** A Golden Order passará a utilizar o S3 para centralizar todos os seus dados de Pesquisa e Desenvolvimento (P&D). Em vez de manter servidores físicos caros que exigem trocas constantes de discos, o S3 oferece um modelo de "pagamento por uso".
- **Justificativa de Segurança:** O S3 oferece criptografia automática (AES-256) tanto para dados parados quanto em trânsito. Para o setor farmacêutico, isso garante que fórmulas e patentes estejam protegidas contra acessos não autorizados. Além disso, a ferramenta permite o "Versionamento", que protege os documentos contra exclusões acidentais ou ataques de Ransomware, permitindo recuperar versões anteriores instantaneamente.

### Etapa 2: Amazon EC2 com Instâncias Spot
- **Foco da ferramenta:** Computação de alto desempenho com economia de escala.
- **Descrição de caso de uso:** Para análises químicas complexas e simulações que demandam muito processamento, utilizaremos as Instâncias Spot. Elas aproveitam a capacidade computacional ociosa da AWS com descontos de até 90%. Isso permite que a Golden Order realize pesquisas que antes levariam meses em apenas alguns dias, sem elevar o orçamento.
- **Justificativa de Segurança:** O EC2 opera dentro da **Virtual Private Cloud (VPC)**, uma rede isolada na nuvem que funciona como o seu próprio data center virtual. O controle de acesso é rígido através de "Security Groups" (firewalls virtuais), garantindo que apenas as máquinas autorizadas e os pesquisadores autenticados tenham acesso aos dados de processamento.

### Etapa 3: AWS Lambda
- **Foco da ferramenta:** Automação e execução de código sem servidores (Serverless).
- **Descrição de caso de uso:** O Lambda será utilizado para processar fluxos de trabalho, como a validação de pedidos de distribuidores ou a triagem automática de laudos laboratoriais. A empresa deixa de pagar por um servidor ligado o dia todo e passa a pagar apenas pelos segundos em que o código está sendo executado.
- **Justificativa de Segurança:** Ao eliminar a necessidade de gerenciar servidores (Patching e manutenção de sistema operacional), o Lambda reduz a "superfície de ataque". A segurança é baseada no princípio do privilégio mínimo através do **AWS IAM** (Identity and Access Management), onde cada função só tem permissão para acessar exatamente o que precisa para sua tarefa, minimizando riscos de vazamento.

## Conclusão
A implementação de tecnologias AWS na **Golden Order** traz uma evolução necessária para a competitividade da empresa. Espera-se uma redução de custos operacionais através da eliminação de hardware físico e uma melhora significativa na conformidade com normas como a LGPD e padrões internacionais de saúde. A migração para a nuvem não é apenas uma economia financeira, mas uma blindagem tecnológica para o capital intelectual da empresa.


**Assinatura do Responsável pelo Projeto:**

_________________________________________________  
**Lucas Galvano de Paula**