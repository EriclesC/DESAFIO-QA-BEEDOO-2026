# Relatório de Bugs – Desafio QA Beedoo

## Resumo de Bugs Encontrados

| Módulo | Quantidade |
|------|------|
| Cadastro de cursos | 5 |
| Listagem de cursos | 3 |
| Exclusão de cursos | 1 |
| **Total** | **9** |

---

# Bugs — Cadastro de Cursos

## Bug 01 — Sistema permite cadastrar curso com número de vagas negativo

**Passos para reproduzir:**
1. Acessar a tela de cadastro de curso
2. Informar um número negativo no campo "Número de vagas"
3. Preencher os demais campos
4. Clicar em salvar

**Resultado atual:**
O sistema permite salvar o curso com número de vagas negativo.

**Resultado esperado:**
O sistema deve impedir valores negativos no campo "Número de vagas".

**Severidade:**
Alta

**Evidências:**
https://drive.google.com/drive/folders/1wt_k1VBtzyY82MYoe3GnhDSreRU2Zjj8

---

## Bug 02 — Sistema permite cadastrar curso com data anterior à data atual

**Passos para reproduzir:**
1. Acessar a tela de cadastro de curso
2. Informar uma data de início e fim anterior à data atual
3. Preencher os demais campos
4. Clicar em salvar

**Resultado atual:**
O sistema permite cadastrar cursos com datas anteriores à data atual.

**Resultado esperado:**
O sistema deve validar as datas e impedir cadastro com datas inválidas.

**Severidade:**
Média

**Evidências:**
https://drive.google.com/drive/folders/1tpB58_gTFDQpnhAu-a2hOpE_OwPNUdd_

---

## Bug 03 — Sistema permite cadastrar curso sem preencher o formulário

**Passos para reproduzir:**
1. Acessar a tela de cadastro de curso
2. Deixar todos os campos vazios
3. Clicar em salvar

**Resultado atual:**
O sistema permite cadastrar o curso sem preencher nenhuma informação.

**Resultado esperado:**
O sistema deve exigir o preenchimento dos campos obrigatórios antes de permitir o cadastro.

**Severidade:**
Alta

**Evidências:**
https://drive.google.com/drive/folders/17uOtV6boHq60-1RtfEIzPVOv4CFU5meV
---

## Bug 04 — Campos de texto não possuem limite de caracteres e quebram o layout

**Passos para reproduzir:**
1. Acessar a tela de cadastro de curso
2. Inserir um texto muito grande nos campos "Nome do curso", "Descrição do curso" e "Instrutor"
3. Salvar o curso
4. Acessar a listagem

**Resultado atual:**
Os textos ultrapassam o limite visual e quebram o layout da página.

**Resultado esperado:**
Os campos devem possuir limite de caracteres ou tratamento de layout para evitar quebra da interface.

**Severidade:**
Média

**Evidências:**
https://drive.google.com/drive/folders/1gKlq3sNn7N87f_NfOdDdD0GeaR16ijb1
---

## Bug 05 — Sistema permite cadastrar curso com data final menor que a data inicial

**Passos para reproduzir:**
1. Acessar a tela de cadastro de curso
2. Informar uma data inicial
3. Informar uma data final menor que a data inicial
4. Preencher os demais campos
5. Clicar em salvar

**Resultado atual:**
O sistema permite salvar o curso mesmo com a data final menor que a data inicial.

**Resultado esperado:**
O sistema deve validar as datas e impedir cadastro quando a data final for menor que a data inicial.

**Severidade:**
Alta

**Evidências:**
https://drive.google.com/drive/folders/1fS9w3h9u8D770c5u2Q8EDpQl7iNZfC6w
---

# Bugs — Listagem de Cursos

## Bug 06 — Campos de data desalinhados na listagem

**Passos para reproduzir:**
1. Acessar a página de listagem de cursos
2. Observar os campos "Data inicial" e "Data final"

**Resultado atual:**
Os campos aparecem desalinhados na tabela de listagem.

**Resultado esperado:**
Os campos devem estar alinhados corretamente conforme o layout da página.

**Severidade:**
Baixa

**Evidências:**

---

## Bug 07 — Sistema não exibe mensagem quando não existem cursos cadastrados

**Passos para reproduzir:**
1. Acessar a aplicação sem possuir cursos cadastrados
2. Navegar para a página de listagem de cursos

**Resultado atual:**
A página é exibida sem nenhuma informação e sem mensagem ao usuário.

**Resultado esperado:**
O sistema deve exibir uma mensagem informando que não existem cursos cadastrados.

**Severidade:**
Média

**Evidências:**
https://drive.google.com/drive/folders/1VNAoltHZPYvllFo9_206aag2GlW9VbWZ
---

## Bug 08 — Informação do instrutor não é exibida na listagem de cursos

**Passos para reproduzir:**
1. Cadastrar um curso informando o nome do instrutor
2. Acessar a página de listagem de cursos

**Resultado atual:**
A informação do instrutor não é exibida na listagem.

**Resultado esperado:**
A listagem deve exibir corretamente a informação do instrutor para cada curso.

**Severidade:**
Média

**Evidências:**
Link do Google Drive

---

# Bugs — Exclusão de Cursos

## Bug 09 — Botão excluir curso não remove o curso da listagem

**Passos para reproduzir:**
1. Acessar a listagem de cursos
2. Clicar no botão "Excluir curso"
3. Confirmar a exclusão

**Resultado atual:**
O sistema exibe a mensagem "Curso excluído com sucesso", porém o curso continua na listagem.

**Resultado esperado:**
O curso deve ser removido da listagem após a exclusão.

**Severidade:**
Alta

**Evidências:**
https://drive.google.com/drive/folders/1XbDVfX_d4gzLIG-YanyojHDtcK1Wt3r7
