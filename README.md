# claude-code-tools

Repositório de plugins para o [Claude Code](https://docs.anthropic.com/en/docs/claude-code). Contém o plugin **novo-projeto-plugin**, que disponibiliza a skill `/novo-projeto` para inicializar qualquer repositório com um sistema completo de governança persistente.

---

## O que é a skill `/novo-projeto`

A skill executa um bootstrap completo de governança em um repositório vazio. Após a execução, o repositório passa a ter:

- `CLAUDE.md` com instruções operacionais persistentes
- `.claude/rules/` com 12 regras normativas de comportamento
- `.claude/skills/` com 6 skills especializadas
- `.claude/hooks/` com artefatos de reforço operacional
- `Instructions/` com memória arquitetural, de negócio, BDD, contratos, glossário, decisões e snippets canônicos
- `open-questions.md` e `assumptions-log.md` para rastreamento de dúvidas e premissas

A partir do bootstrap, mensagens simples em linguagem natural são suficientes para que o Claude interprete, classifique, consulte a governança acumulada e execute corretamente.

---

## Pré-requisitos

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) instalado (`npm install -g @anthropic-ai/claude-code`)
- Git instalado e configurado

---

## Instalação do plugin em um repositório novo

### 1. Adicione este repositório como fonte de plugins

No repositório onde você quer usar a skill, adicione a referência ao plugin no arquivo `.claude/settings.json`:

```json
{
  "plugins": [
    {
      "source": "github:AlbertKellner/claude-code-tools/plugins/novo-projeto-plugin"
    }
  ]
}
```

> Se o arquivo `.claude/settings.json` não existir, crie-o na raiz do seu repositório.

### 2. (Alternativa) Instale manualmente copiando a skill

Se preferir não usar o mecanismo de plugins, copie o arquivo da skill diretamente:

```bash
# Na raiz do seu repositório
mkdir -p .claude/skills/novo-projeto
curl -sSL https://raw.githubusercontent.com/AlbertKellner/claude-code-tools/main/plugins/novo-projeto-plugin/skills/novo-projeto/SKILL.md \
  -o .claude/skills/novo-projeto/SKILL.md
```

Ou clone este repositório e copie localmente:

```bash
git clone https://github.com/AlbertKellner/claude-code-tools.git
cp -r claude-code-tools/plugins/novo-projeto-plugin/skills/novo-projeto \
      SEU_REPOSITORIO/.claude/skills/novo-projeto
```

---

## Como usar a skill

### Em um repositório vazio (uso principal)

1. Abra o Claude Code no repositório alvo:

```bash
cd meu-novo-repositorio
claude
```

2. Execute a skill com o comando:

```
/novo-projeto
```

O Claude irá executar o bootstrap completo, criando toda a estrutura de governança descrita acima.

### O que acontece durante o bootstrap

- O Claude cria a estrutura de pastas e arquivos de governança
- Todos os arquivos recebem conteúdo operacional real (sem placeholders vazios)
- As regras em `.claude/rules/` passam a governar todas as interações futuras no repositório
- Após o bootstrap, o repositório evolui com base no seu próprio contexto acumulado

---

## Uso cotidiano após o bootstrap

Depois do bootstrap, não é necessário usar comandos especiais. Mensagens em linguagem natural são suficientes:

```
adicione uma nova regra de negócio para pedidos com desconto
```

```
crie o BDD para o fluxo de cancelamento
```

```
implemente o endpoint de listagem de clientes
```

O Claude vai automaticamente:
1. Interpretar semanticamente a mensagem
2. Consultar a governança do repositório
3. Verificar ambiguidades antes de agir
4. Atualizar a governança quando necessário
5. Implementar seguindo as fontes de verdade do repositório

---

## Estrutura do plugin

```
plugins/novo-projeto-plugin/
├── .claude-plugin/
│   └── plugin.json          # Metadados do plugin
└── skills/
    └── novo-projeto/
        └── SKILL.md         # Prompt completo de bootstrap
```

---

## Contribuição

Abra uma issue ou pull request em [github.com/AlbertKellner/claude-code-tools](https://github.com/AlbertKellner/claude-code-tools).
