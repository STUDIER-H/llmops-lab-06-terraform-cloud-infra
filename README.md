# 🧪 LAB 06: Infraestrutura como Código (IaC) com Terraform na AWS para GPU

## 🎯 Objetivo do Lab
Automatizar o ciclo de vida de recursos de infraestrutura em nuvem utilizando Terraform de forma modular e segura.

---

## 📋 Pré-requisitos
- Ter concluído *Infrastructure as Code with Terraform Foundations* (Coursera).
- Terraform CLI 1.5+, conta na AWS.

---

## 🛠️ O que você deve construir neste Lab:

### Etapa 1: Arquitetura Modular HCL
1. Estruture o código em módulos (`modules/vpc`, `modules/ec2_gpu`, `modules/s3`).
2. Defina os arquivos `main.tf`, `variables.tf`, `outputs.tf` e `terraform.tfvars`.

### Etapa 2: Estado Remoto & Locking
1. Configure o backend do Terraform no arquivo `provider.tf` utilizando um bucket S3 para o arquivo `terraform.tfstate` e uma tabela DynamoDB para State Locking.

---

## ✅ Critérios de Aceitação & Entrega
- [ ] `terraform plan` executado com sucesso gerando o plano de execução sem erros.
- [ ] Recursos criados na AWS comprovados por `terraform apply` limpo.
