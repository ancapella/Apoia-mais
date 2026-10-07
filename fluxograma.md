# 🔄 Fluxograma do Apoia+

```mermaid
flowchart TD
    A([Início]) --> B[Login / Cadastro]
    B --> C{Tipo de usuário}

    C -->|Pessoa Assistida| D[Criar solicitação]
    D --> E[Publicar solicitação]

    C -->|Voluntário| F[Visualizar solicitações]
    E --> F

    F --> G[Selecionar solicitação]
    G --> H[Enviar candidatura]
    H --> I{Candidatura aceita?}

    I -->|Não| F
    I -->|Sim| J[Voluntário selecionado]

    J --> K[Realizar ajuda]
    K --> L[Encerrar solicitação]
    L --> M([Fim])
```

## Descrição

O fluxo inicia com o cadastro ou login do usuário. Após o acesso, o sistema identifica se o usuário é uma **pessoa assistida** ou um **voluntário**.

A pessoa assistida pode criar e publicar uma solicitação de ajuda. Os voluntários podem visualizar as solicitações disponíveis e se candidatar àquelas que possuem interesse ou habilidade para realizar.

Após receber as candidaturas, a pessoa assistida escolhe um voluntário. A ajuda é então realizada e a solicitação é encerrada.
