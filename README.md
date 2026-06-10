# 🚀 AWS EC2 Lab - Gerenciamento de Instâncias na AWS

> Repositório desenvolvido como parte do desafio prático de AWS EC2, com foco na criação, configuração, monitoramento e gerenciamento de instâncias na nuvem utilizando os serviços da AWS.

[![AWS](https://img.shields.io/badge/AWS-EC2-FF9900?style=for-the-badge&logo=amazonaws)](#aws)
[![Cloud](https://img.shields.io/badge/Cloud-Computing-4285F4?style=for-the-badge)](#computação-em-nuvem)
[![GitHub](https://img.shields.io/badge/GitHub-Documentation-181717?style=for-the-badge&logo=github)](#documentação)
[![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)](#conclusão)
---

## 📌 Sobre o Projeto

Este laboratório teve como objetivo explorar os principais recursos do serviço **Amazon EC2 (Elastic Compute Cloud)**, permitindo a criação e gerenciamento de servidores virtuais na nuvem.

Durante a prática foram abordados conceitos essenciais relacionados à infraestrutura cloud, segurança, monitoramento e administração de instâncias.

---

## 🎯 Objetivos

- Criar e configurar instâncias EC2
- Gerenciar grupos de segurança (Security Groups)
- Configurar acesso remoto via SSH
- Monitorar recursos utilizando CloudWatch
- Aplicar boas práticas de segurança na AWS
- Documentar todo o processo utilizando GitHub

---

## 🏗️ Arquitetura do Projeto

```text
┌──────────────┐
│   Usuário    │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ Internet     │
└──────┬───────┘
       │
       ▼
┌─────────────────────┐
│ Security Group      │
│ Porta 22 (SSH)      │
│ Porta 80 (HTTP)     │
│ Porta 443 (HTTPS)   │
└──────┬──────────────┘
       │
       ▼
┌─────────────────────┐
│ Amazon EC2          │
│ Ubuntu Server       │
└──────┬──────────────┘
       │
       ▼
┌─────────────────────┐
│ Amazon CloudWatch   │
└─────────────────────┘
```
---

## ☁️ O que é Amazon EC2?

O Amazon EC2 é um serviço da AWS que permite criar e gerenciar servidores virtuais sob demanda.

### Benefícios

- Escalabilidade
- Alta disponibilidade
- Flexibilidade
- Baixo custo inicial
- Integração com diversos serviços AWS

---

## 🔧 Etapa 1 - Criação da Instância

### Configurações Utilizadas

| Configuração | Valor |
|-------------|--------|
| Sistema Operacional | Ubuntu Server |
| Tipo da Instância | t2.micro |
| Região | us-east-1 |
| Armazenamento | 8 GB SSD |
| Chave SSH | RSA |

### Processo

1. Acesso ao Console AWS
2. Seleção do serviço EC2
3. Criação da instância
4. Configuração do Security Group
5. Geração da chave SSH
6. Inicialização da instância

---

## 🔒 Etapa 2 - Configuração de Segurança

### Security Group

| Porta | Protocolo | Função |
|---------|---------|---------|
| 22 | TCP | SSH |
| 80 | TCP | HTTP |
| 443 | TCP | HTTPS |

### Boas Práticas

- Restringir acesso SSH por IP
- Utilizar autenticação por chave
- Evitar portas desnecessárias abertas
- Aplicar princípio do menor privilégio

---

## 💻 Etapa 3 - Conexão SSH

Comando utilizado:

```bash
ssh -i chave.pem ubuntu@IP_PUBLICO
```

Resultado esperado:

```bash
Welcome to Ubuntu
```

---

## 📊 Etapa 4 - Monitoramento

Utilizando Amazon CloudWatch foi possível monitorar:

- Uso de CPU
- Tráfego de rede
- Disco
- Status da instância
- Alarmes e eventos

---

## 🧠 Conceitos Aprendidos

### EC2

Serviço de computação em nuvem da AWS.

### AMI (Amazon Machine Image)

Modelo utilizado para criação de instâncias.

### Security Group

Firewall virtual responsável pelo controle de acesso.

### Key Pair

Par de chaves para autenticação SSH.

### Elastic IP

Endereço IP público fixo.

### CloudWatch

Ferramenta de monitoramento da AWS.

---

## 🚧 Desafios Encontrados

### Problema

Não foi possível conectar via SSH.

### Solução

- Verificação da chave privada
- Ajuste das permissões do arquivo .pem
- Validação das regras do Security Group

---

## 📈 Insights Obtidos

Durante o laboratório foi possível perceber como a computação em nuvem simplifica o provisionamento de infraestrutura, permitindo criar servidores em minutos sem a necessidade de investimento em hardware físico.

Além disso, ficou evidente a importância da segurança na configuração de grupos de acesso e do monitoramento contínuo dos recursos computacionais.

---

## 🖼️ Evidências

### Diagrama da Arquitetura

<div align="center">

## 🏗️ Diagrama da Arquitetura

<img src="images/diagrama-ec2.png" width="800"/>

</div>

---

## 📚 Recursos Utilizados

### AWS

- Amazon EC2
- Amazon CloudWatch
- IAM
- Security Groups

### Ferramentas

- GitHub
- Git
- Draw.io
- Visual Studio Code

---

## 🔗 Referências

- https://docs.aws.amazon.com/ec2/
- https://docs.aws.amazon.com/cloudwatch/
- https://docs.github.com/
- https://aws.amazon.com/training/

---

## 👨‍💻 Autor

**Gabriel Monteiro**

Estudante de Engenharia | Dados | Inteligência Artificial | Cloud Computing

### Conecte-se comigo

- GitHub: https://github.com/Monteiro-01
- LinkedIn: https://linkedin.com/in/
---

## ⭐ Conclusão

Ao concluir este laboratório, foi possível compreender o ciclo completo de gerenciamento de instâncias EC2, desde o provisionamento até o monitoramento, aplicando conceitos fundamentais de infraestrutura em nuvem e boas práticas de segurança.

Este projeto servirá como material de apoio para futuras implementações e estudos relacionados à computação em nuvem, DevOps e arquitetura AWS.
