# Fit-AI

## DOCUMENTAÇÃO DO PROJETO

### Sistema de Monitoramento de Treinos com IA

## 1. Visão Geral do Projeto
- 1.1 Nome do Projeto
  - Fit AI 

- 1.2 Descrição

  - O FitTrack AI é uma plataforma web (com possibilidade futura mobile) voltada para o acompanhamento de treinos físicos, evolução corporal e consistência do usuário, integrando Inteligência Artificial para fornecer recomendações personalizadas e sugestões de treino com base nos dados registrados.

- O sistema permitirá que usuários registrem seus treinos, acompanhem sua evolução ao longo do tempo e recebam insights inteligentes para melhorar seus resultados.

---

## 2. Objetivo do Projeto
- 2.1 Objetivo Geral
  - Desenvolver um sistema digital capaz de registrar, monitorar e analisar a evolução de treinos físicos, oferecendo suporte inteligente ao usuário por meio de IA.

- 2.2 Objetivos Específicos
  - Permitir o cadastro e gerenciamento de treinos;
  - Registrar execuções diárias de exercícios;
  - Monitorar evolução de peso e desempenho;
  - Gerar relatórios semanais de progresso;
  - Utilizar IA para sugerir treinos e melhorias;
  - Promover consistência e acompanhamento contínuo.

---
   
## 3. Problema que o Sistema Resolve

Atualmente, muitos usuários:

- não conseguem manter consistência nos treinos;
- não possuem controle claro da evolução;
- utilizam planilhas ou anotações desorganizadas;
- não sabem ajustar seus treinos conforme resultados.

O sistema resolve isso oferecendo:

- organização;
- histórico;
- análise de progresso;
- orientação inteligente.

---

## 4. Público-Alvo
- Pessoas que frequentam academia;
- Iniciantes que querem acompanhamento;
- Usuários intermediários que desejam evolução;
- Pessoas que buscam disciplina e consistência.

---

## 5. Domínio do Sistema

O sistema pertence ao domínio de:

- Fitness e Saúde
- Monitoramento de Performance
- Análise de Dados Pessoais
- Sistemas Inteligentes (IA aplicada)

---
  
## 6. Entidades do Domínio

Principais entidades do sistema:

- Usuário
- Perfil físico
- Objetivo (hipertrofia, emagrecimento, etc.)
- Treino
- Exercício
- Execução de treino
- Registro de peso
- Relatório
- Recomendações (IA)

---

## 7. Requisitos Funcionais
   
- 7.1 Usuário

  - RF01: O sistema deve permitir cadastro de usuário;
  - RF02: O sistema deve permitir login/autenticação;
  - RF03: O usuário deve poder editar seu perfil;
  - RF04: O usuário deve definir seu objetivo (ex: hipertrofia);

- 7.2 Treinos

  - RF05: O usuário deve poder cadastrar treinos;
  - RF06: O usuário deve poder definir exercícios dentro de um treino;
  - RF07: O usuário deve poder editar e excluir treinos;
  - RF08: O sistema deve permitir associar treinos a dias da semana;

- 7.3 Execução de Treinos

  - RF09: O usuário deve registrar execução diária de treino;
  - RF10: O usuário deve registrar séries, repetições e carga;
  - RF11: O sistema deve armazenar histórico de execuções;
  - RF12: O sistema deve permitir marcar treino como concluído;

- 7.4 Evolução Física

  - RF13: O usuário deve registrar seu peso por data;
  - RF14: O sistema deve armazenar histórico de peso;
  - RF15: O sistema deve exibir evolução do peso em gráfico;

- 7.5 Relatórios

  - RF16: O sistema deve gerar relatório semanal;
  - RF17: O relatório deve incluir frequência de treino;
  - RF18: O relatório deve incluir variação de peso;
  - RF19: O sistema deve apresentar dados de desempenho;

- 7.6 Inteligência Artificial

  - RF20: O sistema deve gerar sugestões de treino com base no objetivo;
  - RF21: O sistema deve fornecer recomendações com base no histórico;
  - RF22: O sistema deve gerar resumo semanal inteligente;
  - RF23: O sistema deve adaptar sugestões conforme comportamento do usuário;

---

## 8. Requisitos Não Funcionais

- 8.1 Desempenho
  - RNF01: O sistema deve responder em até 2 segundos para ações comuns;
  - RNF02: Relatórios devem ser gerados rapidamente (<3 segundos);
- 8.2 Usabilidade
  - RNF03: Interface deve ser simples e intuitiva;
  - RNF04: Registro de treino deve ser rápido (poucos cliques);
  - RNF05: Sistema deve ser responsivo (mobile-friendly);
- 8.3 Segurança
  - RNF06: Dados do usuário devem ser protegidos;
  - RNF07: Autenticação via JWT;
  - RNF08: Senhas devem ser criptografadas;
- 8.4 Escalabilidade
  - RNF09: Sistema deve suportar crescimento de usuários;
  - RNF10: Banco deve suportar grande volume de dados históricos;
- 8.5 Manutenibilidade
  - RNF11: Código deve ser organizado em camadas;
  - RNF12: Sistema deve permitir fácil adição de novas funcionalidades;

## 9.  Regras de Negócio

- RN01: Cada usuário possui seu próprio conjunto de treinos;
- RN02: Um treino pode conter múltiplos exercícios;
- RN03: Execução de treino deve ser armazenada separadamente do treino base;
- RN04: Peso deve ser registrado com data obrigatória;
- RN05: Relatórios devem considerar período semanal;
- RN06: Recomendações da IA devem considerar histórico do usuário;
- RN07: O sistema não deve sobrescrever dados históricos;
- RN08: Um treino pode ser executado múltiplas vezes;

## 10. Arquitetura do Sistema

- Camadas
- Front-end (Interface do usuário)
- Back-end (API)
- Banco de dados
- Serviço de IA (API externa)

Fluxo básico

Usuário → Front-end → API → Banco
↓
IA

## 11. Tecnologias Sugeridas

- Front-end
  -  React
  - Tailwind CSS
  - Recharts (gráficos)

- Back-end
  - Java (SpringBoot)

- Banco de dados
  - PostgreSQL

- IA
  - API de modelo de linguagem (para recomendações)

## 12. MVP (Produto Mínimo Viável)

O MVP deve conter:

- Cadastro e login;
- Cadastro de treinos;
- Registro de execução;
- Registro de peso;
- Histórico básico;
- Relatório semanal simples;

IA pode entrar como:

- geração básica de treino;
- resumo simples.

## 13. Diferenciais do Projeto

- Uso de IA com base em dados reais do usuário;
- Foco em consistência e evolução;
- Dashboard visual de progresso;
- Sistema adaptativo;
- Projeto completo fullstack + IA.

## 14. Riscos do Projeto

- Escopo muito grande;
- Complexidade na modelagem;
- IA superficial se mal implementada;
- UX ruim no registro de treino;
- Dificuldade em definir métricas de evolução;

## 15. Possíveis Evoluções Futuras

- App mobile;
- Integração com smartwatch;
- Sistema de metas;
- Notificações inteligentes;
- Gamificação (streaks);
- Comunidade/social;
- IA mais avançada (ajuste automático de treino);

## 16. Conclusão

O FitTrack AI é um projeto altamente relevante tanto para aprendizado quanto para portfólio, pois integra diversas áreas da engenharia de software, incluindo desenvolvimento fullstack, modelagem de dados, análise de informações e uso de inteligência artificial.

O projeto apresenta forte potencial de crescimento e permite evolução progressiva, tornando-se uma excelente base para aprofundamento técnico e construção de um produto digital completo.
