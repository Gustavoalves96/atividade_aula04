# Engenharia de Software II - Prática de Git

Projeto de demonstração para a disciplina de Engenharia de Software II
(Prof. Wagner Loch), usado para praticar controle de versão com Git e
programação orientada a objetos em TypeScript.

A aplicação é um menu de terminal que simula o funcionamento básico de um
veículo: acelerar, frear, trocar de marcha e exibir os dados.

## Tecnologias

- TypeScript
- Node.js + ts-node
- prompt-sync (entrada de dados pelo terminal)

## Como executar

Pré-requisito: Node.js instalado.

```bash
git clone https://github.com/Gustavoalves96/atividade_aula04.git
cd atividade_aula04
npm install
npm start
```

Para apenas compilar o projeto:

```bash
npm run build
```

## Estrutura

| Arquivo | Descrição |
| --- | --- |
| `index.ts` | Menu principal e funções de operação do veículo |
| `Veiculo.ts` | Classe `Veiculo` com os atributos do modelo |
| `requisitos.MD` | Lista de requisitos a implementar |

## Requisitos

O andamento da implementação é acompanhado em [requisitos.MD](requisitos.MD).

## Fluxo de trabalho com Git

O repositório usa três níveis de branch:

- `main` — versão estável do projeto
- `dev` — integração do trabalho da equipe
- `feature/nome-da-funcionalidade` - desenvolvimento de cada funcionalidade

Cada integrante cria sua branch a partir da `dev`, desenvolve a funcionalidade
e abre um Pull Request de volta para a `dev`.

```bash
git checkout dev
git pull
git checkout -b feature/minha-funcionalidade
```

Ao concluir, envie a branch e abra o Pull Request tendo a `dev` como base:

```bash
git push -u origin feature/minha-funcionalidade
```

## Equipe

- Gustavo Alves
