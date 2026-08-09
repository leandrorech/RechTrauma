# RechTrauma — Migration Manifest

Data da varredura: 2026-08-09
Origem: ChatGPT File Library + upload direto do usuário
Status: MIGRAÇÃO EM ANDAMENTO

## Artefatos físicos localizados

### Candidatas principais
- `rechtrauma_v23.html` — localizado; 79.032 bytes; interface declara `Documento atual: v23 sem fundo`; 787 linhas.
- `rechtrauma_copiloto_v12.html` — localizado; 60.580 bytes; título interno `RechTrauma Copiloto v12`; 614 linhas.
- `rechtrauma_fluxo_explicado (2)(2).html` — recebido diretamente em 2026-08-09; 114.285 bytes; contém marcação `Visual trauma v24`; SHA-256 `ffbe5dd9ae2a510b4b6b3838e257a19a2ac55389ff3c885a9fe4ca880c412f19`. Tratar como variante candidata posterior, não como canônica automática.

### Outras variantes/material complementar localizado
- `rechtrauma_fluxo_explicado*.html`
- `rechtrauma_pcr_pospcr_modulos_definidos*.html`
- `rechtrauma_rosc_paco2_revisado*.html`
- `rechtrauma_fontes_macro*.html`
- `rechtrauma_macrodecisoes_fontes_limpas.html`
- `rechtrauma_antitrombotico_opcional.html`
- `rechtrauma_areas_criticas_fontes.html`
- `rechtrauma_visivel_corrigido.html`
- `rechtrauma_rastreabilidade.html`
- `rechtrauma_hotfix_clinico_visual.html`
- `rechtrauma_sem_versao*.html`
- `rechtrauma_acoes_explicadas.html`
- `PROTOCOLO_TRAUMA_ATLS_FINAL*.docx`

## Regra de migração
- Não apagar variantes antes da reconciliação.
- Subir candidatas principais em `candidates/`.
- Subir materiais derivados/históricos em `archive/` ou `references/` conforme inspeção.
- Não renomear qualquer variante para `index.html` antes do diff/auditoria.
- Gerar SHA-256 após transferência e registrar neste manifesto.

## Próxima operação de filesystem
Copiar os bytes originais materializados para o repo via ambiente Git/Codex, mantendo filename e hash; depois executar diff v12 ↔ v23 ↔ variante v24 e atualizar `PROJECT_STATE.md` no mesmo commit/PR.
