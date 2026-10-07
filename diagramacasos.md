# 👥 Diagrama de Casos de Uso

O diagrama de casos de uso apresenta as principais interações dos dois tipos de usuários com o sistema Apoia+.

```mermaid
flowchart LR
    Pessoa["🧓 Pessoa Assistida"]
    Voluntario["🙋 Voluntário"]

    subgraph Apoia+["Apoia+"]
        UC1(("Cadastrar-se"))
        UC2(("Realizar login"))
        UC3(("Gerenciar perfil"))
        UC4(("Criar solicitação"))
        UC5(("Acompanhar solicitação"))
        UC6(("Visualizar candidaturas"))
        UC7(("Selecionar voluntário"))
        UC8(("Finalizar solicitação"))

        UC9(("Visualizar solicitações"))
        UC10(("Consultar detalhes"))
        UC11(("Candidatar-se"))
        UC12(("Acompanhar candidaturas"))
        UC13(("Visualizar serviços realizados"))
    end

    Pessoa --> UC1
    Pessoa --> UC2
    Pessoa --> UC3
    Pessoa --> UC4
    Pessoa --> UC5
    Pessoa --> UC6
    Pessoa --> UC7
    Pessoa --> UC8

    Voluntario --> UC1
    Voluntario --> UC2
    Voluntario --> UC3
    Voluntario --> UC9
    Voluntario --> UC10
    Voluntario --> UC11
    Voluntario --> UC12
    Voluntario --> UC13
```

## Atores

### 🧓 Pessoa Assistida

Usuário que necessita de auxílio para realizar uma tarefa ou pequeno serviço.

### 🙋 Voluntário

Usuário que disponibiliza seu tempo e suas habilidades para ajudar outras pessoas.
