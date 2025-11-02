# Arquitetura AWS com EC2, S3, Lambda e EBS

## 📌 Descrição do Projeto

Este repositório documenta a arquitetura e os aprendizados do laboratório sobre gerenciamento de instâncias EC2 na AWS, conforme o desafio proposto pela DIO.

O objetivo é aplicar conceitos de computação em nuvem, especialmente sobre instâncias EC2, armazenamento EBS, uso de S3 e integração com AWS Lambda.

---

## 🏗️ Arquitetura da Solução

A solução proposta utiliza os seguintes componentes AWS:

* **Amazon EC2** – Instância responsável por hospedar a aplicação.
* **Amazon EBS** – Volume de armazenamento persistente anexado à instância EC2.
* **Amazon S3** – Bucket para armazenar artefatos estáticos e logs.
* **AWS Lambda** – Função responsável por processar eventos e automatizar tarefas.

### Fluxo Resumido

1. Usuário acessa a aplicação hospedada na instância EC2.
2. A EC2 lê e grava dados no volume EBS.
3. Arquivos estáticos ou uploads são armazenados no S3.
4. Um evento no S3 aciona uma função Lambda para processamento automático.

> ✅ Diagrama da arquitetura foi criado utilizando **Draw.io** e está disponível na pasta `/architecture`.

---

## 📂 Estrutura do Repositório

```
/architecture
  └── aws-architecture.drawio
/images
  └── aws-architecture.drawio.png
README.md
```

---

## 🧠 Insights e Aprendizados

* Diferença entre armazenamento local da EC2 e volumes EBS.
* Boa prática: usar S3 para armazenar arquivos estáticos.
* Lambda pode automatizar rotinas sem provisionar servidor.
* Importância de documentar arquitetura para reuso e estudo.

---

## 🚀 Como Reproduzir

1. Criar bucket S3
2. Provisionar EC2 com Linux
3. Criar e anexar EBS à instância
4. Configurar Lambda para evento de `ObjectCreated` no S3

---

## 🛠️ Tecnologias Utilizadas

* AWS EC2
* AWS EBS
* AWS S3
* AWS Lambda
* Draw.io
* GitHub

---

## 📎 Documentações Úteis

* Guia EC2 AWS
* Documentação Amazon S3
* Documentação AWS Lambda
* Markdown GitHub

---

## ✅ Conclusão

Este projeto consolida os fundamentos de instâncias EC2 e integra outros serviços essenciais da AWS, formando uma arquitetura escalável e moderna.

> 📍 Esta documentação faz parte do desafio prático DIO: *Gerenciamento de EC2 na AWS*.

---

## 👩‍💻 Autora

Projeto desenvolvido por Amanda — Engenharia de Computação & IA.

LinkedIn: linkedin.com/in/amanda-justen-80b17182
