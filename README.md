# Explorando-a-Infraestrutura-AWS-EC2-EBS-e-S3
 Bootcamp DIO - Santander: Conhecendo os Serviços de Computação e Armazenamento AWS
 Este repositório documenta a minha jornada de aprendizado no módulo sobre AWS do Bootcamp oferecido pela DIO em parceria com o Santander. O foco principal foi explorar os fundamentos dos serviços de computação e armazenamento em nuvem da Amazon.

📚 O Que Aprendi
Parte 1: Amazon EC2 (Elastic Compute Cloud)
Iniciei meus estudos compreendendo o EC2, o serviço de computação em nuvem da AWS. A didática clara do instrutor foi fundamental para dissipar a complexidade inicial e revelar a simplicidade e poder por trás do serviço. Os tópicos explorados incluem:

Conceito de máquinas virtuais (instâncias) sob demanda.

Modelos de custos (sob demanda, reserved, spot).

Estratégias para otimização de recursos.

Casos de uso e aplicações no dia a dia.

Parte 2: Armazenamento na AWS - EBS & S3
Avancei para os módulos de armazenamento, essenciais para qualquer infraestrutura:

Amazon EBS (Elastic Block Store):
Entendi o EBS como um sistema de armazenamento em blocos, análogo a um disco rígido virtual. Aprendi sobre sua flexibilidade para ser anexado e desanexado de instâncias EC2, a possibilidade de criar múltiplos volumes e o seu papel crucial como solução de backup e para a criação de sistemas de arquivos particionados.

Amazon S3 (Simple Storage Service):
Explorei o serviço de armazenamento de objetos, famoso por sua alta durabilidade, segurança e escalabilidade. Aprendi sobre as diferentes classes de armazenamento (Standard, Glacier, etc.) e a importante estratégia do Ciclo de Vida dos Objetos, que automatiza a transição de dados entre classes com base na frequência de acesso (ex.: mover para Glacier após 90 dias sem uso), otimizando significativamente os custos.

🧠 Desafio de Arquitetura: Aplicação Prática
Como parte do módulo, foi proposto um desafio de arquitetura para aplicar na prática os conceitos aprendidos. Para resolvê-lo, projetei uma solução para um cenário do mundo real.

Cenário: Uma grande construtora que precisa gerenciar seus projetos, documentos e dados.

Solução Proposta:
Utilizei EC2 para hospedar aplicações críticas, como softwares de gestão de projetos e ERP. O EBS foi configurado como o disco principal dessas instâncias, garantindo performance e permitindo snapshots para backup rápido. Já o S3 foi empregado para armazenar de forma segura e organizada toda a documentação da empresa (projetos, contratos, imagens de obra), com políticas de ciclo de vida automático para arquivar documentos antigos na classe Glacier, reduzindo custos sem perder acessibilidade.

Esta arquitetura demonstra como os serviços AWS trabalham de forma integrada para criar soluções robustas, escaláveis e econômicas.


