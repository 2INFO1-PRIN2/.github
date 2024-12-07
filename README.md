# **Padrões de Commit**

Os commits devem ser escritos **em inglês** no seguinte formato:  
`<Classificação>:<mensagem de commit><# da issue>`

### **Exemplo**

FEAT: Innital commit #01

O commit semântico possui os seguintes **elementos estruturais (tipos)**, que indicam a intenção ao utilizador(a) do código:

---

### **Classificação de Commit**

- **`feat`**  
  Inclui um **novo recurso** no código.  
  _(Relacionado ao **MINOR** do versionamento semântico)._

- **`fix`**  
  Soluciona um problema (**bug fix**).  
  _(Relacionado ao **PATCH** do versionamento semântico)._

- **`docs`**  
  Indica mudanças na **documentação**, como alterações no README.  
  _(Não inclui modificações em código)._

- **`test`**  
  Modifica ou cria **testes unitários**.  
  _(Não inclui alterações em código)._

- **`build`**  
  Relaciona-se a alterações em **arquivos de build e dependências**.

- **`perf`**  
  Identifica alterações de código relacionadas à **performance**.

- **`style`**  
  Refere-se a **formatações de código** (e.g., semicolons, trailing spaces, lint).  
  _(Não inclui alterações funcionais no código)._

- **`refactor`**  
  Indica **refatorações** que não alteram funcionalidades.  
  _(Exemplo: melhorar o desempenho ou a estrutura do código)._

- **`chore`**  
  Indica **atualizações de tarefas** administrativas ou de build.  
  _(Exemplo: adicionar pacotes no `.gitignore`)._

- **`ci`**  
  Aponta mudanças relacionadas à **integração contínua** (_continuous integration_).

- **`raw`**  
  Refere-se a alterações em **configurações, dados, features ou parâmetros**.

- **`cleanup`**  
  Remoção de **código comentado ou desnecessário**, aprimorando a legibilidade.

- **`remove`**  
  Indica a exclusão de **arquivos, diretórios ou funcionalidades obsoletas**.

---

# **Utilização de Issues**

### **Título da Issue**

O título deve seguir o padrão do commit final gerado pela conclusão da Issue.

Os titulos devem ser escritos **em inglês** no seguinte formato:  
`<Classificação>:<título da Issue>`

### Exemplo:

FEAT: Create sidebar component

### **Resumo**

Apresente brevemente o objetivo daquela tarefa.

## **Descrição**

Descreva o que precisa ser feito ou corrigido, em detalhes de maneira clara.

- A descrição deve ser feita em **inglês**.

## **Informações Adicionais**

- **Assignees** (_responsável pela realização da Issue_)
- **Label** (_legenda relacionada ao responsável da Issue_): `FRONTEND` |
  `SVG` |
  `BACKEND` |
  `DESIGN` |
  `DOCS` |

- **Priority** (_prioridade para a realização da Issue_):
  `HIGH` | `MEDIUM` |`LOW`

- **Status** (_Fase de desenvolvimento da Issue_):
  `Backlog` | `Ready` |`In progress` | `Done`

---

---

# **Utilização de Pull Requests**

### **Título do Pull Request**

O título deve seguir o padrão do commit principal realizado durante a implementação.

Os títulos devem ser escritos **em inglês** no seguinte formato:  
`<Classificação>:<descrição do Pull Request>`

### **Exemplo:**

### **Resumo**

Apresente uma descrição breve sobre o propósito e impacto do Pull Request.

---

## **Descrição**

Detalhe as alterações realizadas de forma clara e objetiva:

- **Funcionalidades implementadas**
- **Bugs corrigidos**
- **Melhorias de código**
- **Refatorações**

> A descrição deve ser feita em **inglês**.

---

## **Informações Adicionais**

- **Reviewers:** (\_pessoas responsáveis pela revisão das alterações realizas)
- **Assignees:** (_pessoas responsáveis pelas alterações realizadas_)
- **Label:** (_categoria relacionada às mudanças realizadas_):
  - `FRONTEND`
  - `SVG`
  - `BACKEND`
  - `DESIGN`
  - `DOCS`

---

## Prática

1.Selecione a aba `Pull requests`em seu repositório:

![Minha Imagem](<./images/PR(1).png>)

2.Após isso, selecione a branch de onde você deseja realizar o pull para a branch que você realizará o push:

- No exemplo estamos realizando o pull da branch `add-badges-to-readme` para a branch `main`.
- Ou seja, comparando os arquivos de `add-badges-to-readme` com os da `main`.

![Minha Imagem](<./images/PR(2).png>)

03.Depois disso, adicione as propriedades desejada em seu Pull Request

- Neste exemplo, foi adicionado propriedade aos campos `Reviwers`, `Assignees`, `Labels` e `Projects`.

![Minha Imagem](<./images/PR(3).png>)

4.Após a aprovação dos usuários predefinidos como `Reviwers`, confirme o `merge` das branchs e o `Pull request estará concluído`.

![Minha Imagem](<./images/PR(4).png>)

# **Glossário 📖**

- **`Issues`**  
  Ferramenta usada para gerenciar tarefas, pedidos de novos recursos e correções de bugs em projetos de código aberto. As issues devem ser descritas e listadas, permitindo aos colaboradores discutirem e rastrearem o progresso das mesmas.

- **`Pull requests`**  
  Mecanismo usado para submeter alterações propostas ao repositório original. Um pull request é uma solicitação para que os mantenedores do projeto revisem e potencialmente incorporem as alterações. O pull request passará por um processo de avaliação e pode ser aceito ou rejeitado.

- **`Merge`**  
  Processo de unir mudanças de uma ramificação (branch) à outra em um repositório Git. O merge combina históricos de commits distintos, incorporando alterações feitas em diferentes ramificações, geralmente como parte de um pull request ou resolução de conflitos de código.
