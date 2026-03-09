# Desafio QA – Beedoo - Ericles Carvalho

## Objetivo

Realizar a análise da aplicação disponibilizada, identificar cenários de teste relevantes e registrar possíveis defeitos encontrados durante a execução dos testes.

---

# Análise inicial da aplicação

A aplicação analisada consiste em um sistema simples de gerenciamento de cursos, permitindo ao usuário realizar operações básicas de CRUD.

Durante a análise inicial foram identificadas as seguintes funcionalidades principais:

- Cadastro de cursos
- Listagem de cursos cadastrados
- Exclusão de cursos

A interface da aplicação apresenta:

- Um formulário para cadastro de novos cursos
- Uma listagem exibindo os cursos cadastrados
- Um botão de exclusão para cada curso listado

Com base nessa estrutura, foi possível identificar o fluxo principal da aplicação.

### Fluxo principal da aplicação

1. Usuário cadastra um curso
2. O curso aparece na listagem
3. O usuário pode remover o curso da listagem

A partir desse fluxo principal foram definidos os cenários de teste.

---

# Estratégia de testes

A estratégia de testes foi definida com foco em garantir a qualidade das funcionalidades principais da aplicação.

Os testes foram organizados por **módulos funcionais**, permitindo melhor rastreabilidade e organização:

- Cadastro de cursos
- Listagem de cursos
- Exclusão de cursos

Para cada módulo foram criados cenários contemplando:

- Fluxo principal
- Validações de campos
- Comportamentos esperados da interface
- Possíveis entradas inválidas

Também foram considerados **cenários negativos**, com o objetivo de identificar comportamentos inesperados da aplicação.

---


# Decisões tomadas para criação dos testes

Algumas decisões foram tomadas durante a elaboração dos cenários de teste:

### Organização por funcionalidade

Os testes foram agrupados por funcionalidade para facilitar a identificação de defeitos e a manutenção da documentação.

### Priorização baseada no fluxo do usuário

Os cenários de teste foram priorizados considerando o fluxo mais comum de utilização da aplicação:

- criação de cursos
- visualização na listagem
- exclusão de cursos

### Escrita de cenários em BDD

Os cenários foram documentados utilizando o formato **BDD (Given / When / Then)**, pois esse formato facilita:

- leitura
- entendimento do comportamento esperado
- comunicação entre áreas técnicas e de negócio

---


# Raciocínio durante a análise

Durante a análise da aplicação, o primeiro passo foi compreender o comportamento esperado do sistema a partir da interface disponível.

Com base nisso, foram identificados os principais pontos de validação:

- comportamento correto do formulário de cadastro
- exibição adequada das informações na listagem
- atualização da interface após ações do usuário
- consistência dos dados após exclusões

Além disso, foram explorados cenários que poderiam revelar falhas na aplicação, como:

- cadastro com informações inválidas
- inconsistências na atualização da listagem
- possíveis falhas na remoção de cursos

Durante a execução dos testes foram identificados alguns comportamentos inesperados, que foram documentados no relatório de bugs.

---

# Cobertura de testes

Os cenários de teste foram elaborados cobrindo os seguintes aspectos:

| Tipo de teste | Descrição |
|-----|-----|
| Fluxo principal | Cadastro, listagem e exclusão de cursos |
| Validação de campos | Verificação de entradas válidas e inválidas |
| Testes negativos | Tentativas de uso da aplicação com dados inesperados |
| Comportamento da interface | Atualização da listagem após ações do usuário |

---

# Casos de teste

Os cenários de teste foram documentados em formato BDD na planilha abaixo:

https://docs.google.com/spreadsheets/d/169U1EWwIMZQPWpBQxrp0hg8pgERAw-tfc6F7f7IOXps/edit?usp=sharing

A planilha contém:

- descrição do cenário
- passos do teste
- resultado esperado
- status da execução
- prioridade
- referência para bugs encontrados

---

# Relatório de bugs

Os defeitos identificados durante a execução dos testes estão documentados no arquivo:

https://github.com/EriclesC/DESAFIO-QA-BEEDOO-2026/blob/main/bugs.md

Cada bug contém:

- título
- passos para reprodução
- resultado atual
- resultado esperado
- severidade
- evidências

---

# Evidências dos testes

As evidências da execução dos testes (prints e gravações) estão disponíveis no link abaixo:

https://drive.google.com/drive/folders/1vXLVH09ueRypOoSETVTi7mGrZTbF7guV

---

# Ambiente de testes

| Item | Detalhes |
|-----|-----|
| Aplicação testada | https://creative-sherbet-a51eac.netlify.app/ |
| Navegador | Google Chrome |
| Sistema operacional | Windows |
| Tipo de testes | Testes funcionais manuais |
| Data da execução | Março de 2026 |

---

# Resumo da execução de testes

| Métrica | Quantidade |
|------|------|
| Cenários de teste criados | 13 |
| Bugs encontrados | 9 |
| Funcionalidades testadas | 3 |

Funcionalidades avaliadas:

- Cadastro de cursos
- Listagem de cursos
- Exclusão de cursos
