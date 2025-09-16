name: Bug Report
description: Registrar um bug encontrado
title: "[Bug]: "
labels: ["bug"]
projects: ["ztrax-ofc/2"]
assignees:
  - mateusdreher-ztrax
body:
  - type: input
    id: reporter
    attributes:
      label: Nome de quem encontrou o bug
      placeholder: ex. Claudio Cleiton
    validations:
      required: true
  - type: textarea
    id: what-happened
    attributes:
      label: Descreva o erro
      description: Descrição precisa e detalhada do erro
    validations:
      required: true
  - type: dropdown
    id: project
    attributes:
      label: Projeto
      description: Qual projeto o bug ocorreu
      options:
        - Tracing Precisão
        - Tracing Presença
        - Rondas
        - Rondas chat
        - Pausa térmica
      default: 0
    validations:
      required: true
  - type: dropdown
    id: env
    attributes:
      label: Qual ambiente o bug ocorreu
      options:
        - Produção
        - Desenvolvimento
        - Demonstração
  - type: textarea
    id: steps
    attributes:
      label: Passos para reproduzir
      description: DEscreva os passos para reproduzir o erro.
