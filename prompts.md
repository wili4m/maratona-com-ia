# Prompts de IA - Bootcamp DevOps

Este documento contém todos os prompts de IA identificados no roteiro do Bootcamp DevOps com IA na Prática.

## 🐳 Prompts para Docker

### 1. Criação de .dockerignore
```
Com base no projeto e no @src/Dockerfile, crie o arquivo .dockerignore junto do Dockerfile
```
**Explicação**: Prompt para criar um arquivo .dockerignore otimizado baseado na estrutura do projeto e no Dockerfile existente.
**Objetivo**: Excluir arquivos desnecessários do contexto de build do Docker

### 2. Melhorias no Dockerfile
```
Analise o projeto @src e avalie o @src/Dockerfile em relação a qualidade 
e possíveis melhorias. 
Liste as melhorias que podem ser feitas e o Dockerfile com as implementações sugeridas.
```
**Explicação**: Prompt para análise crítica e otimização de um Dockerfile existente.
**Objetivo**: Identificar e implementar melhorias de performance, segurança e boas práticas

### 3. Dockerfile para Projeto Principal
```
Analise o projeto e crie o arquivo Dockerfile e o arquivo .dockerignore para a aplicação ser executadaem containers Docker.
O comando Docker build será executado dentro da pasta @src
```
**Explicação**: Prompt para criar do zero os arquivos Docker necessários para containerizar a aplicação.
**Objetivo**: Containerizar a aplicação principal do bootcamp

## 🤖 Prompts para Claude Code - Docker

### 1. Listagem de Containers
```
Liste os containers em execução
```
**Explicação**: Comando simples para visualizar containers ativos no Docker.
**Objetivo**: Monitoramento básico de containers

### 2. Análise de Logs
```
Analise como está a execução do container com o postgresql. Com base nos logs tem algum erro ?
```
**Explicação**: Prompt para análise diagnóstica de um container específico através de logs.
**Objetivo**: Troubleshooting e diagnóstico de problemas

### 3. Criação de Container
```
Execute um container usando a imagem nginx e com um publish de porta 8080:80
```
**Explicação**: Comando para criar e executar um container com configuração específica de porta.
**Objetivo**: Demonstrar criação de containers com mapeamento de portas

### 4. Remoção de Container
```
Remova o container que executa o postgresql
```
**Explicação**: Comando para remover um container específico em execução.
**Objetivo**: Limpeza e gerenciamento de containers

## ☸️ Prompts para Kubernetes

### 1. Criação de Manifesto
```yaml
Analise o projeto e crie o arquivo de manifesto para fazer o deploy da aplicação em ambientes Kubernetes.
O manifesto deve ser criado dentro de uma pasta k8s no repositório e em um único arquivo yaml. É importante que o banco de dados postgre vai ser criado externamente em um banco de dados gerenciado.

Utilize apenas deployment e services, as variáveis de ambiente vão ser definidas diretamente no yaml e o mínimo de configuração.
```
**Explicação**: Prompt complexo para criar manifesto Kubernetes com especificações detalhadas.
**Objetivo**: Deploy da aplicação no Kubernetes com configuração mínima

### 2. Listagem de Nodes
```
Liste os nodes do cluster Kubernetes
```
**Explicação**: Comando para visualizar os nodes do cluster Kubernetes.
**Objetivo**: Verificação da infraestrutura do cluster

### 3. Listagem de Pods
```
Liste os pods do cluster Kubernetes
```
**Explicação**: Comando para visualizar todos os pods em execução no cluster.
**Objetivo**: Monitoramento de aplicações no cluster

## 🔍 Prompt Complexo - Análise de Cluster

### Análise Completa de Cluster Kubernetes
```markdown
# Prompt para Análise Completa de Cluster Kubernetes

## Função
Você é um especialista em Kubernetes e DevOps responsável por analisar clusters Kubernetes e fornecer insights sobre infraestrutura, aplicações e otimizações.

## Objetivo
Realizar uma análise completa e detalhada do cluster Kubernetes conectado, identificando o estado atual da infraestrutura, aplicações em execução, configurações de segurança e oportunidades de melhoria.

## Contexto
Você tem acesso ao cluster Kubernetes através do MCP (Model Context Protocol) de Kubernetes. Use este acesso para coletar informações em tempo real sobre todos os aspectos do cluster, incluindo nodes, pods, services, deployments.

## Tarefa
Execute as seguintes análises usando o MCP de Kubernetes:

### 1. Inventário de Infraestrutura
- Liste todos os nodes do cluster com suas especificações (CPU, memória, sistema operacional)
- Verifique o status e saúde dos nodes
- Identifique a versão do Kubernetes em uso
- Analise o uso de recursos (CPU, memória, armazenamento) por node

### 2. Análise de Aplicações e Workloads
- Liste todas as aplicações existentes
- Liste todos os deployments, pods e services em execução
- Verifique o status dos pods e identificar pods com problemas

### 3. Configurações de Rede e Serviços
- Liste todos os services e seus tipos.
- Identifique serviços expostos externamente

## Saída
Forneça um relatório estruturado em markdown contendo:

### Resumo Executivo
- Status geral do cluster (saudável/problemático)
- Principais descobertas
- Prioridades de ação

### Detalhes da Infraestrutura
- Especificações dos nodes
- Versões e compatibilidade
- Utilização de recursos atual

### Inventário de Aplicações
- Lista consolidada de aplicações por namespace
- Status de cada aplicação
- Configurações de recursos

### Recomendações de Otimização
Organize as recomendações por prioridade:

#### Alta Prioridade (Crítico)
- Problemas que afetam estabilidade ou segurança

#### Média Prioridade (Importante)
- Otimizações de performance e eficiência

#### Baixa Prioridade (Desejável)
- Melhorias de best practices e governança

### Próximos Passos
- Ações imediatas recomendadas
- Plano de implementação das melhorias
- Métricas para acompanhamento
```

**Explicação**: Prompt estruturado seguindo metodologia FOCUS (Função, Objetivo, Contexto, Tarefa, Saída) para análise profunda de clusters Kubernetes.
**Objetivo**: Realizar auditoria completa e fornecer insights acionáveis sobre o cluster

---

## 📋 Resumo

- **Total de prompts**: 8 prompts simples + 1 prompt complexo
- **Categorias**: Docker (3), Claude Code (4), Kubernetes (3), Análise Avançada (1)
- **Finalidade**: Automação de tarefas DevOps através de IA
- **Aplicação**: Bootcamp prático de DevOps com integração de IA