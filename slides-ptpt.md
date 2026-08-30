# Segurança e Privacidade Online na Prática

### Workshop prático de 75 min para iniciantes

**Passwords • Passkeys • Privacidade • DNS • Ad-blocking**

Fernando 🐼 — Setembro 2026

## Notes
Bem-vindo! 75 min sem jargão, tudo gratuito e fazes hoje. Interrompe e pergunta. No fim sais com checklist de 5 passos.

---

# O que vais levar daqui hoje

## 7 super-poderes em 80 min

- 🔐 Passwords à prova de hackers
- 🔑 Passkeys — adeus passwords
- 🕵️ Saber se já foste hackeado
- 📵 Travar tracking no telemóvel
- 🛡️ Bloquear ads/malware no DNS
- 🧹 Limpar tracking dos links (evitar doxing)
- 🔒 VPN — quando usar (e quando é cilada)

> Traz o telemóvel — vamos fazer ao vivo

## Notes
Agenda visual. Diz que é hands-on. Cria expectativa: no fim da Parte A já migras para gestor.

---

# PARTE A — PASSWORDS
## A tua primeira linha de defesa

> "Segurança não é um produto, é um hábito."

20% do esforço, 80% da proteção.

## Notes
Transição energética. Pergunta: "Quem reutiliza a mesma password?" (mãos no ar, sem vergonha). Normal — vamos resolver.

---

# O problema é grave. E é pessoal.

- **123456** e **password** ainda são #1 e #2 em PT (2024)
- **65%** reutiliza a mesma password
- 1 fuga → todas as contas em risco

**Credential stuffing:** vazam email+password num site → bots testam no Gmail, Instagram, banca automaticamente.

> 1 password = 1 chave para todas as portas

## Notes
Mostra HaveIBeenPwned aberto (sem pesquisar ainda). Explica fuga LinkedIn 2012 ainda usada hoje. 14+ mil milhões de contas no HIBP.

---

# O que é uma password *forte*?

### Comprimento > Complexidade

- **Má:** `P@ssw0rd!` — 8 chars, previsível
- **Boa:** `correct horse battery staple` — 4 palavras, 28 chars
- **Ótima:** `k9$Lp-27q-VALE-azul-trovão-482` — gerada

**Regra de ouro:** Longa (14-16+) • Única • Aleatória

> Se consegues decorar, é fraca. Deixa o gestor decorar.

## Notes
Entropia simples: cada char extra multiplica exponencialmente. Mostra gerador Bitwarden. Passphrase Diceware para master password.

---

# Gestores de Passwords
## O teu cofre cifrado

Cofre cifrado → só abre com a tua **Master Password**

Tu decoras **1** passphrase. Ele cria as outras 200.

**Recomendados:**
- **Bitwarden** — [bitwarden.com](https://bitwarden.com)
- **Proton Pass** — [proton.me/pass](https://proton.me/pass)
- **1Password** — [1password.com](https://1password.com)

> Zero-knowledge: ninguém vê as tuas passwords

## Notes
Analogia cofre vs chaves debaixo do tapete. Demo criar conta Bitwarden, gerar 20 chars, autofill. Aviso: guardar no browser sem master não é seguro.

---

# DEMO — Passa para gestor em 3 passos

1. **Instalar** Bitwarden (app + extensão) + master passphrase
2. **Importar** do Chrome/Firefox (2 cliques)
3. **Trocar** as 5 críticas: Email → Banco → Instagram → Google/Apple → Finanças

**Dica:** Ativa 2FA no próprio Bitwarden.

> 5 minutos hoje ao almoço e ficas com 80% feito

## Notes
Demo importação ao vivo ou screenshots. Prioriza 5 críticas. Mostra relatório "Reused/Exposed" no Bitwarden.

---

# Passkeys — O futuro sem passwords

Site guarda **cadeado** (pública). Telemóvel guarda **chave** (privada).

Desbloqueias com Face ID / PIN.

- ✅ À prova de phishing
- ✅ Nada para roubar
- ✅ Mais rápido

→ [passkeys.directory](https://passkeys.directory)

## Notes
Analogia cadeado/chave. Demo criar passkey em myaccount.google.com → Security → Passkeys. Fica no iCloud/Google Password Manager. Mantém gestor como fallback.

---

# Passkeys vs Passwords

**Passwords (antigo):**
- Criadas por ti — adivinháveis
- Reutilizáveis — vazam em todo o lado
- Phishing funciona
- Precisas de 2FA à parte

**Passkeys (novo):**
- Geradas pelo dispositivo — únicas por site
- Nada para roubar no servidor
- Phishing falha (domínio não bate)
- Já são 2 fatores (posse + biometria)

**Prática 2026:** passkey onde puderes, gestor para o resto.

## Notes
Contraste sem tabela. Reforça transição complementar. Mostra [passkeys.directory](https://passkeys.directory). Incentiva testar hoje no Google/Apple ID.

---

# Já foste exposto? Vamos ver agora.

## [haveibeenpwned.com](https://haveibeenpwned.com)

1. Escreve o teu email
2. 🟢 Verde = seguro (por agora)
3. 🔴 Vermelho = estiveste numa fuga → vê onde/o quê vazou

**Se vermelho:**
- Muda password nesse site + onde reutilizaste
- Ativa 2FA → clica **Notify me**

> Demo ao vivo — voluntário sem mostrar no ecrã

## Notes
DEMO CRÍTICA com email de teste. Troy Hunt, não faz spam. Mostra Pwned Passwords. QR no canto para seguirem.

---

# 2FA é obrigatório + Phishing com IA

**Ativa já em 5:** Email • Banco • Apple/Google • Instagram/TikTok • Finanças

**Ordem:** Passkey > App TOTP (Ente/Aegis/Proton/2FAS) > SMS

**Phishing 2026:** emails/SMS perfeitos, voz clonada, sites idênticos.

**Regra:** Nunca cliques em link de email/SMS para login. Vai tu ao site.

> 2FA é o cinto quando a password falha

## Notes
Mostra QR TOTP. SMS fraco (SIM swap). Compara phishing antigo vs IA lado a lado. Passkeys resolvem phishing.

---

# PARTE B — PRIVACIDADE
## Recuperar o controlo

> "Nada a esconder" ≠ "Nada a proteger"

Privacidade é **escolha**: o que partilhas, com quem, quando.

## Notes
Mito não é para criminosos. Vamos fechar janelas escancaradas por defeito.

---

# Mito: "O Modo Incógnito protege-me"

**O que FAZ:**
- Apaga histórico/cookies locais ao fechar
- Bom para emprestar portátil

**O que NÃO FAZ:**
- Não esconde IP (ISP/patrão vê)
- Não bloqueia Google/Facebook tracking
- Não é VPN nem anonimato

> Apagas pegadas em casa, mas as câmaras da rua filmam.

## Notes
Mostra aviso do Chrome incógnito. Pergunta quem usa para privacidade. Humor para desmistificar.

---

# Porque vês banners de cookies?

## EU Cookie Law (GDPR + ePrivacy)

- Na UE, tracking só com **consentimento**
- **Aceitar tudo** = luz verde a 100+ trackers
- **Rejeitar / Necessários** = só o essencial

**Dica:** Sê chato, clica sempre Rejeitar. Usa **Consent-O-Matic**.

## Notes
Mostra banner real → Gerir → 100 parceiros = choque. Essenciais vs marketing. Tens direito a rejeitar sem perder acesso.

---

# Do Not Track e Global Privacy Control

- **DNT (2009):** "por favor não me sigas" → **ninguém respeitou**
- **GPC (2020+):** sucessor com **força legal** (CA + UE/GDPR)

Ativa GPC: Brave já vem ligado • Firefox → Privacidade → GPC

> DNT morreu. GPC tem dentes.

→ [globalprivacycontrol.org](https://globalprivacycontrol.org)

## Notes
DNT opcional falhou. GPC com EFF, enforceable. Demo Brave.

---

# O teu telemóvel está a seguir-te?

## Ad Tracking IDs — desliga em 30s

- **iPhone (IDFA):** Definições → Privacidade → Rastreio → desativa "Permitir que apps peçam"
- **Android (GAID):** Definições → Privacidade → Anúncios → Elimina ID + desativa personalização

> Faz agora no teu telemóvel

## Notes
DEMO interativa. Screenshots lado a lado. Não remove anúncios, mas impede perfil entre apps. ATT reduziu 60%+ tracking.

---

# O que é DNS?

Escreves `google.com` → DNS traduz para `142.250.180.14`

Se controlares o DNS, **bloqueias malware/ads antes de carregarem**.

> **Porteiro do prédio.** Para toda a casa, configura no **router** — todos os dispositivos protegidos sem instalar nada em cada um.

## Notes
Analogia lista telefónica. Diagrama Dispositivo → DNS → Internet. Leve, rápido, funciona em smart TV. Não é VPN, é complementar.

---

# DNS Filtering — 3 porteiros

**1. Cloudflare Families** — [one.one.one.one/family](https://one.one.one.one/family)
- `1.1.1.2` malware • `1.1.1.3` malware+adulto

**2. DNS4EU** — [joindns4.eu](https://www.joindns4.eu)
- UE, GDPR, sem logs, `86.54.11.13`

**3. NextDNS** — [my.nextdns.io](https://my.nextdns.io)
- Personalizável, 300k/mês grátis, por dispositivo

## Notes
Compara em 3 bullets curtos. Mostra mudar DNS no iPhone/Android e no router (toda a casa). Recomenda NextDNS para controlo total.

---

# DEMO — NextDNS em 2 minutos

1. Vai a **[my.nextdns.io](https://my.nextdns.io)** → conta grátis
2. Listas: NextDNS Ads & Trackers + StevenBlack
3. Liga **Native Tracking Protection**
4. Instala perfil (iOS) / app (Android) / router

Vês em tempo real: bloqueios, % trackers, por dispositivo

## Notes
Demo dashboard com gráfico. Antes/depois num site com ads. Grátis chega para 2-3 pessoas. Pi-hole para nerds.

---

# Ad-blocking — Não é estética, é privacidade

Anúncios = **trackers** entre sites.

Bloquear = mais rápido, mais bateria, menos malware.

> A seguir: as 3 ferramentas que importam

## Notes
Exemplo site notícias 3s vs 10s, 50 trackers vs 2. Transição.

---

# uBlock Origin + Privacy Badger

**uBlock Origin — para todos** — [ublockorigin.com](https://ublockorigin.com)
- Instala e esquece. Leve, 90% bloqueado.

**Privacy Badger (EFF)** — [privacybadger.org](https://privacybadger.org)
- Aprende sozinho, bloqueia quem te segue em 3+ sites.

> Começa com uBlock. Chega para 90% das pessoas.

## Notes
Mostra instalação Chrome/Firefox. Não uses 5 ad-blockers ao mesmo tempo. Para iniciantes, isto basta.

---

# nuMatrix — Para curiosos

**Fork do uMatrix** — [codeberg.org/arek/nuMatrix](https://codeberg.org/arek/nuMatrix)

- Matriz por domínio: JS, cookies, XHR, media
- Controlo cirúrgico do que cada site carrega
- Curva maior, pode partir sites no início

> Power users: experimenta depois de dominares o uBlock

## Notes
Screenshot matriz. Para quem quer perceber tudo. Aviso que parte sites até aprender. Separa do slide anterior para não sobrecarregar iniciantes.

---

# Email Aliasing — Esconde o real

### Parte 1: Truques (organização, não privacidade)

- **Gmail ignora pontos:** `joao.silva@gmail.com` = `joaosilva@gmail.com`
- **Gmail `+`:** `joao+loja@gmail.com` → filtra, mas fácil de remover
- **Outlook:** `+` + **aliases reais** ([outlook.live.com](https://outlook.live.com) → até 10)

> Útil para organizar, **não esconde** — tira-se o ponto/+ num segundo

## Notes
Demo `joao+teste` cria filtro. Outlook alias real. Explica que é trivial limpar, não é privacidade.

---

# Email Aliasing — Privacidade real

### Parte 2: Aliases aleatórios

Em vez de `joao@gmail.com` → `joao.loja.8f3k@aleatorio.simplelogin.com`

- Spam? **Desligas o alias** (1 clique)
- Fuga? Sabes **quem vendeu** os dados
- Respondes sem revelar o real

**Usa:** [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io) • iCloud Hide My Email • Firefox Relay

> Gmail/Outlook para organizar. SimpleLogin/Addy para privacidade.

## Notes
Demo criar alias no SimpleLogin/Proton Pass. Alias por serviço = higiene digital. Liga a gestor = identidade descartável por site.

---

# VPN — Túnel cifrado, não capa de invisibilidade

**O que FAZ:**
- Cifra até ao servidor VPN — esconde IP do Wi-Fi/ISP/patrão
- Útil em Wi-Fi público, censura, bloqueio geográfico

**O que NÃO FAZ:**
- Não bloqueia trackers/cookies
- Não és anónimo logado no Google
- Não protege de malware

> Para o dia-a-dia, **NextDNS + uBlock** já dão 80%

## Notes
Analogia camião blindado até correio central, depois vai aberta. Não é privacidade total, é transporte. Mostra quando usar.

---

# VPN — O golpe das grátis e como escolher

**⚠️ Grátis = tu és o produto**
SuperVPN, TurboVPN, GeckoVPN (100M+) — venderam logs, vazaram dados.

**Como escolher (auditada, WireGuard, RAM-only):**
- **Mullvad** — [mullvad.net](https://mullvad.net) (5€/mês, sem email)
- **Proton VPN** — [protonvpn.com](https://protonvpn.com) (grátis honesto)
- **IVPN** — [ivpn.net](https://www.ivpn.net)

> Se é grátis e não é Proton, desconfia.

## Notes
Alerta forte: pior que sem VPN. Muitas grátis são da mesma empresa chinesa. Se só podes grátis, Proton Free é a única confiável.

---

# Links sujos — limpa o tracking antes de partilhar

- Links vêm sujos: `?utm_source=...&fbclid=...&igsh=...` que identificam quem clicou/partilhou
- Instagram `igsh` e Facebook `fbclid` fazem **doxing** — quem recebe vê de quem veio
- **Regra:** partilha só `https://site.com/pagina` — apaga tudo depois de `?`

**Ferramentas:**
- **Android:** [altsea.app](https://altsea.app) — cola o link → copia limpo
- **Desktop:** [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper) — remove auto ao copiar

> Partilhar link sujo = partilhar o teu rasto

## Notes
DEMO ao vivo: copia link Instagram com `?igsh=` → cola em altsea.app → mostra link limpo. Explica doxing: `igsh` devolve ao perfil de quem partilhou. UTM não é essencial — site abre igual sem `?utm_...`. Mostra Tracking Token Stripper a limpar no desktop ao copiar.

---

# O teu Plano de Ação — HOJE (5 passos)

1. ✅ Gestor (Bitwarden) + importa + troca email/banca
2. ✅ Primeira passkey (Google/Apple)
3. ✅ [haveibeenpwned.com](https://haveibeenpwned.com) + Notify me
4. ✅ Telemóvel: desativa tracking + DNS NextDNS/1.1.1.3
5. ✅ Browser: [ublockorigin.com](https://ublockorigin.com)

> Foto neste slide. 30 min hoje à noite.

## Notes
Slide mais importante, deixa 2 min. Foto. 1+2+3 = 80% do ganho.

---

# Recursos — Guarda este slide (1/2)

**Contas & Passwords**
- [haveibeenpwned.com](https://haveibeenpwned.com)
- [bitwarden.com](https://bitwarden.com) • [proton.me/pass](https://proton.me/pass)
- [passkeys.directory](https://passkeys.directory)
- [ente.io/auth](https://ente.io/auth) • [getaegis.app](https://getaegis.app)

**Privacidade**
- [one.one.one.one/family](https://one.one.one.one/family)
- [joindns4.eu](https://www.joindns4.eu)
- [my.nextdns.io](https://my.nextdns.io)
- [ublockorigin.com](https://ublockorigin.com)

## Notes
Primeira metade dos links. Diz que PDF tem tudo clicável. Segunda metade no próximo slide.

---

# Recursos — Guarda este slide (2/2)

**Email & VPN**
- [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io)
- [mullvad.net](https://mullvad.net) • [protonvpn.com](https://protonvpn.com)
- [privacybadger.org](https://privacybadger.org) • [globalprivacycontrol.org](https://globalprivacycontrol.org)

**Testa & Truques**
- [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- [altsea.app](https://altsea.app)
- [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper)
- support.google.com/mail/answer/5238509

> PDF com todos os links será partilhado

## Notes
Segunda metade. Linktree/Notion com tudo. Menciona vídeos fase 2.

---

# QR Codes — Passwords & Contas

## Notes
Dá 30s para fotografar. Kit arranque passwords. HaveIBeenPwned urgente.

---

# QR Codes — Privacidade & Proteção

## Notes
Segundo lote. NextDNS mais impacto. uBlock no portátil. SimpleLogin para alias.

---

# Perguntas?
## Obrigado!

### Segurança é maratona, não sprint.

Começa com 1 passo hoje.

## Notes
Encerra, Q&A. Se tempo, VPN vs DNS ou Brave vs Firefox.
