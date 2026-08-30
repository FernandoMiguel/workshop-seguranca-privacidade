# Segurança e Privacidade Online na Prática

### Workshop prático de 75 min para iniciantes

**Senhas • Passkeys • Privacidade • DNS • Bloqueio de Anúncios**

Fernando 🐼 — Setembro de 2026

## Notes
Boas-vindas! 75 min sem jargão, tudo gratuito e você faz hoje. Pode interromper e perguntar à vontade. No final você sai com um checklist de 5 passos.

---

# O que você vai levar daqui hoje

## 7 superpoderes em 80 min

- 🔐 Senhas à prova de hackers
- 🔑 Passkeys — adeus senhas
- 🕵️ Saber se você já foi hackeado
- 📵 Travar rastreamento no celular
- 🛡️ Bloquear anúncios/malware no DNS
- 🧹 Limpar rastreamento dos links (evitar doxing)
- 🔒 VPN — quando usar (e quando é cilada)

> Traga o celular — vamos fazer ao vivo

## Notes
Agenda visual. Diga que é hands-on. Crie expectativa: no final da Parte A você já migra para um gerenciador.

---

# PARTE A — SENHAS
## Sua primeira linha de defesa

> "Segurança não é um produto, é um hábito."

20% do esforço, 80% da proteção.

## Notes
Transição com energia. Pergunte: "Quem reutiliza a mesma senha?" (mãos para cima, sem vergonha). É normal — vamos resolver.

---

# O problema é grave. E é pessoal.

- **123456** e **password** ainda são #1 e #2 no Brasil (2024)
- **65%** reutiliza a mesma senha
- 1 vazamento → todas as contas em risco

**Credential stuffing:** vazam e-mail+senha num site → bots testam automaticamente no Gmail, Instagram, banco.

> 1 senha = 1 chave para todas as portas

## Notes
Mostre o HaveIBeenPwned aberto (sem pesquisar ainda). Explique que o vazamento do LinkedIn de 2012 ainda é usado hoje. São mais de 14 bilhões de contas no HIBP.

---

# O que é uma senha *forte*?

### Tamanho > Complexidade

- **Ruim:** `P@ssw0rd!` — 8 caracteres, previsível
- **Boa:** `correct horse battery staple` — 4 palavras, 28 caracteres
- **Ótima:** `k9$Lp-27q-VALE-azul-trovão-482` — gerada

**Regra de ouro:** Longa (14-16+) • Única • Aleatória

> Se você consegue decorar, é fraca. Deixe o gerenciador decorar.

## Notes
Entropia simples: cada caractere extra multiplica exponencialmente. Mostre o gerador do Bitwarden. Frase-senha Diceware para a senha mestra.

---

# Gerenciadores de Senhas
## Seu cofre criptografado

Cofre criptografado → só abre com sua **senha mestra**

Você decora **1** frase-senha. Ele cria as outras 200.

**Recomendados:**
- **Bitwarden** — [bitwarden.com](https://bitwarden.com)
- **Proton Pass** — [proton.me/pass](https://proton.me/pass)
- **1Password** — [1password.com](https://1password.com)

> Zero-knowledge: ninguém vê suas senhas

## Notes
Analogia do cofre vs. chaves embaixo do tapete. Demonstre criando conta no Bitwarden, gerando 20 caracteres, preenchimento automático. Aviso: salvar no navegador sem senha mestra não é seguro.

---

# DEMO — Migre para o gerenciador em 3 passos

1. **Instalar** Bitwarden (app + extensão) + frase da senha mestra
2. **Importar** do Chrome/Firefox (2 cliques)
3. **Trocar** as 5 críticas: E-mail → Banco → Instagram → Google/Apple → Finanças

**Dica:** Ative o 2FA no próprio Bitwarden.

> 5 minutos hoje na hora do almoço e você já garante 80%

## Notes
Demonstração de importação ao vivo ou com prints. Priorize as 5 críticas. Mostre o relatório "Senhas Reutilizadas/Expostas" no Bitwarden.

---

# Passkeys — O futuro sem senhas

Site guarda **cadeado** (chave pública). Celular guarda **chave** (privada).

Você desbloqueia com Face ID / PIN.

- ✅ À prova de phishing
- ✅ Nada para roubar
- ✅ Mais rápido

→ [passkeys.directory](https://passkeys.directory)

## Notes
Analogia cadeado/chave. Demonstre criando uma passkey em myaccount.google.com → Segurança → Chaves de acesso (Passkeys). Fica no iCloud/Google Gerenciador de Senhas. Mantenha o gerenciador como plano B.

---

# Passkeys vs Senhas

**Senhas (antigo):**
- Criadas por você — adivinháveis
- Reutilizáveis — vazam em todo lugar
- Phishing funciona
- Precisa de 2FA separado

**Passkeys (novo):**
- Geradas pelo dispositivo — únicas por site
- Nada para roubar no servidor
- Phishing falha (domínio não confere)
- Já são 2 fatores (posse + biometria)

**Na prática em 2026:** use passkey onde puder, gerenciador para o resto.

## Notes
Contraste sem tabela. Reforce a transição complementar. Mostre [passkeys.directory](https://passkeys.directory). Incentive a testar hoje na conta do Google/Apple ID.

---

# Você já foi exposto? Vamos ver agora.

## [haveibeenpwned.com](https://haveibeenpwned.com)

1. Digite seu e-mail
2. 🟢 Verde = seguro (por enquanto)
3. 🔴 Vermelho = você esteve em um vazamento → veja onde/o que vazou

**Se der vermelho:**
- Troque a senha nesse site + onde reutilizou
- Ative o 2FA → clique em **Notify me**

> Demo ao vivo — voluntário sem mostrar na tela

## Notes
DEMO CRÍTICA com e-mail de teste. Troy Hunt, não faz spam. Mostre o Pwned Passwords. QR code no canto para acompanharem.

---

# 2FA é obrigatório + Phishing com IA

**Ative já em 5:** E-mail • Banco • Apple/Google • Instagram/TikTok • Finanças

**Ordem:** Passkey > App TOTP (Ente/Aegis/Proton/2FAS) > SMS

**Phishing em 2026:** e-mails/SMS perfeitos, voz clonada, sites idênticos.

**Regra:** Nunca clique em link de e-mail/SMS para fazer login. Acesse o site você mesmo.

> 2FA é o cinto de segurança quando a senha falha

## Notes
Mostre QR code do TOTP. SMS é fraco (SIM swap). Compare phishing antigo vs. com IA lado a lado. Passkeys resolvem o phishing.

---

# PARTE B — PRIVACIDADE
## Retomar o controle

> "Nada a esconder" ≠ "Nada a proteger"

Privacidade é **escolha**: o que você compartilha, com quem e quando.

## Notes
Mito de que privacidade é só para criminosos. Vamos fechar janelas que vêm escancaradas por padrão.

---

# Mito: "O Modo Anônimo me protege"

**O que FAZ:**
- Apaga histórico/cookies locais ao fechar
- Bom para emprestar o notebook

**O que NÃO FAZ:**
- Não esconde o IP (provedor/chefe vê)
- Não bloqueia rastreamento do Google/Facebook
- Não é VPN nem anonimato

> Você apaga as pegadas em casa, mas as câmeras da rua continuam filmando.

## Notes
Mostre o aviso do modo anônimo do Chrome. Pergunte quem usa para ter privacidade. Use humor para desmistificar.

---

# Por que você vê banners de cookies?

## Lei de Cookies da UE (GDPR + ePrivacy)

- Na UE, rastreamento só com **consentimento**
- **Aceitar tudo** = sinal verde para 100+ rastreadores
- **Rejeitar / Necessários** = só o essencial

**Dica:** Seja chato, clique sempre em Rejeitar. Use o **Consent-O-Matic**.

## Notes
Mostre um banner real → Gerenciar → 100 parceiros = choque. Essenciais vs. marketing. Você tem direito de rejeitar sem perder acesso.

---

# Do Not Track e Global Privacy Control

- **DNT (2009):** "por favor, não me rastreie" → **ninguém respeitou**
- **GPC (2020+):** sucessor com **força legal** (CA + UE/GDPR)

Ative o GPC: Brave já vem ligado • Firefox → Privacidade → GPC

> DNT morreu. GPC tem dentes.

→ [globalprivacycontrol.org](https://globalprivacycontrol.org)

## Notes
DNT opcional falhou. GPC com apoio da EFF, com exigibilidade legal. Demonstre no Brave.

---

# Seu celular está te rastreando?

## IDs de rastreamento de anúncios — desligue em 30s

- **iPhone (IDFA):** Ajustes → Privacidade → Rastreamento → desative "Permitir que Apps Solicitem Rastreamento"
- **Android (GAID):** Configurações → Privacidade → Anúncios → Exclua o ID + desative a personalização

> Faça agora no seu celular

## Notes
DEMO interativa. Prints lado a lado. Não remove anúncios, mas impede a criação de perfil entre apps. ATT reduziu 60%+ do rastreamento.

---

# O que é DNS?

Você digita `google.com` → DNS traduz para `142.250.180.14`

Se você controla o DNS, **bloqueia malware/anúncios antes de carregarem**.

> **Porteiro do prédio.** Para a casa toda, configure no **roteador** — todos os dispositivos protegidos sem instalar nada em cada um.

## Notes
Analogia da lista telefônica. Diagrama Dispositivo → DNS → Internet. Leve, rápido, funciona até em smart TV. Não é VPN, é complementar.

---

# Filtragem DNS — 3 porteiros

**1. Cloudflare Families** — [one.one.one.one/family](https://one.one.one.one/family)
- `1.1.1.2` malware • `1.1.1.3` malware+adulto

**2. DNS4EU** — [joindns4.eu](https://www.joindns4.eu)
- UE, GDPR, sem logs, `86.54.11.13`

**3. NextDNS** — [my.nextdns.io](https://my.nextdns.io)
- Personalizável, 300k/mês grátis, por dispositivo

## Notes
Compare em 3 bullets curtos. Mostre como mudar o DNS no iPhone/Android e no roteador (casa toda). Recomende NextDNS para controle total.

---

# DEMO — NextDNS em 2 minutos

1. Acesse **[my.nextdns.io](https://my.nextdns.io)** → conta grátis
2. Listas: NextDNS Ads & Trackers + StevenBlack
3. Ative **Native Tracking Protection**
4. Instale perfil (iOS) / app (Android) / roteador

Veja em tempo real: bloqueios, % de rastreadores, por dispositivo

## Notes
Demonstre o dashboard com gráfico. Antes/depois num site com anúncios. O plano grátis dá para 2-3 pessoas. Pi-hole para quem curte mais técnica.

---

# Bloqueio de anúncios — Não é estética, é privacidade

Anúncios = **rastreadores** entre sites.

Bloquear = mais rápido, mais bateria, menos malware.

> A seguir: as 3 ferramentas que importam

## Notes
Exemplo site de notícias 3s vs 10s, 50 rastreadores vs 2. Transição.

---

# uBlock Origin + Privacy Badger

**uBlock Origin — para todo mundo** — [ublockorigin.com](https://ublockorigin.com)
- Instale e esqueça. Leve, 90% bloqueado.

**Privacy Badger (EFF)** — [privacybadger.org](https://privacybadger.org)
- Aprende sozinho, bloqueia quem te segue em 3+ sites.

> Comece com o uBlock. É suficiente para 90% das pessoas.

## Notes
Mostre a instalação no Chrome/Firefox. Não use 5 bloqueadores ao mesmo tempo. Para iniciantes, isso já basta.

---

# nuMatrix — Para curiosos

**Fork do uMatrix** — [codeberg.org/arek/nuMatrix](https://codeberg.org/arek/nuMatrix)

- Matriz por domínio: JS, cookies, XHR, mídia
- Controle cirúrgico do que cada site carrega
- Curva de aprendizado maior, pode quebrar sites no começo

> Para usuários avançados: experimente depois de dominar o uBlock

## Notes
Print da matriz. Para quem quer entender tudo. Avise que quebra sites até aprender. Separado do slide anterior para não sobrecarregar iniciantes.

---

# E-mail com máscara — Esconda o real

### Parte 1: Truques (organização, não privacidade)

- **Gmail ignora pontos:** `joao.silva@gmail.com` = `joaosilva@gmail.com`
- **Gmail `+`:** `joao+loja@gmail.com` → filtra, mas fácil de remover
- **Outlook:** `+` + **aliases reais** ([outlook.live.com](https://outlook.live.com) → até 10)

> Útil para organizar, **não esconde** — dá para tirar o ponto/+ em um segundo

## Notes
Demonstre `joao+teste` criando filtro. Alias real no Outlook. Explique que é trivial limpar, não é privacidade.

---

# E-mail com máscara — Privacidade real

### Parte 2: Aliases aleatórios

Em vez de `joao@gmail.com` → `joao.loja.8f3k@aleatorio.simplelogin.com`

- Spam? **Desative o alias** (1 clique)
- Vazamento? Você sabe **quem vendeu** seus dados
- Pode responder sem revelar o real

**Use:** [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io) • iCloud Hide My Email • Firefox Relay

> Gmail/Outlook para organizar. SimpleLogin/Addy para privacidade.

## Notes
Demonstre criando um alias no SimpleLogin/Proton Pass. Um alias por serviço = higiene digital. Combine com o gerenciador = identidade descartável por site.

---

# VPN — Túnel criptografado, não capa de invisibilidade

**O que FAZ:**
- Criptografa até o servidor VPN — esconde IP do Wi-Fi/provedor/chefe
- Útil em Wi-Fi público, censura, bloqueio geográfico

**O que NÃO FAZ:**
- Não bloqueia rastreadores/cookies
- Você não fica anônimo logado no Google
- Não protege contra malware

> Para o dia a dia, **NextDNS + uBlock** já entregam 80%

## Notes
Analogia do caminhão blindado até o centro de distribuição, depois segue aberto. Não é privacidade total, é transporte. Mostre quando usar.

---

# VPN — O golpe das grátis e como escolher

**⚠️ Grátis = você é o produto**
SuperVPN, TurboVPN, GeckoVPN (100M+) — venderam logs, vazaram dados.

**Como escolher (auditada, WireGuard, só RAM):**
- **Mullvad** — [mullvad.net](https://mullvad.net) (5€/mês, sem e-mail)
- **Proton VPN** — [protonvpn.com](https://protonvpn.com) (grátis honesto)
- **IVPN** — [ivpn.net](https://www.ivpn.net)

> Se é grátis e não é Proton, desconfie.

## Notes
Alerta forte: pior que ficar sem VPN. Muitas grátis são da mesma empresa chinesa. Se só puder usar grátis, Proton Free é a única confiável.

---

# Links sujos — limpe o rastreamento antes de compartilhar

- Links vêm sujos: `?utm_source=...&fbclid=...&igsh=...` que identificam quem clicou/compartilhou
- Instagram `igsh` e Facebook `fbclid` fazem **doxing** — quem recebe vê de quem veio
- **Regra:** compartilhe só `https://site.com/pagina` — apague tudo depois de `?`

**Ferramentas:**
- **Android:** [altsea.app](https://altsea.app) — cole o link → copie limpo
- **Desktop:** [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper) — remove automaticamente ao copiar

> Compartilhar link sujo = compartilhar seu rastro

## Notes
DEMO ao vivo: copie link do Instagram com `?igsh=` → cole no altsea.app → mostre o link limpo. Explique doxing: `igsh` permite voltar ao perfil de quem compartilhou. UTM não é essencial — o site abre igual sem `?utm_...`. Mostre o Tracking Token Stripper limpando no desktop ao copiar.

---

# Seu Plano de Ação — HOJE (5 passos)

1. ✅ Gerenciador (Bitwarden) + importe + troque e-mail/banco
2. ✅ Primeira passkey (Google/Apple)
3. ✅ [haveibeenpwned.com](https://haveibeenpwned.com) + Notify me
4. ✅ Celular: desative rastreamento + DNS NextDNS/1.1.1.3
5. ✅ Navegador: [ublockorigin.com](https://ublockorigin.com)

> Tire foto deste slide. 30 min hoje à noite e você resolve.

## Notes
Slide mais importante, deixe 2 min. Foto. 1+2+3 = 80% do ganho.

---

# Recursos — Guarde este slide (1/2)

**Contas & Senhas**
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
Primeira metade dos links. Diga que o PDF tem tudo clicável. Segunda metade no próximo slide.

---

# Recursos — Guarde este slide (2/2)

**E-mail & VPN**
- [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io)
- [mullvad.net](https://mullvad.net) • [protonvpn.com](https://protonvpn.com)
- [privacybadger.org](https://privacybadger.org) • [globalprivacycontrol.org](https://globalprivacycontrol.org)

**Teste & Truques**
- [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- [altsea.app](https://altsea.app)
- [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper)
- support.google.com/mail/answer/5238509

> PDF com todos os links será compartilhado

## Notes
Segunda metade. Linktree/Notion com tudo. Mencione vídeos da fase 2.

---

# QR Codes — Senhas & Contas

## Notes
Dê 30s para fotografarem. Kit de arranque de senhas. HaveIBeenPwned é urgente.

---

# QR Codes — Privacidade & Proteção

## Notes
Segundo lote. NextDNS com mais impacto. uBlock no notebook. SimpleLogin para aliases.

---

# Perguntas?
## Obrigado!

### Segurança é maratona, não sprint.

Comece com 1 passo hoje.

## Notes
Encerra, Q&A. Se der tempo, VPN vs DNS ou Brave vs Firefox.
