# MELHORIA-001 — Campos de nome aceitam apenas números sem validação de formato

## Informações

| Campo | Valor |
|-------|-------|
| ID | MELHORIA-001 |
| Módulo | Cadastro Administração Pública |
| Funcionalidade | Validação dos campos Nome do órgão e Nome do representante |
| Severidade | Baixa |
| Prioridade | Baixa |
| Ambiente | Ambiente público disponível ao usuário |
| Navegador | Brave |
| Sistema Operacional | Windows 11 |
| Status | Aberto |

---

## Descrição

Os campos "Nome do órgão" e "Nome do representante" aceitam valores compostos exclusivamente por números (ex.: "12345"), sem qualquer validação de formato. Para o campo "Nome do representante", isso é incoerente, pois nomes de pessoas não contêm dígitos. Para o campo "Nome do órgão", embora números sejam válidos em muitos nomes (ex.: "9º Batalhão de Polícia Militar"), um valor sem nenhuma letra não representa um nome de órgão válido.

---

## Pré-condições

- Usuário acessando a página de Cadastro Administração Pública.
- Campos de texto disponíveis para preenchimento.

---

## Passos para reprodução

1. Acessar a página de Cadastro Administração Pública.
2. Preencher o campo "Nome do órgão" com "12345".
3. Preencher o campo "Nome do representante" com "12345".
4. Preencher os demais campos obrigatórios.
5. Observar que nenhuma mensagem de erro ou bloqueio é exibido nos campos de nome.

---

## Resultado esperado

- **Nome do representante:** aceitar apenas letras (incluindo acentos), espaços, apóstrofo e hífen, preferencialmente exigindo nome e sobrenome.
- **Nome do órgão:** exigir ao menos uma letra e um tamanho mínimo, permitindo números e símbolos usuais em nomes de órgãos (ex.: "º", "-", "()").
- Em ambos os casos, exibir mensagem de erro clara quando o valor informado for inválido.

---

## Resultado obtido

Ambos os campos aceitam "12345" sem exibir qualquer mensagem de erro ou impedimento.

---

## Impacto

Permite o envio de cadastros com dados claramente inválidos, o que pode gerar retrabalho para a equipe responsável pela validação (contato do analista em até 24h) e reduzir a qualidade dos dados registrados no sistema.

---

## Evidências

- [Vídeo](https://github.com/user-attachments/assets/f1a302a2-7015-4188-9fdb-ffb342ec409c)
