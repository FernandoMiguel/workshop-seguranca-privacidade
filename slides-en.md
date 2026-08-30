# Online Security & Privacy — Hands-On

### A 75-minute practical workshop for beginners

**Passwords • Passkeys • Privacy • DNS • Ad-blocking**

Fernando 🐼 — September 2026

## Notes
Welcome! No jargon, no scare tactics — just practical steps you can use today. Everything here is free. Jump in anytime with questions. You'll leave with a 5-step checklist you can do tonight.

---

# What you'll walk away with today

## 7 quick wins in 75 minutes

- 🔐 Passwords that actually stand up to hackers
- 🔑 Passkeys — the end of passwords
- 🕵️ How to check if you've already been breached
- 📵 How to stop your phone from tracking you
- 🛡️ Blocking ads and malware at the DNS level
- 🧹 Stripping tracking junk from links (and avoiding doxxing)
- 🔒 VPNs — when they help, and when they're a trap

> Keep your phone handy — we're doing this live.

## Notes
Set expectations: this is hands-on, not a lecture. Tell them by the end of Part A they'll have moved at least one account to a password manager. Keep it visual and fast.

---

# PART A — PASSWORDS
## Your first line of defense

> "Security isn't a product — it's a habit."

Get this one habit right and you get 80% of the protection.

## Notes
High-energy transition. Ask: "Who's reused the same password on multiple sites?" Hands up — no shame, it's normal. We're about to fix it for good.

---

# This is serious — and it's personal.

- **123456** and **password** are still #1 and #2 worldwide (2024)
- **65%** of people reuse the same password everywhere
- One breach → every account you own is at risk

**How it works — credential stuffing:** a site leaks your email + password → bots automatically try it on Gmail, Instagram, your bank.

> One password is a master key to every door you own.

## Notes
Open haveibeenpwned.com but don't search yet. Mention the 2012 LinkedIn breach — those passwords are still being tried today. HIBP now has 14+ billion breached accounts.

---

# What makes a password *strong*?

### Go long, not clever

- **Weak:** `P@ssw0rd!` — 8 characters, completely predictable
- **Strong:** `correct horse battery staple` — 4 random words, 28 characters
- **Ideal:** `k9$Lp-27q-VALE-blue-thunder-482` — randomly generated

**The golden rule:** Long (14–16+ characters) • Unique for every site • Truly random

> If you can remember it, it's too weak. Let your manager remember it for you.

## Notes
Explain entropy simply: each extra character makes it exponentially harder to guess. Live demo the Bitwarden generator. Mention Diceware for your one master passphrase — four random words you *can* remember.

---

# Password managers
## Your encrypted vault

Think of it as a safe that only opens with your **master passphrase**.

You memorize **one** strong passphrase. It remembers the other 200 for you.

**Our top picks (all zero-knowledge):**
- **Bitwarden** — [bitwarden.com](https://bitwarden.com)
- **Proton Pass** — [proton.me/pass](https://proton.me/pass)
- **1Password** — [1password.com](https://1password.com)

> Zero-knowledge means not even they can see your passwords.

## Notes
Use the safe vs. "key under the doormat" analogy. Live demo: create a Bitwarden account, generate a 20-character password, show autofill. Warn: saving passwords in your browser without a master password isn't safe.

---

# Demo — switch to a manager in 3 steps

1. **Install** Bitwarden (app + browser extension) and set your master passphrase
2. **Import** everything from Chrome / Firefox — it's two clicks
3. **Fix the top 5 first:** Email → Bank → Instagram → Google/Apple → Finance

**Pro tip:** Turn on 2FA inside Bitwarden itself.

> Do this over lunch — five minutes and you're 80% there.

## Notes
Show the import live or with screenshots. Tell them not to boil the ocean — just fix the five accounts that would hurt most if hacked. Show Bitwarden's "Reused" and "Exposed" reports.

---

# Passkeys — the future without passwords

The site keeps the **lock** (public key). Your phone keeps the **key** (private key).

You unlock with Face ID, fingerprint, or your PIN.

- ✅ Phishing-proof by design
- ✅ Nothing to steal from the server
- ✅ Faster than typing a password

→ See what's ready: [passkeys.directory](https://passkeys.directory)

## Notes
Lock-and-key analogy works well here. Demo: myaccount.google.com → Security → Passkeys → Create. It lives in iCloud Keychain / Google Password Manager. Keep your password manager as a backup for sites that don't support passkeys yet.

---

# Passkeys vs. passwords

**Passwords (the old way):**
- You make them up — so they're guessable
- You reuse them — so one leak exposes everything
- Phishing works
- You need 2FA as an extra step

**Passkeys (the new way):**
- Your device creates them — unique for every site
- Nothing valuable sits on the server
- Phishing fails (the domain has to match)
- They're already two factors (something you have + something you are)

**The move in 2026:** use a passkey wherever you can, password manager everywhere else.

## Notes
No need for a table — just contrast. Emphasize they're complementary, not competing. Show passkeys.directory and nudge them to try it today on their Google or Apple ID.

---

# Have you been breached? Let's find out.

## [haveibeenpwned.com](https://haveibeenpwned.com)

1. Type in your email
2. 🟢 Green = you're clear — for now
3. 🔴 Red = you've been in a breach → see where and what leaked

**If it's red:**
- Change that password *and* everywhere you reused it
- Turn on 2FA → click **Notify me** so you'll know next time

> Live demo — we'll use a test address so no one has to share theirs.

## Notes
This is the big live demo. Use a test email you know is breached. Explain who Troy Hunt is and that the site doesn't spam. Show "Pwned Passwords" too. Point to the QR in the corner so people can follow on their phones.

---

# 2FA is non-negotiable — and phishing just got scary good

**Turn it on today for these 5:** Email • Bank • Apple/Google • Instagram/TikTok • Finance

**What to use, best to worst:** Passkey > Authenticator app (Ente / Aegis / Proton / 2FAS) > SMS

**Phishing in 2026:** flawless emails and texts, cloned voices, pixel-perfect fake sites.

**The rule:** Never tap a login link from an email or text. Go to the site yourself and log in.

> 2FA is the seatbelt for when your password fails.

## Notes
Show a TOTP code spinning. Explain SMS is weak because of SIM swapping. Put an old-school phishing email next to an AI-generated one — indistinguishable now. Passkeys are the real fix for phishing.

---

# Social engineering — the weakest link is you

- They don't hack your PC — they hack **you**: urgency, fear, curiosity
- **WhatsApp “Hi mum/dad, I changed my number”** — asks for money via MB WAY
- **Fake tech support:** “I'm from Microsoft / your bank — install AnyDesk”

> Stop. Doubt it. Verify through another channel (call the old number).

## Notes
Show a real WhatsApp mum/dad scam screenshot + cloned voice call. The rule: urgency = red flag. Hang up and call them yourself.

---

# Stop. Check. Only then click.

- **Hover before you click** — the real destination shows at the bottom. Does it match?
- Email or text with an urgent link or attachment? Don't open it. Go directly to the site or app
- Downloads only from official sites — `https` + exact domain (`fnac.pt` ≠ `fnac-pt-offer.com`)

> Two seconds of checking saves hours of cleaning up.

## Notes
Demo hover on desktop vs long-press on mobile. Show a fake domain with hyphens. Attachments .zip/.exe = never open.

---

# PART B — PRIVACY
## Taking back control

> "I have nothing to hide" is not the same as "I have nothing to protect."

Privacy is **choice** — what you share, with whom, and when.

## Notes
Reframe the myth: privacy isn't about having something to hide, it's about closing windows that are open by default. This section is about quietly taking that control back.

---

# Myth: "Incognito Mode makes me private"

**What it *does* do:**
- Wipes history and cookies *on that device* when you close the window
- Handy if you're lending someone your laptop

**What it *doesn't* do:**
- It doesn't hide your IP — your ISP and your boss can still see where you went
- It doesn't stop Google or Facebook from tracking you
- It's not a VPN, and it's not anonymity

> Incognito wipes footprints off your floor, but the street cameras are still rolling.

## Notes
Show Chrome's actual Incognito disclaimer — most people have never read it. Ask who uses it to be "private" — a little humor lands well here.

---

# So why all the cookie banners?

## The EU Cookie Law (GDPR + ePrivacy)

- In the EU, tracking needs your **consent**
- **Accept all** = you just green-lit 100+ trackers
- **Reject / Necessary only** = you get the site without the surveillance

**Make it a habit:** Always hit Reject. If you're tired of clicking, use **Consent-O-Matic**.

## Notes
Show a real banner → "Manage preferences" → 100+ "partners" — that shock value sticks. Explain "necessary" vs "marketing." Remind them they can say no and still use the site.

---

# Do Not Track vs. Global Privacy Control

- **DNT (2009):** "Please don't track me" → **everyone ignored it**
- **GPC (2020+):** the successor with **actual legal weight** (California + EU/GDPR)

How to turn on GPC: Brave has it on by default • Firefox → Settings → Privacy → turn on GPC

> DNT is dead. GPC actually has teeth.

→ [globalprivacycontrol.org](https://globalprivacycontrol.org)

## Notes
DNT failed because it was voluntary. GPC is backed by the EFF and is enforceable. Quick demo in Brave's settings.

---

# Is your phone tracking you across apps?

## Ad tracking IDs — switch them off in 30 seconds

- **iPhone (IDFA):** Settings → Privacy & Security → Tracking → turn off "Allow Apps to Request to Track"
- **Android (GAID):** Settings → Privacy → Ads → Delete advertising ID + turn off ad personalization

> Do this right now, on your phone.

## Notes
Live, interactive demo. Show side-by-side screenshots. Be clear: this doesn't remove ads, it stops apps from building one profile about you across every app. Apple's ATT cut cross-app tracking by over 60%.

---

# Wait — what *is* DNS?

You type `google.com` → DNS translates it to `142.250.180.14`

If you control DNS, you **block malware and ads before they even load**.

> Think of it as the **building's doorman.** Set it once on your **router** and every device in the house is protected — no app to install on each phone, TV, or laptop.

## Notes
Phone book analogy for DNS. Sketch: Device → DNS → Internet. Emphasize it's lightweight, fast, works on smart TVs. It's not a VPN — it's the perfect complement to one.

---

# DNS filtering — pick your doorman

**1. Cloudflare Families** — [one.one.one.one/family](https://one.one.one.one/family)
- `1.1.1.2` blocks malware • `1.1.1.3` blocks malware + adult content

**2. DNS4EU** — [joindns4.eu](https://www.joindns4.eu)
- EU-run, GDPR-friendly, no logs — `86.54.11.13`

**3. NextDNS** — [my.nextdns.io](https://my.nextdns.io)
- Fully customizable, 300k queries/month free, per-device profiles

## Notes
Keep it to three short options. Show how to change DNS on iPhone/Android and, more importantly, on the router so the whole house is covered. Recommend NextDNS if they want the most control.

---

# Demo — NextDNS in 2 minutes

1. Go to **[my.nextdns.io](https://my.nextdns.io)** → create a free account
2. Enable blocklists: NextDNS Ads & Trackers + StevenBlack
3. Turn on **Native Tracking Protection**
4. Install the profile (iOS) / app (Android) / or set it on your router

Then watch the live log: what got blocked, what percentage is tracking, broken down by device.

## Notes
Show the dashboard graph. Do a before/after on an ad-heavy news site. Free tier is enough for 2–3 people. Mention Pi-hole for the tinkerers.

---

# Ad blockers — it's not about looks, it's about privacy

Ads *are* trackers that follow you from site to site.

Blocking them means faster pages, better battery, and less malware.

> Up next: the 3 tools that actually matter.

## Notes
Show a news site loading in 3 sec vs 10 sec, 50 trackers vs 2. This sets up the next two slides.

---

# uBlock Origin + Privacy Badger

**uBlock Origin — for everyone** — [ublockorigin.com](https://ublockorigin.com)
- Install it and forget it. Lightweight, blocks ~90% out of the box.

**Privacy Badger (EFF)** — [privacybadger.org](https://privacybadger.org)
- Learns as you browse — if it sees the same tracker on 3+ sites, it blocks it.

> Start with uBlock Origin. That's enough for 90% of people.

## Notes
Show how to install in Chrome/Firefox. Warn them not to run five ad blockers at once — they'll fight each other. For beginners, this combo is the sweet spot.

---

# nuMatrix — for the curious

**A modern fork of uMatrix** — [codeberg.org/arek/nuMatrix](https://codeberg.org/arek/nuMatrix)

- A grid: which domains can run JS, set cookies, make XHR, load media
- Surgical control over what each site is allowed to do
- Steeper learning curve — expect sites to break at first

> For power users: try this *after* you're comfortable with uBlock Origin.

## Notes
Show a screenshot of the matrix. Explain it's for people who want to see everything. Warn that it'll break sites until you learn it. That's why it's on its own slide — so beginners don't feel overwhelmed.

---

# Email aliasing — hide your real address

### Part 1: Tricks (handy for organizing, not for privacy)

- **Gmail ignores dots:** `joao.silva@gmail.com` is the same as `joaosilva@gmail.com`
- **Gmail `+` trick:** `joao+shop@gmail.com` → easy to filter, but trivial to strip out
- **Outlook:** `+` plus **real aliases** ([outlook.live.com](https://outlook.live.com) → up to 10)

> Great for organizing, **useless for privacy** — anyone can remove the dot or `+` in a second.

## Notes
Live demo: send to `joao+test@gmail.com` and show the filter it creates. Show Outlook's real alias screen. Make the point: this is convenient, but it's not hiding you.

---

# Email aliasing — real privacy

### Part 2: Random aliases

Instead of `joao@gmail.com`, you give out `joao.shop.8f3k@random.simplelogin.com`

- Spam? **Kill the alias** with one click
- Breach? You instantly know **who sold your address**
- You can still reply without ever revealing your real email

**Use:** [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io) • iCloud Hide My Email • Firefox Relay

> Gmail/Outlook for organizing. SimpleLogin/Addy for actual privacy.

## Notes
Demo creating an alias in SimpleLogin or Proton Pass. One alias per service is digital hygiene — if one leaks, you just burn that alias. Pair it with your password manager and you get a disposable identity per site.

---

# Shopping online — pay without exposing your card

- **Virtual / single-use card:** [MB WAY](https://www.mbway.pt) • Revolut single-use • [Privacy.com](https://privacy.com)
- Check the shop: `https` + padlock + business ID/contact visible — beware `fnac-offer.com`
- Turn on notifications and limits — if it leaks, you kill the virtual card in 10 seconds, physical card stays safe

> Virtual card leaked? Cancel in 10 seconds. Physical card untouched.

## Notes
Demo MB WAY virtual card creation. Show Revolut single-use toggle. Check shop NIF/contact. Serious shops have HTTPS + real contact info.

---

# VPN — an encrypted tunnel, not an invisibility cloak

**What it *does* do:**
- Encrypts everything to the VPN server — hides your IP from the coffee-shop Wi-Fi, your ISP, your employer
- Useful on public Wi-Fi, to get around censorship, or for geo-blocked content

**What it *doesn't* do:**
- It doesn't block trackers or cookies
- It doesn't make you anonymous if you're logged into Google
- It doesn't protect you from malware

> For everyday life, **NextDNS + uBlock Origin** already get you 80% of the way there.

## Notes
Analogy: it's an armored truck to the central post office — after that, your mail goes out normally. It's transport protection, not total privacy. Be clear about when it actually helps.

---

# VPNs — the free trap and how to pick a good one

**⚠️ If it's free, *you're* the product**
SuperVPN, TurboVPN, GeckoVPN (100M+ installs each) — all caught selling logs and leaking data.

**How to choose (look for: audited, WireGuard, RAM-only servers):**
- **Mullvad** — [mullvad.net](https://mullvad.net) (€5/month, no email required)
- **Proton VPN** — [protonvpn.com](https://protonvpn.com) (the one honest free plan)
- **IVPN** — [ivpn.net](https://www.ivpn.net)

> If it's free and it's not Proton, assume you're paying with your data.

## Notes
Be blunt: a bad VPN is worse than no VPN. Many of the free ones are owned by the same handful of Chinese companies. If you can only use free, Proton Free is the only one I'd trust.

---

# Home Wi-Fi vs. street Wi-Fi

- **At home:** router with WPA3 + filtered DNS (NextDNS) = whole house protected
- **Out (café / airport / hotel):** open network = unencrypted traffic is visible — turn off “auto-join”
- Really need it? Use **mobile data** or a **VPN** (Mullvad/Proton) — everything else already goes over `https`

> At home your doorman is the router. On the street, bring your own.

## Notes
Explain evil twin (“Hotel WiFi FREE” clone), open hotspot with no password. Show how to turn off auto-join on iOS/Android. Mobile data beats open Wi-Fi.

---

# Messy links — clean tracking before you share

- Links often come dirty: `?utm_source=...&fbclid=...&igsh=...` — they identify who clicked and who shared
- Instagram's `igsh` and Facebook's `fbclid` can actually **doxx** you — anyone with the link can trace it back to the person who shared it
- **The rule:** only share `https://site.com/page` — delete everything after the `?`

**Tools to clean them:**
- **Android:** [altsea.app](https://altsea.app) — paste the link, copy the clean version
- **Desktop:** [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper) — strips it automatically when you copy

> Sharing a messy link is sharing your trail.

## Notes
Live demo: copy an Instagram link with `?igsh=` → paste into altsea.app → show the clean link. Explain the doxxing risk: that `igsh` token can lead back to the sharer's profile. UTM params aren't needed — the page loads fine without `?utm_...`. Show Tracking Token Stripper cleaning it on desktop as you copy.

---

# Your action plan — do this TODAY (5 steps)

1. ✅ Password manager (Bitwarden) → import → fix email + banking first
2. ✅ Create your first passkey (Google/Apple)
3. ✅ Check [haveibeenpwned.com](https://haveibeenpwned.com) → click Notify me
4. ✅ Phone: turn off ad tracking + set DNS to NextDNS / 1.1.1.3
5. ✅ Browser: install [ublockorigin.com](https://ublockorigin.com)

> Snap a photo of this slide. Give yourself 30 minutes tonight.

## Notes
The most important slide — leave it up for a full two minutes. Tell them to take a photo. Steps 1+2+3 alone get them 80% of the benefit.

---

# Resources — save this slide (1/2)

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
First half of the links. Tell them the PDF has everything clickable. The second half is on the next slide.

---

# Resources — save this slide (2/2)

**Email & VPN**
- [simplelogin.io](https://simplelogin.io) • [addy.io](https://addy.io)
- [mullvad.net](https://mullvad.net) • [protonvpn.com](https://protonvpn.com)
- [privacybadger.org](https://privacybadger.org) • [globalprivacycontrol.org](https://globalprivacycontrol.org)

**Test & Tricks**
- [coveryourtracks.eff.org](https://coveryourtracks.eff.org)
- [altsea.app](https://altsea.app)
- [Tracking Token Stripper](https://github.com/jparise/chrome-utm-stripper)
- support.google.com/mail/answer/5238509

> The PDF with all links will be shared.

## Notes
Second half. Mention you'll share a Linktree/Notion page with everything. Tease the Phase 2 videos.

---

# QR Codes — Passwords & Accounts

## Notes
Give them 30 seconds to snap photos. This is the starter kit for passwords. Emphasize HaveIBeenPwned as the urgent one.

---

# QR Codes — Privacy & Protection

## Notes
Second batch. Call out NextDNS as the highest-impact one. uBlock Origin for the laptop, SimpleLogin for aliases.

---

# Questions?
## Thank you!

### Security is a marathon, not a sprint.

Start with one step today.

## Notes
Wrap up, invite Q&A. If there's extra time, riff on VPN vs DNS or Brave vs Firefox.
