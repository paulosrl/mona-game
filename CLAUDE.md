# CLAUDE.md — Mona's Octoverse Arcade (mona-game)

Regras só deste repositório. As comuns a todo projeto estão em `trilha-ai/CLAUDE-comum.md`, importado abaixo.

@trilha-ai/CLAUDE-comum.md

## O que é

Um jogo de navegador para o desafio "Mona's Octoverse Arcade" do GitHub Day of Learning: Mona, a Octogata, coleta quadrados verdes de commit e desvia de bugs vermelhos, com Copilot como ajudante que dá uma dica a cada 10 pontos. Entrega-se como extensão de canvas do Copilot App, julgada por uma banca (rubrica de 25 pontos no README do desafio).

Origem do starter: `ghlearn/day-of-learning-challenge`, commit `958b903` (2026-10-30), copiado para `.github/extensions/monas-octoverse-arcade-starter/`; as regras do desafio estão em https://github.com/ghlearn/day-of-learning-challenge/blob/main/README.md e no guia https://ghlearn.github.io/monas-octoverse-arcade/

## Documentos

- Em `sdd/`: PRD `prd-mona-game.md` · TDD `tdd-mona-game.md` · decomposição `decomposicao-mona-game.md` · briefings `briefing-openspec/briefing-change-NN-*.md` · a página `documentacao.html` · os padrões técnicos `padroes-tecnicos.md`, ponto de partida do TDD.
- Contexto e regras por artefato do OpenSpec: `openspec/config.yaml`. Onde o trabalho parou: `ANDAMENTO.md`.

## Comandos

```bash
scripts/check.sh    # a parte fixa (trilha-ai/verifica.sh: regras, método, specs) e, depois da etapa 2, lint, tipos e testes
# rodar: abrir o repositório como Project no Copilot App e pedir "Open the Mona's Octoverse Arcade starter canvas";
# fora dele, abrir .github/extensions/monas-octoverse-arcade-starter/game.html direto no navegador
```

## Regras de código

- O jogo é só `game.html`, com HTML, CSS e JavaScript puro: sem `package.json`, dependências, assets externos nem etapa de build (regra do desafio).
- O `extension.mjs` do starter não muda: ele registra o canvas e serve o `game.html`.
- <ferramentas de teste e de lint, definidas no TDD; elas não podem virar dependência do jogo>.

## Dados a proteger

- As credenciais da conta do GitHub Hands-on Labs nunca entram no repositório, no vídeo de demonstração nem na submissão.

## Armadilhas próprias

- Nenhuma ainda.

## Exceções ao comum

- Nenhuma.
