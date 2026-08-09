# RechTrauma — PROJECT STATE

Última atualização: 2026-08-09
Branch canônica: `main`
Status: ARTEFATOS RECUPERADOS / RECONCILIAÇÃO PENDENTE

> O repositório e este documento são a fonte canônica do estado do projeto. Não confiar em resumos de chats para determinar status atual.

## FACT
- O repo existia vazio até esta migração.
- A varredura física da Library recuperou múltiplos artefatos RechTrauma.
- Artefatos confirmados incluem `rechtrauma_copiloto_v12.html` e `rechtrauma_v23.html`.
- `rechtrauma_copiloto_v12.html` declara internamente `RechTrauma Copiloto v12`.
- `rechtrauma_v23.html` declara na interface `Documento atual: v23 sem fundo` e contém XABCDE longitudinal, eFAST, Shock Index/SIA, ABC Score, RTS, PTM/DCR, neuro, airway e módulos adicionais.
- A existência de v23 invalida o antigo bloqueador documental "v12 não localizado"; porém ainda não prova que v23 seja clinicamente canônica.

## DECISION
- Preservar v12 como referência histórica.
- Tratar v23 como candidata mais recente localizada, NÃO como release canônica até diff/auditoria.
- Não descartar nenhuma variante física antes da reconciliação.

## IN PROGRESS
- Migração dos artefatos físicos para o GitHub.
- Inventário de variantes e relação de derivação entre v12, v23 e arquivos intermediários.

## BLOCKED
- Falta comparar v12 → v23 funcional e clinicamente.
- Falta auditoria de fórmulas, thresholds, doses, contraindicações e referências atuais.
- Falta validação por cenários antes de uso assistencial.

## CANDIDATES LOCATED
- `rechtrauma_v23.html` — candidata mais recente localizada.
- `rechtrauma_copiloto_v12.html` — versão v12 comprovada.
- Outras variantes na Library: fluxo explicado, PCR/pós-PCR, ROSC/PaCO2, fontes macro, rastreabilidade, hotfix clínico visual e outras; ainda não reconciliadas.

## NEXT
1. Concluir migração física dos HTMLs relevantes.
2. Gerar manifesto com hashes.
3. Diff dirigido v12 ↔ v23.
4. Eleger baseline/canônico somente após auditoria e testes.

## REGRA DE SINCRONIZAÇÃO
Qualquer agente (ChatGPT/Codex, Claude, Copilot ou outro) que altere o projeto deve atualizar este arquivo no mesmo commit/PR quando a alteração mudar estado, decisão, bloqueador ou próximo passo.
