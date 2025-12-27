# 👋 Sobre este GitHub

Este perfil é organizado como um **portfólio técnico** focado em **arquitetura de software, cloud computing e engenharia de plataformas**.

Os repositórios aqui não representam produtos finais, mas sim **estudos estruturados, laboratórios técnicos e componentes reutilizáveis**, criados para explorar decisões arquiteturais, trade-offs e padrões aplicáveis a sistemas reais e complexos.

---

## 📦 Tipos de Repositórios

### 🧱 Sandboxes — Casos Arquiteturais Completos

```text
sandbox-<tema>-platform[-ano]
```

- Casos de estudo end-to-end
- Arquitetura documentada (C4, ADRs)
- Integração entre front-end, back-end e processamento
- Infraestrutura como código
- Foco em padrões arquiteturais, não em produto

### 🧪 Labs — Estudos Técnicos Focados

```text
lab-<tecnologia>-<tema>
```

- Exploração profunda de uma tecnologia, ferramenta ou padrão
- Spikes, POCs e experimentos direcionados
- Escopo intencionalmente limitado

### 🎮 Playgrounds — Experimentos Rápidos

```text
playground-<stack>
```

- Exploração livre e rápida de ideias
- Sem compromisso com arquitetura final ou documentação extensa
- Espaço para aprendizado incremental

### ☁️ Infraestrutura como Código (Terraform)
```text
terraform-<provider>-<resource>
```

- Módulos reutilizáveis de Terraform
- Isolados por responsabilidade
- Pensados para composição, versionamento e reuso

### 🤖 Automação com GitHub Actions
```text
gha-<action-name>
```

- Actions reutilizáveis (composite ou JS)
- Automação de build, qualidade, segurança e release

### Workflows reutilizáveis
```text
gh-workflow-<workflow-name>
```

- Workflows baseados em workflow_call
- Padronização de CI/CD entre múltiplos repositórios

## 🧠 Domínio de Negócio

Alguns sandboxes utilizam domínios reais (ex: crédito imobiliário) como contexto de aplicação.

O domínio é utilizado apenas como cenário realista para exercitar arquitetura e engenharia.

Os padrões e decisões explorados são transferíveis para diversos setores, como seguros, marketplace, logística e plataformas internas.

## 🧭 Princípios e Filosofia

- Arquitetura antes da ferramenta
- Contratos antes da implementação
- Infraestrutura como código, não como script
- Decisões explícitas e registradas (ADRs)
- Evolução incremental, consciente e documentada

## 📌 Como Navegar por este GitHub

1. Comece pelos repositórios de ```sandboxes```
2. Leia o README e os demais doocumentos do repositório (e.g. ARCHITECTURE.md e os ADRs)
3. Observe os códigos da aplicaçõe, infraestrutura e como elas se conectam com as decisões