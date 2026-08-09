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
- Em 2026-08-09 foi recebido fisicamente `rechtrauma_fluxo_explicado (2)(2).html`; o arquivo contém marcação visual `Visual trauma v24`, portanto existe evidência de uma variante posterior à v23, mas isso NÃO estabelece que seja a versão clínica canônica.
- SHA-256 de `rechtrauma_fluxo_explicado (2)(2).html`: `ffbe5dd9ae2a510b4b6b3838e257a19a2ac55389ff3c885a9fe4ca880c412f19`.

## DECISION
- Preservar v12 como referência histórica.
- Tratar v23 e a variante `fluxo_explicado` com marcação v24 como candidatas, NÃO como releases canônicas até diff/auditoria.
- Não descartar nenhuma variante física antes da reconciliação.

## IN PROGRESS
- Migração dos artefatos físicos para o GitHub.
- Inventário de variantes e relação de derivação entre v12, v23, variante v24 e arquivos intermediários.

## BLOCKED
- Falta comparar v12 → v23 → variante v24 funcional e clinicamente.
- Falta auditoria de fórmulas, thresholds, doses, contraindicações e referências atuais.
- Falta validação por cenários antes de uso assistencial.

## CANDIDATES LOCATED
- `rechtrauma_fluxo_explicado (2)(2).html` — variante física com marcação visual v24; SHA-256 registrado acima.
- `rechtrauma_v23.html` — candidata previamente localizada.
- `rechtrauma_copiloto_v12.html` — versão v12 comprovada.
- Outras variantes na Library: PCR/pós-PCR, ROSC/PaCO2, fontes macro, rastreabilidade, hotfix clínico visual e outras; ainda não reconciliadas.

## NEXT
1. Migrar fisicamente os HTMLs relevantes para o GitHub sem alterar conteúdo.
2. Atualizar `MIGRATION_MANIFEST.md` com hashes e origem.
3. Diff dirigido v12 ↔ v23 ↔ variante v24.
4. Eleger baseline/canônico somente após auditoria e testes.

## REGRA DE SINCRONIZAÇÃO
Qualquer agente (ChatGPT/Codex, Claude, Copilot ou outro) que altere o projeto deve atualizar este arquivo no mesmo commit/PR quando a alteração mudar estado, decisão, bloqueador ou próximo passo.
