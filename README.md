# aws-cloud-practitioner-lab-streaming
Laboratório prático de implementação de servidor de streaming no AWS Lightsail para consolidação de conceitos da certificação AWS Cloud Practitioner (CLF-C02).

#  Laboratório Prático: AWS Cloud Practitioner (CLF-C02)

Este repositório documenta a aplicação prática dos conceitos estudados para a certificação **AWS Certified Cloud Practitioner**, utilizando um cenário real de implementação de infraestrutura de mídia.

##  Objetivos de Aprendizado (Conceitos da Certificação)
O projeto foi desenhado para validar os pilares do **AWS Well-Architected Framework**:

* **Excelência Operacional:** Automatização do deploy do Ant Media Server em instâncias Linux.
* **Segurança:** Implementação de Grupos de Segurança (Firewall stateful) e gestão de acesso via Key Pairs (SSH).
* **Eficiência de Performance:** Seleção de instâncias baseada em carga de processamento de vídeo (Transcoding).
* **Otimização de Custos:** Comparação entre modelos SaaS e infraestrutura autogerenciada no AWS Lightsail.

##  Serviços AWS Utilizados
* **Amazon Lightsail:** VPS para hospedagem da aplicação (Compute).
* **VPC & Networking:** Configuração de regras de entrada/saída (Inbound/Outbound) para portas RTMP (1935) e HTTP (5080).
* **Identity and Access Management (IAM):** Gerenciamento de chaves privadas (.pem) para acesso administrativo seguro.

##  Troubleshooting & Insights de Estudo
Durante o laboratório, analisei o comportamento do sistema de arquivos e permissões Linux. Enfrentei um desafio de indexação de arquivos via SFTP, o que me permitiu explorar mais profundamente a interação entre a camada de aplicação e o storage do OS, consolidando conceitos de persistência de dados.

---
*Projeto realizado como parte da trilha de estudos para a AWS Certified Cloud Practitioner.*
