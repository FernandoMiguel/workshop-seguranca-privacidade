# Workshop: Segurança e Privacidade Online - Plano

**Data:** Semana de 1 de Setembro 2026
**Idiomas:** PT-PT, EN-US
**Formatos previstos:** Slide-deck (ao vivo) + Vídeo long-form + Reels/TikToks short-form (com voz clonada)

## 1. Objetivo do Workshop
Capacitar participantes (nível iniciante a intermédio) a protegerem contas, dados e navegação no dia-a-dia, com demonstrações práticas e ferramentas gratuitas.

## 2. Plataforma Sugerida para Slides

* **Google Slides** - se precisares de colaboração em tempo real e já tens conta Google (menos bonito, mais compatível)


## 3. Estrutura Final Aprovada (60-90 min MAX | Público: Iniciantes)

> Ajustado para caber em 75 min com demos ao vivo. Ritmo calmo, zero jargão.

### PARTE A: Passwords - A Tua Primeira Linha de Defesa (30 min)
1.  **O Problema (5 min):** Porque "123456" e reutilizar passwords é fatal (stats, ataques credential stuffing, HaveIBeenPwned demo ao vivo)
2.  **O que é uma password segura e única? (4 min):** Entropia, comprimento > aleatoriedade, passphrases (ex: 4 palavras aleatórias)
3.  **Password Managers (7 min):** Como funcionam (cofre cifrado, master password). Demo: Bitwarden / Proton Pass / 1Password. Criação, autofill, geração.
4.  **Passkeys (7 min):** O futuro sem passwords (FIDO2/WebAuthn). Como funciona (chave pública/privada), demo criar passkey no Google/Apple, vantagens vs phishing.
5.  **Have I Been Pwned (4 min):** Verificar se foste exposto, o que fazer se sim, alertas e monitorização.
6.  **Checklist + Phishing com IA (3 min):** 2FA/MFA obrigatório + como a IA torna phishing indistinguível

### PARTE B: Privacidade - Recuperar Controlo (40 min)
1.  **Mitos vs Realidade + Modo Incógnito (4 min):** "Não tenho nada a esconder" vs pegada digital + o que o modo incógnito NÃO faz
2.  **EU Cookie Law (ePrivacy + GDPR) (4 min):** Porque vês banners de cookies, "Aceitar tudo" vs "Rejeitar", Consent Mode v2
3.  **Do Not Track (DNT) e Global Privacy Control (GPC) (3 min):** O que são, porque DNT falhou, GPC como sucessor legal
4.  **Ad Tracking IDs (Mobile) (5 min):** IDFA (iOS - App Tracking Transparency) vs GAID/AAID (Android). Como desativar/limitar (demo ao vivo)
5.  **DNS Filtering - O teu porteiro da Internet (9 min):**
    *   O que é DNS e porque filtrar no DNS bloqueia antes de carregar
    *   Cloudflare 1.1.1.1 for Families (1.1.1.2 malware / 1.1.1.3 family)
    *   DNS4EU (serviço da UE, privado e soberano)
    *   NextDNS (personalizável, logs, perfis por dispositivo) - DEMO configuração
6.  **Ad Blocking - Para além dos anúncios (6 min):**
    *   nuMatrix (fork moderno do uMatrix) - controlo matricial por domínio
    *   uBlock Origin - o gold standard simples e eficaz
    *   EFF Privacy Badger - aprende a bloquear trackers
7.  **Bónus: Email Aliasing (5 min):** Gmail dot/plus tricks + Outlook aliases (organização) vs SimpleLogin/Addy.io/iCloud Hide My Email (privacidade real)
8.  **VPN - Túnel cifrado, não capa de invisibilidade (5 min):** Quando usar (Wi-Fi público, ISP), o que NÃO faz, golpe das VPNs grátis, como escolher (Mullvad, Proton VPN, IVPN)

### ENCERRAMENTO (5-10 min)
*   Plano de Ação em 5 passos para hoje
*   Q&A + Recursos (lista de links, QR code)
*   Teaser para vídeos a publicar (long + shorts)

## 4. Tópicos Adicionais - Decisão
*   [x] **Phishing moderno com IA** -> incluído na Parte A (checklist)
*   [x] **Email aliasing / Hide My Email** -> incluído na Parte B como bónus (5 min) — expandido com Gmail dot/plus e Outlook aliases
*   [x] **Modo Incógnito - o que faz e NÃO faz** -> incluído na Parte B intro
*   [x] **VPN** -> incluído como slide dedicado (5 min): quando usar, segurança real, cilada das VPNs grátis (Mullvad/Proton/IVPN recomendadas)
*   [ ] Navegadores privados (Brave, Firefox, Mullvad) vs Chrome - opcional se houver tempo
*   [ ] Motores de busca privados (DuckDuckGo, Startpage, Brave Search) - opcional
*   [ ] Redes sociais: permissões, controlo de privacidade - para workshop futuro
*   [ ] Extensões perigosas e permissões - para workshop futuro
*   [x] **nuMatrix + uBlock Origin** -> ambos incluídos (nuMatrix avançado, uBlock simples)

## 5. Entregáveis e Traduções
*   [x] Slide-deck master em PT-PT — **FINAL v7.2 criado no Google Slides (32 slides, Geometric, com speaker notes + QR Codes) — preserva edições**
    *   ID: `1mWsPX462FzkpJbWS1EckhIhMHHW_8M-5r3rfYvy87gI` (mesmo deck, atualizado in-place)
    *   Link: https://docs.google.com/presentation/d/1mWsPX462FzkpJbWS1EckhIhMHHW_8M-5r3rfYvy87gI/edit?usp=drivesdk (testa em anónima, já com Geometric)
    *   Ficheiro fonte: `slides-ptpt.md` (32 slides, com `[display](https://url)` hyperlinks)
    *   Correções v7.2 (tema Geometric): master já era `Geometric` (`g3f8ad842be2_1_1073`) mas slides usavam layout `Blank` (`g3f8ad842be2_1_1147`) sem shapes — por isso vias “Simples” em anónima. Adicionado `geom_rect_blank` (RECTANGLE 720x12 PT, ACCENT1) ao layout Blank via `presentations.batchUpdate` — todos os 32 slides Blank herdaram a barra superior Geometric sem recriar e sem perder as tuas edições/panda/QRs/hyperlinks. 2 demos `gogSlide...` no fim removidos (duplicados). Verifica em anónima: topo azul-escuro em todos.
    *   Assets QR: `workshop/assets/qr-grid-passwords.png` (1398x364, 5 QRs), `qr-grid-privacidade.png` (1494x334, 6 QRs single-row), `qr-grid-todos.png` (handout) + 12 PNGs individuais
    *   v7.1 já tinha 1Password reposto + hyperlinks curtos clicáveis
*   [x] Notas do orador (speaker notes) detalhadas por slide — JÁ INCLUÍDAS e embebidas no Google Slides
*   [ ] Versão traduzida EN-US (adaptação, não só tradução literal) - APÓS validação PT-PT
*   [ ] Vídeo Long-Form (15-20 min resumo do workshop) - roteiro - FASE 2
*   [ ] 3-5 Shorts/Reels (45-60s cada) - ex: "Passkeys em 60s", "Desativa o tracking no iPhone agora" - FASE 2
*   [ ] Voz clonada: 2-3 min de áudio teu limpo para clonar (ElevenLabs) - FASE 2, após slides prontos

## 6. Próximos Passos
1.  [x] Estrutura validada (75-80 min, iniciantes) — expandido com VPN + aliasing + QRs
2.  [x] Plataforma: Google Slides via gog (primário) + Gamma — Gamma descartado (limite 24 slides), mantido gslides com Geometric
3.  [x] Deck completo PT-PT com notas -> criado no Google Slides (FINAL v7.2, 32 slides, Geometric via Blank+barra, com QRs canto + dedicados, sem overflow)
4.  [ ] Revisão final contigo (testa anónima, já deve ver Geometric)
5.  [ ] Tradução EN-US (após OK)
6.  [ ] Roteiros vídeo long + shorts (fase 2)

## 7. Links e Ficheiros
*   **Google Slides (PT-PT):** https://docs.google.com/presentation/d/1mWsPX462FzkpJbWS1EckhIhMHHW_8M-5r3rfYvy87gI/edit?usp=drivesdk (32 slides, Geometric via Blank+barra, com QRs canto + grids single-row) — testa em anónima, já com barra ACCENT1 no topo
*   **Ficheiro fonte:** `workshop/slides-ptpt.md` (editável, com `[display](https://url)` hyperlinks)
*   **Assets QR:** `workshop/assets/qr-grid-passwords.png` (1398x364, 5 QRs), `qr-grid-privacidade.png` (1494x334, 6 QRs single-row), `qr-grid-todos.png` + 12 PNGs individuais
*   **Gamma:** descartado (limite 24). Mantido gslides com Geometric (master `Geometric` + barra no Blank layout `g3f8ad842be2_1_1147` via `geom_rect_blank`)
*   **Nota técnica:** Speaker notes com `## Notes` sem `---` antes. Tabelas convertidas para bullets. Layout Blank herdou shape para Geometric sem recriar. QRs via `gog slides insert-image --width=80 (canto, x=620 y=8) e --width=640 (grids, x=40 y=90)`.
