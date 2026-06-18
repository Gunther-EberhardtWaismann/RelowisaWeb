# RELOWISA - Plataforma Web para Dimensionamento de Sistemas Puxados BPS

## Visão Geral

A RELOWISA será uma plataforma web desenvolvida para apoiar o dimensionamento de sistemas puxados conforme a metodologia Bosch Production System (BPS).

A proposta visa substituir o modelo atual baseado em planilhas eletrônicas descentralizadas por uma solução centralizada, segura, rastreável e escalável, hospedada em ambiente Microsoft Azure.

A plataforma buscará padronizar os cálculos RELOWISA, aumentar a confiabilidade dos resultados, melhorar a governança dos dados e viabilizar a aplicação estruturada do ciclo PDCA nos processos de manufatura.

---

# Problema

Atualmente, os cálculos necessários para o dimensionamento de supermercados e Kanbans são realizados por meio de planilhas eletrônicas distribuídas entre diferentes usuários.

Esse cenário gera diversos desafios operacionais e de governança, tais como:

- Existência de múltiplas versões da mesma planilha;
- Falta de rastreabilidade das alterações realizadas;
- Possibilidade de erros em fórmulas e referências;
- Dificuldade de manutenção e expansão das soluções;
- Ausência de uma base única de dados;
- Limitações para auditoria e controle de acesso;
- Dependência excessiva de conhecimento individual.

Diante desse contexto, surge a necessidade de uma solução corporativa capaz de centralizar e padronizar o processo de cálculo.

---

# Objetivo Geral

Desenvolver uma plataforma web centralizada para execução dos cálculos RELOWISA, proporcionando:

- Maior confiabilidade dos resultados;
- Governança de dados;
- Rastreabilidade das operações;
- Controle de acesso por perfis;
- Integração com iniciativas de melhoria contínua;
- Redução da dependência de planilhas eletrônicas.

---

# Objetivos Específicos

- Centralizar os dados em um banco de dados corporativo;
- Automatizar os cálculos da metodologia RELOWISA;
- Implementar mecanismos de auditoria e rastreabilidade;
- Disponibilizar relatórios e históricos de cálculo;
- Integrar a solução ao ciclo PDCA;
- Permitir simulações e análises comparativas;
- Garantir conformidade com requisitos corporativos de segurança.

---

# Escopo da Solução

A plataforma proposta deverá contemplar os seguintes módulos:

## Gestão de Materiais

- Cadastro de materiais;
- Classificação de itens;
- Gestão de parâmetros produtivos.

## Gestão de Recursos

- Cadastro de máquinas;
- Gestão de capacidades;
- Parametrização de tempos operacionais.

## Gestão de Loops Produtivos

- Criação de loops de produção;
- Associação de materiais e recursos;
- Controle de parâmetros de cálculo.

## Calendário de Produção

- Cadastro de turnos;
- Cadastro de feriados;
- Planejamento de dias úteis;
- Configuração de capacidade produtiva.

## Motor de Cálculo RELOWISA

- Cálculo automatizado das parcelas RE, LO, WI e SA;
- Armazenamento dos resultados;
- Simulações de cenários.

## Gestão PDCA

- Registro de ações;
- Controle de responsáveis;
- Acompanhamento de melhorias;
- Histórico de resultados.

---

# Metodologia RELOWISA

O sistema implementará a metodologia RELOWISA para dimensionamento de Kanbans:

```text
K = RE + LO + WI + SA
```

Onde:

| Componente | Descrição |
|------------|------------|
| RE | Cobertura do Tempo de Reposição |
| LO | Cobertura para Formação de Lote |
| WI | Cobertura para Flutuações de Demanda |
| SA | Cobertura para Riscos Operacionais |

O resultado representará a quantidade necessária de Kanbans para suportar o sistema puxado.

---

# Arquitetura Proposta

## Frontend

A interface será desenvolvida utilizando:

- React
- SAP Fundamental Styles
- Design responsivo

## Backend

A camada de negócio será desenvolvida utilizando:

- Python
- Framework Bottle
- API REST

## Banco de Dados

Será utilizado:

- Azure SQL Database

## Autenticação

A autenticação será realizada através de:

- Azure Active Directory
- OAuth 2.0
- OpenID Connect

---

# Infraestrutura Azure

A solução será hospedada utilizando serviços gerenciados da Microsoft Azure:

| Serviço | Objetivo |
|----------|----------|
| Azure App Service | Hospedagem do backend |
| Azure Static Web Apps | Hospedagem do frontend |
| Azure SQL Database | Persistência de dados |
| Azure Active Directory | Gestão de identidade |
| Azure Monitor | Monitoramento |
| Application Insights | Telemetria |
| Azure Key Vault | Gestão de segredos |
| Azure DevOps | CI/CD |

---

# Segurança

A plataforma será projetada considerando os princípios de segurança corporativa:

- Criptografia TLS 1.3;
- Controle de acesso baseado em funções (RBAC);
- Integração com Azure AD;
- Registro de auditoria;
- Backups automatizados;
- Gestão segura de credenciais.

Além disso, o projeto buscará aderência às recomendações de:

- ISO 27001;
- OWASP Top 10;
- NIST Cybersecurity Framework.

---

# Benefícios Esperados

Com a implantação da plataforma, espera-se:

## Operacionais

- Eliminação das planilhas descentralizadas;
- Redução de erros de cálculo;
- Padronização dos processos;
- Menor esforço de manutenção.

## Gerenciais

- Melhor rastreabilidade;
- Maior visibilidade dos resultados;
- Histórico consolidado de informações;
- Melhor suporte à tomada de decisão.

## Técnicos

- Escalabilidade;
- Alta disponibilidade;
- Governança de dados;
- Arquitetura moderna baseada em nuvem.

---

# Roadmap Futuro

Possíveis evoluções da solução incluem:

- Integração com SAP ERP;
- Integração com sistemas MES;
- Dashboards em Power BI;
- Simulações avançadas;
- Aplicação de Machine Learning para previsão de demanda;
- Expansão para múltiplas plantas industriais.

---

# Status do Projeto

Proposta Conceitual

Este repositório tem como objetivo documentar a proposta, arquitetura, requisitos e planejamento da futura Plataforma Web RELOWISA.

---

# Autor

**Günther Ebehardt Waismann**

Projeto de Engenharia de Software aplicado à Engenharia de Manufatura e Sistemas Produtivos.
