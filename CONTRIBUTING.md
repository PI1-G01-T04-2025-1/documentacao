# 🤝 Contribuindo com o Projeto Oásis

Olá! 👋  

Este documento orienta sobre as boas práticas e padrões que seguimos no repositório.

- 📝 [Padrão de Commits](#-padrão-de-commits)
- 📜 [Histórico de Versões](#-histórico-de-versões)

## Regras gerais de contribuição
- Sempre criar branches específicas para cada funcionalidade ou correção.
- Seguir o padrão de commits descrito.
- Atualizar a documentação se necessário.
- Realizar testes antes de enviar Pull Requests.


## 📝 Padrão de Commits

Este projeto adota o padrão baseado no **Conventional Commits** para manter um histórico de mudanças limpo e organizado.  
Todos os colaboradores devem seguir esse modelo ao realizar commits.

### 🧾 Como configurar o `.gitmessage`

Para facilitar o uso do padrão de commits, recomendamos configurar um **template de mensagem de commit** com `.gitmessage`. Isso ajuda a lembrar a estrutura correta sempre que fizer um commit.

#### ⚙️ Passos para configuração

1. Crie um arquivo no seu diretório local:

```bash
touch ~/.gitmessage
```

2. Abra e edite o arquivo com o conteúdo indicado:

```bash
nano ~/.gitmessage
```

Conteúdo para o template:

```text
# <tipo>(escopo opcional): mensagem breve
# Linha em branco
# Corpo da mensagem (opcional, explique o que e por quê)

# Tipos:
# feat     -> nova funcionalidade
# fix      -> correção de bug
# docs     -> mudanças na documentação
# style    -> formatação, espaços, ponto e vírgula etc.
# refactor -> refatoração de código
# test     -> testes adicionados ou modificados
# chore    -> tarefas gerais (ex: configs)

# Exemplo:
# feat(interface): adiciona gráfico de posição
```

3. Configure o Git para usar esse arquivo:

```bash
git config --global commit.template ~/.gitmessage
```

Ou, se quiser configurar **apenas para este repositório**:

```bash
git config --local commit.template .gitmessage
```

4. Usando o template

Sempre que for fazer um commit, basta rodar:

```bash
git commit
```

O Git abrirá automaticamente seu editor configurado com o conteúdo do `.gitmessage`.
Você só precisa preencher ou ajustar a mensagem conforme o padrão.

Perfeito! Aqui está um **texto explicativo** para adicionar ao `CONTRIBUTING.md` ou ao final da documentação, explicando como manter o **Histórico de Versões**:

<br>

## 📜 Histórico de Versões

O **Histórico de Versões** serve para documentar as principais alterações realizadas nas documentações do projeto ao longo do tempo, garantindo **rastreabilidade** e **transparência** sobre as mudanças feitas.

### Como utilizar

1. Sempre que fizer uma alteração relevante (ex.: inclusão de novas seções, ajustes em histórias de usuário ou modificações estruturais), adicione uma nova linha na tabela de **Histórico de Versões**.

2. Inclua as seguintes informações:

   * **Versão**: use o padrão incremental (ex.: 1.1, 1.2, ...).
   * **Data**: data da alteração.
   * **Descrição**: explique brevemente o que foi alterado.
   * **Autor(es)**: coloque seu nome ou link para seu perfil no Github.

#### Exemplo:

```markdown
| Versão | Data | Descrição | Autor(es) | 
| -- | -- | -- | -- |
|`1.0`|17/05/2025| Modelagem do BPMN | [Carlos Rodrigues](https://github.com/Carlos-kadu) e [Rayene Almeida](https://github.com/rayenealmeida) |
```
