# AGENTS.md

## Regra obrigatória de coordenação

Antes de qualquer alteração:
1. Leia `PROJECT_STATE.md`.
2. Leia a documentação e artefatos diretamente relacionados à tarefa.
3. Verifique `main`, PRs e commits recentes quando houver risco de trabalho concorrente.

Depois de qualquer alteração que mude estado, decisão, bloqueador, versão ou próximo passo:
1. Atualize `PROJECT_STATE.md` no mesmo commit/PR.
2. Preserve distinção entre FACT, DECISION, IN PROGRESS, BLOCKED, PROPOSAL e DONE.
3. Não converta proposta ou versão numericamente mais alta em canônico sem prova funcional/clínica.

O repositório é a fonte canônica. Histórico de chats, memória de agentes e handoffs externos são contexto auxiliar, nunca autoridade para o estado atual.
