# Guia de Contribuição - Livro de Receitas PacocaScript

Este documento define os padrões obrigatórios para a equipe, garantindo a rastreabilidade e a organização do projeto, conforme as diretrizes da atividade.

## 1. Padrões de Nomenclatura

### 1.1 Branches
Toda branch deve ser criada a partir da `main` atualizada e seguir o padrão:
*   **Formato:** `feature/<categoria>-<nome-da-receita>`
*   **Exemplo:** `feature/sobremesas-<nome-da-receita>`

### 1.2 Commits (Conventional Commits)
As mensagens devem indicar claramente o tipo de mudança:
*   `feat:` Para adicionar uma nova receita (ex: `feat: adicionar receita de <nome-da-receita>`).
*   `docs:` Para atualizar o menu ou documentação (ex: `docs: atualizar menu com link para <nome-da-receita>`).
*   `fix:` Para correções solicitadas no Code Review (ex: `fix: ajustar link do rodape`).

## 2. Regras para Abertura de Issues

Antes de começar a codificar, crie uma Issue com o título no formato `[Receita] <Nome> - <Categoria>` e utilize o modelo abaixo na descrição:

```markdown
# Descrição
O Livro de Receitas não possui a receita de <nome-da-receita> na categoria <categoria>.

Esperado:
- Arquivo `<categoria>/<nome-da-receita>.md` com a receita seguindo a estrutura pedida na atividade: título, seção de ingredientes listados, seção de modo de preparo numerada;
- Rodapé de navegação no fim do arquivo com links para voltar a sua categoria e para o `menu.md`;
- Link da receita na seção `Receitas` do `menu.md` .

# Critérios de Aceitação
- [ ] Arquivo <categoria>/<nome-da-receita>.md criado
- [ ] Receita com: titulo, seções de ingredientes e modo de preparo
- [ ] Rodapé com link para a categoria e para o menu principal
- [ ] Link no menu.md apontando para o arquivo da receita
- [ ] PR com 3 aprovações