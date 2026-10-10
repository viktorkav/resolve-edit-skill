# resolve-edit-skill

Skill em português para orientar um agente de IA na edição de vídeos de fala no DaVinci Resolve: organização, seleção de tomadas, corte inicial, áudio, imagens de apoio e revisão.

O arquivo da skill é [resolve-editar/SKILL.md](resolve-editar/SKILL.md). Ele não depende de identidade visual, presets ou plugins de terceiros.

## Usar

1. Baixe o arquivo `SKILL.md` e coloque-o na pasta de skills do seu agente. No Claude Code, por exemplo: `.claude/skills/resolve-editar/SKILL.md` no projeto. No Codex: `.agents/skills/resolve-editar/SKILL.md` no projeto.
2. Abra o DaVinci Resolve com os brutos e o projeto de trabalho. Para o agente executar operações, configure um conector MCP compatível ou o scripting oficial da Blackmagic, conforme sua versão e edição do Resolve.
3. Peça ao agente para usar a skill `resolve-editar`, informando o projeto, a timeline, os arquivos de origem e o resultado desejado.

Exemplo: “Use resolve-editar para montar uma primeira versão deste vídeo. Preserve a timeline original, selecione as tomadas pela fala gravada e mantenha o áudio sincronizado. Depois, revise os cortes e salve uma timeline editável.”

A skill descreve o procedimento; não instala ferramentas nem inclui um transcritor. Quando uma operação não estiver disponível, o agente deve apontar a etapa manual necessária. A montagem precisa de revisão audiovisual antes da entrega.

## Licença

MIT. Não afiliado à Blackmagic Design.
