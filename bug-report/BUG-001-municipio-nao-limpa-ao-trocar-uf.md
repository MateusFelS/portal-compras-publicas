# BUG-001 — Município permanece selecionado ao trocar a UF no cadastro

## Informações

| Campo | Valor |
|-------|-------|
| ID | BUG-001 |
| Módulo | Cadastro Administração Pública |
| Funcionalidade | Seleção de UF e Município |
| Severidade | Média |
| Prioridade | Média |
| Ambiente | Ambiente público disponível ao usuário |
| Navegador | Brave |
| Sistema Operacional | Windows 11 |
| Status | Aberto |

---

## Descrição

Ao alterar a UF após já ter selecionado um município, o campo Município não é limpo e continua exibindo o município da UF anterior. Com isso, o formulário fica em um estado inconsistente (ex.: UF = MS com município = Acrelândia), e o botão CADASTRAR permanece desabilitado sem qualquer mensagem informando o motivo.

---

## Pré-condições

- Usuário acessando a página de Cadastro Administração Pública.
- Campos UF e Município disponíveis para edição.

---

## Passos para reprodução

1. Acessar a página de Cadastro Administração Pública.
2. Selecionar a UF "AC".
3. Selecionar o município "Acrelândia".
4. Trocar a UF para "MS".
5. Observar o campo Município e o estado do botão CADASTRAR.

---

## Resultado esperado

Ao trocar a UF, o campo Município deve ser limpo automaticamente e a lista de municípios deve ser recarregada de acordo com a nova UF selecionada, mantendo o mesmo comportamento já existente no sistema de filtro e busca da plataforma. Caso haja algum campo inválido, o sistema deve exibir uma mensagem clara indicando o problema.

---

## Resultado obtido

O município "Acrelândia" continua selecionado mesmo com a UF "MS". O botão CADASTRAR fica desabilitado e nenhuma mensagem de erro ou orientação é exibida ao usuário.

---

## Impacto

O formulário permite um estado inválido (município que não pertence à UF), o usuário não entende por que não consegue concluir o cadastro e a plataforma apresenta comportamento inconsistente entre o cadastro e o filtro de busca, prejudicando a usabilidade e a acessibilidade.

---

## Evidências

- [Vídeo](https://github.com/user-attachments/assets/bf881902-463a-44fd-9625-3e35b5a3ba30)
