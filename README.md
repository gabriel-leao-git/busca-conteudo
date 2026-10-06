# busca-conteudo

Skill de IA para Claude Code (e outros agentes compatíveis) que funciona como um **radar de oportunidades de conteúdo**. Ela pesquisa a web, acha notícias, lançamentos, tendências e vídeos outliers, e transforma isso em oportunidades prontas para executar, com ângulo, hook, formato, plataforma, viral score, risco e próxima ação.

Feita para o posicionamento **"Eu construo, testo e mostro"** do Gabriel Leão.

## Instalação

Requer Node.js (para o `npx`).

```bash
npx skills add gabriel-leao-git/busca-conteudo
```

Por padrão a skill é instalada no projeto atual. Variações úteis:

```bash
# instalar globalmente (disponível em todos os projetos)
npx skills add gabriel-leao-git/busca-conteudo -g

# instalar só para o Claude Code
npx skills add gabriel-leao-git/busca-conteudo -a claude-code

# ver o que o repositório oferece, sem instalar
npx skills add gabriel-leao-git/busca-conteudo --list
```

Depois de instalar, abra uma nova sessão do Claude Code para a skill ser carregada.

## Como usar

Não precisa chamar a skill pelo nome. Ela dispara quando o pedido é sobre ideias de conteúdo. Exemplos:

- "me dá conteúdo pra hoje"
- "quero algo pro TikTok sobre cybersecurity"
- "achei esse vídeo bombando [link], quero usar de referência"
- "o que está rolando fora da bolha tech que eu posso abordar?"
- "encontre vídeos outliers sobre IA"
- "quero algo que eu possa construir e transformar em conteúdo"

## O que tem aqui

```
.claude/skills/content-opportunity-radar/
├── SKILL.md                      # fluxo de trabalho, regras e formato de saída
└── references/
    ├── scoring.md                # viral score, penalidades, critérios de aceitação
    ├── editorial-lenses.md       # camadas editoriais, segunda ordem, conflito, experimento
    ├── platforms-and-formats.md  # TikTok, Reels, carrossel, Shorts, YouTube e formatos
    ├── modes.md                  # os 8 modos de pedido (geral, nicho, referência, outliers...)
    ├── cross-niche.md            # interseções entre tecnologia e outras áreas
    └── examples.md               # exemplos de saída
```

## Observação

A skill depende de ferramenta de busca na web para trabalhar com tendências atuais. Sem acesso à web, ela avisa e marca o que veio de memória.

## Licença

Veja [LICENSE](LICENSE).
