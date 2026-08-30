# Practical Online Security & Privacy

### Hands-on 75-min workshop for beginners

**Passwords • Passkeys • Privacy • DNS • Ad-blocking**

Fernando 🐼 — September 2026

## Notes
Welcome! 75 min with no jargon, everything free and you can do it today. Jump in with questions anytime. You'll leave with a 5-step checklist.

---

# What you'll take home today

## 7 superpowers in 75 min

- 🔐 Hacker-proof passwords
- 🔑 Passkeys — goodbye passwords
- 🕵️ Check if you've been hacked
- 📵 Stop tracking on your phone
- 🛡️ Block ads/malware at the DNS level
- 🧹 Clean tracking from links (avoid doxing)
- 🔒 VPN — when to use it (and when it's a trap)

> Bring your phone — we'll do it live

## Notes
Visual agenda. Say it's hands-on. Set expectations: by the end of Part A you'll have migrated to a password manager.

---

# PART A — PASSWORDS
## Your first line of defense

> "Security isn't a product, it's a habit."

20% of the effort, 80% of the protection.

## Notes
High-energy transition. Ask: "Who reuses the same password?" (hands up, no shame). Totally normal — let's fix it.

---

# The problem is serious. And it's personal.

- **123456** and **password** are still #1 and #2 worldwide (2024)
- **65%** reuse the same password
- 1 breach → every account at risk

**Credential stuffing:** email+password leaks on one site → bots automatically try them on Gmail, Instagram, banking.

> 1 password = 1 key for every door

## Notes
Show HaveIBeenPwned open (don't search yet). Explain the 2012 LinkedIn breach is still used today. 14+ billion accounts in HIBP.

---

# What makes a *strong* password?

### Length > Complexity

- **Bad:** `P@ssw0rd!` — 8 chars, predictable
- **Good:** `correct horse battery staple` — 4 words, 28 chars
- **Great:** `k9$Lp-27q-VALE-blue-thunder-482` — generated

**Golden rule:** Long (14-16+) • Unique • Random

> If you can remember it, it's weak. Let the manager remember it.

## Notes
Simple entropy: each extra character multiplies exponentially. Show Bitwarden generator. Diceware passphrase for the master password.

---

# Password Managers
## Your encrypted vault

Encrypted vault → only opens with your **Master Password**

You memorize **1** passphrase. It creates the other 200.

**Recommended:**
- **Bitwarden** — [bitwarden.com](https://bitwarden.com)
- **Proton Pass** — [proton.me/pass](https://proton.me/pass)
- **1Password** — [1password.com](https://1password.com)

> Zero-knowledge: nobody can see your passwords

## Notes
Analogy: vault vs keys under the doormat. Demo creating a Bitwarden account, generating 20 chars, autofill. Warning: saving in the browser without a master password isn't secure.

---

# DEMO — Switch to a manager in 3 steps

1. **Install** Bitwarden (app + extension) + master passphrase
2. **Import** from Chrome/Firefox (2 clicks)
3. **Change** the top 5: Email → Bank → Instagram → Google/Apple → Finance

**Tip:** Enable 2FA on Bitwarden itself.

> 5 minutes over lunch and you're 80% done

## Notes
Live import demo or screenshots. Prioritize the top 5. Show the "Reused/Exposed" report in Bitwarden.

---

# Passkeys — The passwordless future

Site keeps the **lock** (public key). Your phone keeps the **key** (private key).

Unlock with Face ID / PIN.

- ✅ Phishing-proof
- ✅ Nothing to steal
- ✅ Faster

→ [passkeys.directory](https://passkeys.directory)

## Notes
Lock/key analogy. Demo creating a passkey at myaccount.google.com → Security → Passkeys. Stored in iCloud/Google Password Manager. Keep the manager as fallback.

---

# Passkeys vs Passwords

**Passwords (old):**
- You create them — guessable
- Reused — leak everywhere
- Phishing works
- Need separate 2FA

**Passkeys (new):**
- Device-generated — unique per site
- Nothing to steal on the server
- Phishing fails (domain doesn't match)
- Already 2 factors (possession + biometrics)

**Best practice in 2026:** passkey where you can, manager for the rest.

## Notes
Contrast without a table. Reinforce that it's a complementary transition. Show [passkeys.directory](https://passkeys.directory). Encourage trying it today on Google/Apple ID.

---

# Have you been exposed? Let's check now.

## [haveibeenpwned.com](https://haveibeenpwned.com)

1. Enter your email
2. 🟢 Green = safe (for now)
3. 🔴 Red = you were in a breach → see where/what leaked

**If red:**
- Change the password on that site + anywhere you reused it
- Enable 2FA → click **Notify me**

> Live demo — volunteer without showing on screen

## Notes
CRITICAL DEMO with a test email. Troy Hunt, no spam. Show Pwned Passwords. QR in the corner so they can follow along.

---

# 2FA is mandatory + AI phishing

**Enable now on 5:** Email • Bank • Apple/Google • Instagram/TikTok • Finance

**Ranking:** Passkey > Authenticator app (Ente/Aegis/Proton/2FAS) > SMS

**Phishing in 2026:** flawless emails/SMS, cloned voices, pixel-perfect sites.

**Rule:** Never click a login link from email/SMS. Go directly to the site.

> 2FA is the seatbelt when the password fails

## Notes
Show TOTP QR. SMS is weak (SIM swap). Compare old vs AI phishing side by side. Passkeys solve phishing.

---

# PART B — PRIVACY
## Taking back control

> "Nothing to hide" ≠ "Nothing to protect"

Privacy is **choice**: what you share, with whom, when.

## Notes
Myth that privacy is only for criminals. Let's close the windows left wide open by default.

---

# Myth: "Incognito Mode protects me"

**What it DOES:**
- Clears history/cookies locally when you close
- Good for lending your laptop

**What it DOESN'T:**
- Doesn't hide your IP (ISP/boss can see)
- Doesn't block Google/Facebook tracking
- Not a VPN, not anonymity

> You wipe footprints at home, but street cameras still record.

## Notes
Show Chrome's incognito warning. Ask who uses it for privacy. Use humor to demystify.

---

# Why do you see cookie banners?

## EU Cookie Law (GDPR + ePrivacy)

- In the EU, tracking requires **consent**
- **Accept all** = green light for 100+ trackers
- **Reject / Necessary only** = essentials only

**Tip:** Be annoying, always click Reject. Use **Consent-O-Matic**.

## Notes
Show a real banner → Manage → 100 partners = shock. Essentials vs marketing. You have the right to reject without losing access.

---

# Do Not Track and Global Privacy Control

- **DNT (2009):** "please don't track me" → **nobody honored it**
- **GPC (2020+):** successor with **legal teeth** (CA + EU/GDPR)

Enable GPC: Brave has it on by default • Firefox → Privacy → GPC

> DNT is dead. GPC has teeth.

→ [globalprivacycontrol.org](https://globalprivacycontrol.org)

## Notes
Optional DNT failed. GPC backed by EFF, enforceable. Demo in Brave.

---

# Is your phone tracking you?

## Ad Tracking IDs — turn off in 30s

- **iPhone (IDFA):** Settings → Privacy → Tracking → turn off "Allow Apps to Request to Track"
- **Android (GAID):** Settings → Privacy → Ads → Delete ID + turn off personalization

> Do it now on your phone

## Notes
Interactive DEMO. Side-by-side screenshots. Doesn't remove ads, but stops cross-app profiling. ATT cut tracking by 60%+.

---

# What is DNS?

You type `google.com` → DNS translates to `142.250.180.14`

If you control DNS, you **block malware/ads before they load**.

> **Building doorman.** For the whole house, set it on the **router** — every device protected with nothing to install per device.

## Notes
Phonebook analogy. Diagram Device → DNS → Internet. Lightweight, fast, works on smart TV. Not a VPN, it's complementary.

---

# DNS Filtering — 3 doormen

**1. Cloudflare Families** — [one.one.one.one/family](https://one.one.one.one/family)
- `1.1.1.2` malware • `1.1.1.3` malware+adult

**2. DNS4EU** — [joindns4.eu](https://www.joindns4.eu)
- EU, GDPR, no logs, `86.54.11.13`

**3. NextDNS** — [my.nextdns.io](https://my.nextdns.io)
- Customizable, 300k/month free, per device

## Notes
Compare in 3 short bullets. Show changing DNS on iPhone/Android and on the router (whole house). Recommend NextDNS for full control.

---

# DEMO — NextDNS in 2 minutes

1. Go to **[my.nextdns.io](https://my.nextdns.io)** → free account
2. Lists: NextDNS Ads & Trackers + StevenBlack
3. Turn on **Native Tracking Protection**
4. Install profile (iOS) / app (Android) / router

See in real time: blocks, % trackers, per device

## Notes
Demo dashboard with graph. Before/after on an ad-heavy site. Free tier covers 2-3 people. Pi-hole for nerds.

---

# Ad-blocking — Not aesthetics, it's privacy

Ads = **trackers** across sites.

Blocking = faster, more battery, less malware.

> Next: the 3 tools that matter

## Notes
Example news site 3s vs 10s, 50 trackers vs 2. Transition.

---

# uBlock Origin + Privacy Badger

**uBlock Origin — for everyone** — [ublockorigin.com](https://ublockorigin.com)
- Install and forget. Lightweight, 90% blocked.

**Privacy Badger (EFF)** — [privacybadger.org](https://privacybadger.org)
- Learns on its own, blocks whoever tracks you on 3+ sites.

> Start with uBlock. Enough for 90% of people.

## Notes
Show Chrome/Firefox install. Don't use 5 ad-blockers at once. For beginners, this is enough.

---

# nuMatrix — For the curious

**Fork of uMatrix** — [codeberg.org/arek/nuMatrix](https://codeberg.org/arek/nuMatrix)

- Matrix per domain: JS, cookies, XHR, media
- Surgical control over what each site loads
- Steeper learning curve, may break sites at first

> Power users: try it after you've mastered uBlock

## Notes
Screenshot of the matrix. For those who want to understand everything. Warning that it breaks sites until you learn. Separated from previous slide to not overwhelm beginners.

---

# Email Aliasing — Hide the real one

### Part 1: Tricks (organization, not privacy)

- **Gmail ignores dots:** `joao.silva@gmail.com` = `joaosilva@gmail.com`
- **Gmail `+`:** `joao+shop@gmail.com` → filterable, but easy to strip
- **Outlook:** `+` + **real aliases** ([outlook.live.com](https://outlook.live.com) → up to 10)

> Useful for organizing, **doesn't hide** — dots/+ stripped in a second

## Notes
Demo `joao+test` creates a filter. Outlook real alias. Explain it's trivial to clean, not privacy.

---

# Email Aliasing — Real privacy

### Part 2: Random aliases

Instead of `joao@gmail.com` → `joao.shop.8f3k@random.simplelogin.com`

- Spam? **Turn off the alias** (1 click)
- Breach? You know **who sold** your data
- Reply without revealing the real address

**Use:** [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io) • iCloud Hide My Email • Firefox Relay

> Gmail/Outlook to organize. SimpleLogin/Addy for privacy.

## Notes
Demo creating an alias in SimpleLogin/Proton Pass. One alias per service = digital hygiene. Link to manager = disposable identity per site.

---

# VPN — Encrypted tunnel, not an invisibility cloak

**What it DOES:**
- Encrypts to the VPN server — hides IP from Wi-Fi/ISP/boss
- Useful on public Wi-Fi, censorship, geo-blocks

**What it DOESN'T:**
- Doesn't block trackers/cookies
- Not anonymous while logged into Google
- Doesn't protect from malware

> For daily use, **NextDNS + uBlock** already give you 80%

## Notes
Analogy: armored truck to the central post office, then it goes open. Not total privacy, it's transport. Show when to use it.

---

# VPN — The free trap and how to choose

**⚠️ Free = you are the product**
SuperVPN, TurboVPN, GeckoVPN (100M+) — sold logs, leaked data.

**How to choose (audited, WireGuard, RAM-only):**
- **Mullvad** — [mullvad.net](https://mullvad.net) (5€/month, no email needed)
- **Proton VPN** — [protonvpn.com](https://protonvpn.com) (honest free tier)
- **IVPN** — [ivpn.net](https://www.ivpn.net)

> If it's free and it's not Proton, be suspicious.

## Notes
Strong warning: worse than no VPN. Many free ones are owned by the same Chinese company. If you can only use free, Proton Free is the only trustworthy one.

---

# Dirty links — clean tracking before sharing

- Links come dirty: `?utm_source=...&fbclid=...&igsh=...` that identify who clicked/shared
- Instagram `igsh` and Facebook `fbclid` enable **doxing** — recipient can trace who shared it
- **Rule:** share only `https://site.com/page` — delete everything after `?`

**Tools:**
- **Android:** [altsea.app](https://altsea.app) — paste link → copy clean
- **Desktop:** [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper) — auto-removes on copy

> Sharing a dirty link = sharing your trail

## Notes
LIVE DEMO: copy an Instagram link with `?igsh=` → paste into altsea.app → show clean link. Explain doxing: `igsh` traces back to the sharer's profile. UTM isn't essential — site loads fine without `?utm_...`. Show Tracking Token Stripper cleaning on desktop when you copy.

---

# Your Action Plan — TODAY (5 steps)

1. ✅ Manager (Bitwarden) + import + change email/bank
2. ✅ First passkey (Google/Apple)
3. ✅ [haveibeenpwned.com](https://haveibeenpwned.com) + Notify me
4. ✅ Phone: disable tracking + NextDNS/1.1.1.3 DNS
5. ✅ Browser: [ublockorigin.com](https://ublockorigin.com)

> Photo this slide. 30 min tonight.

## Notes
Most important slide, leave 2 min. Photo. 1+2+3 = 80% of the gain.

---

# Resources — Save this slide (1/2)

**Accounts & Passwords**
- [haveibeenpwned.com](https://haveibeenpwned.com)
- [bitwarden.com](https://bitwarden.com) • [proton.me/pass](https://proton.me/pass)
- [passkeys.directory](https://passkeys.directory)
- [ente.io/auth](https://ente.io/auth) • [getaegis.app](https://getaegis.app)

**Privacy**
- [one.one.one.one/family](https://one.one.one.one/family)
- [joindns4.eu](https://www.joindns4.eu)
- [my.nextdns.io](https://my.nextdns.io)
- [ublockorigin.com](https://ublockorigin.com)

## Notes
First half of links. Say the PDF has everything clickable. Second half on next slide.

---

# Resources — Save this slide (2/2)

**Email & VPN**
- [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io)
- [mullvad.net](https://mullvad.net) • [protonvpn.com](https://protonvpn.com)
- [privacybadger.org](https://privacybadger.org) • [globalprivacycontrol.org](https://globalprivacycontrol.org)

**Test & Tricks**
- [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- [altsea.app](https://altsea.app)
- [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper)
- support.google.com/mail/answer/5238509

> PDF with all links will be shared

## Notes
Second half. Linktree/Notion with everything. Mention phase 2 videos.

---

# QR Codes — Passwords & Accounts

## Notes
Give 30s to photograph. Starter kit for passwords. HaveIBeenPwned is urgent.

---

# QR Codes — Privacy & Protection

## Notes
Second batch. NextDNS has the biggest impact. uBlock on laptop. SimpleLogin for alias.

---

# Questions?
## Thank you!

### Security is a marathon, not a sprint.

Start with 1 step today.

## Notes
Wrap up, Q&A. If time, VPN vs DNS or Brave vs Firefox.
