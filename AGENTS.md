# AGENTS — workshop-seguranca-privacidade

## Project
Workshop 75 min para iniciantes: Segurança e Privacidade Online (Passwords, Passkeys, DNS, VPN, Ad-blocking). Não é projeto de código — sem build/test/lint. Artefacto é o deck de slides + plano.

- Repo: `FernandoMiguel/workshop-seguranca-privacidade` (public, branch `main`)
- Idioma principal: PT-PT (`slides-ptpt.md`); PT-BR e EN-US são adaptações futuras
- Licença: educativo, reutilização com atribuição

## Structure
- `slides-ptpt.md` — **fonte do deck** (33 slides, com `## Notes` e hyperlinks `[display](url)`)
- `plan.md` — plano completo + log de versões (fonte de verdade para estrutura/histórico)
- `assets/` — logos + QR grids (`qr-grid-passwords.png` 1398x364, `qr-grid-privacidade.png` 1494x334, `qr-grid-todos.png` + 12 PNGs individuais + `qr_grid1/2_v7.png` legados)
- `README.md` — sumário público com link do Google Slides
- Google Slides FINAL v7.3 (33 slides): `1mWsPX462FzkpJbWS1EckhIhMHHW_8M-5r3rfYvy87gI` — https://docs.google.com/presentation/d/1mWsPX462FzkpJbWS1EckhIhMHHW_8M-5r3rfYvy87gI/edit?usp=drivesdk

## Editing Slides — Source of Truth is `slides-ptpt.md`
Formato exigido pelo `gog slides create-from-markdown`:
- `#` = título do slide, `---` = separador, `## Notes` (inglês, sem `---` antes) = speaker notes
- Links: `[texto curto](https://url)` — mantém display curto, URL completa no href
- **Nunca usar tabelas Markdown** (`|---|---|`) — quebra layout; usar bullets
- Manter slides curtos: <510 chars ideal, <300 para evitar overflow (validado em v6/v7)
- Demo slides com QR de canto vs grids dedicados são intencionais — não remover

## Google Slides via `gog` — Gotchas (hard-won)
- **Criar/atualizar:** `gog slides create-from-markdown --content-file slides-ptpt.md "Título"` cria deck novo. **Não recriar o deck FINAL à toa** — perde edições manuais (panda, QRs posicionados, hyperlinks aplicados via API, barra Geometric).
- **Atualizações cirúrgicas (preferir):**
  - Texto: `gog slides insert-text <presentationId> <objectId> "texto" --insertion-index N`
  - Hyperlinks: `gog slides link --range start:end <presentationId> <objectId> --url https://...` (requer `locate` para achar `objectId` + range UTF-16)
  - Imagens: `gog slides insert-image --width 80 --x 620 --y 8 <id> <slideId> assets/qr-...png` (canto) ou `--width 640 --x 40 --y 90` (grid centralizado)
  - Notas: `gog slides update-notes <id> <slideId>`
- **Tema Geometric:** master é `Geometric` (`g3f8ad842be2_1_1073`) mas layout `Blank` (`g3f8ad842be2_1_1147`) vem sem shapes — por isso deck parecia "Simples" em anónima. Fix v7.2 adicionou `geom_rect_blank` (RECTANGLE 720x12 PT, ACCENT1) ao layout Blank via `presentations.batchUpdate`. Se recriar deck, reaplicar ou usar layouts `TITLE`/`TITLE_AND_BODY` que já têm barra.

## Assets & QR
- Grids foram gerados single-row compactos para caber em `--width 640`; não voltar a grelhas 2-row.
- Ao reinserir QRs, usar coordenadas exatas acima; y=90 evita sobreposição com título.
- `assets/qr-grid-todos.png` é handout, não vai para slides.

## Git
- Commit msgs em PT-PT, escopo `feat:` para deck; incluir ID do Slides e versão no body
- Não commitar `.DS_Store` (já em `.gitignore`)
