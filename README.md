# Google Accounts Creator · The Ultimate Tool for Gmail Automation 🚀

Accounts Creator - a program for automatic bulk creation of Google accounts. The main difficulty of mass account registration is Google's anti‑bot protection.  The protection system successfully recognizes the frequent creation of accounts from the same device or IP.  And even if you use incognito mode and constantly change IP, through a router reboot or proxy, Google will easily recognize this.  
Our software is designed to solve this problem. It uses advanced **fingerprint spoofing systems**, supports **proxies**, and, just as importantly, connects them correctly to avoid leaks.

## More info: https://youtube-booster.space/google-accounts-creator/

![image](https://github.com/user-attachments/assets/640e4742-82ba-4827-88ba-36e68254dde6)

---

## Table of Contents
- [Features](#features)
- [Demo](#6-demo--screenshots--gif)
- [Quick Start](#7-quick-start)
- [Configuration](#8-configuration)
- [Advanced settings](#9-advanced-settings)
- [Best Practices & Tips](#10-best-practices--tips)
- [Troubleshooting / Known Errors](#14-troubleshooting--known-errors)
- [Roadmap](#15-roadmap)
- [Changelog](#16-changelog)
- [FAQ](#18-faq)

---

## Features ✅ <a id="features"></a>

- Unlimited account creation.  
- Mobile, residential, static (socks5/http) proxy support. Also, the bot allows to use API for IP reset.  
- The bot generates a profile for each account that stores cookies and the original system fingerprint. This reduces the risk of bans and removes the need to authorize each time an account is used.  
- Allows you to set two‑factor authentication for an account, which also greatly increases the trustworthiness of the account.  
- The profile photo upload feature is available.  
- Available 17 services for SMS verification. There is also an option to connect a service that is currently not on the list.  
- You can select the country of the number and the cellular operator.  
- Ability to use one number to confirm multiple accounts.  
- Create Gmail accounts without phone verification (up to 80‑90 % success rate).  
- PerfectCanvas technology support.  
- Allows you to create accounts of any country and language.  
- Available automatic name generation or use your own lists.  
- Ability to set the age and gender of the account user.  
- The list of created accounts is saved in xlsx or txt files.  

---

## Demo 📺 <a id="6-demo--screenshots--gif"></a>: https://www.youtube.com/embed/Oy8ypJhSAgk

---

## Quick Start ⚙️ <a id="7-quick-start"></a>

### Prerequisites
- Windows 8.1/10/11 (64‑bit) **or** Windows Server 2016+  
- FingerprintSwitcher key  
- Dedicated mobile 4G/LTE proxy with API IP‑switch **or** residential with a dynamic IP  
- Refill the balance on one of the available SMS services  

### Installation
1. **Download** the latest release from the repository.  
2. **Launch** `GoogleAccReger.exe`. During the first startup, the program will automatically install all necessary components and libraries, so the startup may take longer. Updates are made according to the same principle when restarting; if a new version of the program is available, it will be installed automatically. Nothing is required from you.

### First run
1. Paste your FingerprintSwitcher and SMS API keys.  
2. Add proxies or a proxy API endpoint.  
3. Click **OK** – creation starts immediately and runs until stopped.  

---

## Configuration 🔧 <a id="8-configuration"></a>

| Параметр | Описание |
|----------|----------|
| **Number of accounts** | The parameter specifies how many accounts to create. **(DEPRECATED, now the bot works infinitely)** |
| **FingerprintSwitcher API key** | Enter the API key from the service that you received earlier. |
| **Number of uses per fingerprint** | The function sets how many times the same fingerprint will be reused. Sometimes high‑quality prints come across, which can be used 3 or more times. However, for reliability and protection from a ban, I recommend using the value “1”. |
| **Enable mobile fingerprints** | If the function is enabled, the script will receive not only desktop fingerprints from the FingerprintSwitcher server, but also mobile ones. ⚠️ *YouTube Booster doesn't support mobile fingerprints.* |
| **Detailed logs** | The feature enables more detailed logging of the Fingerprint module. Use only if there are problems with the script. |
| **The path to the folder with profiles** | Profiles for registered accounts will be saved in this folder. |
| **Accounts gender** | Choose the gender of accounts. |
| **Names import type** | The program can generate names automatically, but you can also specify them manually. |
| **List with names** | If in the previous step, you select "Manually" to generate the required number of first and last names, <https://www.name-generator.org.uk/quick/>. First name should be followed by last name. Generate only male or female names into one list. Next, you can specify the gender in the settings. Save the data to a `.txt` file with UTF‑8 encoding. As a result, the file should look like this: |
| **Names language** | If in the previous step you select "Automatically" specify the language of names and surnames. |
| **Year of birth** | Set the desired age of account users. |
| **Backup mail** | Select the type of backup mail for your Google account: *Fake* or *Real*. Fake mail is not created; an email is simply invented and entered during registration. Real mail is real accounts of some inexpensive service like Rambler.ru. It is recommended to select “Real” because during re‑authorizing, Google may request a code that will be sent to the backup email. |
| **If you chose “Real”…** | I recommend buying Rambler.ru mail with activated IMAP, SMTP, POP3. Other services are also suitable. You can buy them here:<br>• <https://accsmarket.com/en/catalog/drugie-pochty/rambler><br>• <https://install-shop.com/?cat_id=327#><br>• <https://buyinstaprom.com/?cat_id=5650><br>• <https://accs-shop.com/?cat_id=4925><br>After the purchase, you will get a txt file in the format “Email:Password”. |
| **Path to backup mail file** | Specify the path to this txt file. |
| **Choose proxy type** |  |
| **Mobile (Change IP on request)** | Enter the proxy below. Format: `http://login:password@ip:port`. Then fill in “API for IP change” field (link that changes the proxy IP when you go to it). |
| **Regular proxies** | Specify the path to the `.txt` file with the proxies. Format: `http://login:password@ip:port`, one per line. |
| **Account creation without SMS verification** | The feature allows you to break the registration process when requesting SMS verification. Useful for those who are not in a hurry and want to save money. About 15‑20 % of accounts are created without SMS confirmation. |
| **SMS activation service** | Select the service which you have funded earlier. |
| **SMS activation service API key** | Enter API key you received earlier. |
| **Country of phone number** | Select the same country in which your proxy located. |
| **Cellular carrier (optional)** | Specify the name of the mobile operator (e.g., *Vodafone*). Only the numbers of this operator will be requested. |
| **How many times to reuse numbers** | Some SMS activation services allow you to use the number several times. Choose how many times you want to use the same phone number for registration. Recommended no more than 2‑4. |
| **Enable two‑factor authentication (2fa)** | Activates 2fa in accounts (Google Authenticator). |
| **Upload avatars** | Enables picking of avatar for account (may be unstable on slow proxies). |
| **Number of unsuccessful attempts** | Sets the number of unsuccessful attempts before the script stops. Useful if Google changes the registration procedure. |

![image](https://github.com/user-attachments/assets/d7c597b1-f36c-4ceb-b6ba-5fd28216f405)


---

## Advanced settings 🌐 <a id="9-advanced-settings"></a>

- If you are the site owner, you can collect fingerprints from users of your site. *Learn more.*  
- **Use custom servers.** Works only if custom server functionality is enabled in your account. Otherwise, an error will occur. Compatible with PerfectCanvas.  
  - `true` – Use custom server to obtain fingerprint.  
  - `false` – Obtain fingerprint from the common server.  
- **PerfectCanvas rendering in real time.**  
  - `true` – If no static fingerprint match, canvas data will be rendered in real time from machines online.  
  - `false` – Search only the static database; if not found, an error will occur.  

---

## Transferring the licence 🔑 <a id="transferring-the-licence"></a>

If you receive **Too many usages** or **Only single instance allowed** while starting on a new server:  
1. Close the bot on the old host.  
2. Go to the licence reset page (sent to your email after purchase), submit the registered login.  
3. Wait **5 minutes**, run the software on a new instance.

---

## Best Practices & Tips 💡 <a id="10-best-practices--tips"></a>

- Buy a 3‑month FingerprintSwitcher key. Premium key has higher priority and shorter PerfectCanvas render queue (≈ 30 s vs. 2–5 min per print).  
- Set fingerprint **Reuse = 1**. Reusing fingerprints more than 1 time increases linkage risk.  
- Match the proxy country with the phone country. Mismatches dramatically raise SMS challenge rate.  
- Use mobile or residential proxies with API rotation. 4G/LTE egress rotates the ASN every request, mimicking real subscriber churn and slashing captcha hits.  
- Keep **max failures ≤ 10**. If Google silently changes the signup form, the bot stops early, saving SMS credits until you pull the next update.  
- Backup your profiles folder.  
- Enable 2FA for long‑term projects.  
- Disable avatar uploads on slow proxies (connections < 3 Mbps).  

---

## Troubleshooting / Known Errors 🐞 <a id="14-troubleshooting--known-errors"></a>

| Message | Likely cause | Fix |
|---------|--------------|-----|
| Too many usages / Only single instance allowed | Bot is already running elsewhere, or BAS glitch. | Close old host → reset licence via link → wait 5 min. If glitch: reboot the machine. |
| The key is not allowed to use right now | 1‑month FingerprintSwitcher key hit concurrency cap. | Upgrade to 3‑month key or wait 15 min. |
| Waiting for fingerprints… (≥ 30 min) | Queue saturation or expired API key. | Check key validity → rerun during daytime → consider Custom Server. |
| Failed to verify account via phone number. Let's get another Fingerprint. | Bad fingerprint, spammed phone, or flagged IP. | Bot auto‑retries 3 phones then switches fingerprint. |
| Proxy connection failed / Unable to reset modem | Wrong credentials or dead endpoint. | Test proxy; verify IP‑switch URL returns **OK**. |
| Wrong credentials or no licence | Typos, firewall blocking BAS licence host, licence expired. | Re‑enter creds → whitelist `*.bablosoft.com` → renew subscription. |
| Long captcha solving times (> 60 s) | 2Captcha balance < $0.5 or Recaptcha V3 complexity. | Top‑up balance or move to CapMonster self‑hosted. |

![image](https://github.com/user-attachments/assets/34a68ada-c36e-4e01-b3c9-483c0da6eb23)

---

## Roadmap 🗺️ <a id="15-roadmap"></a>

| ETA | Item | Status |
|-----|------|--------|
| 2025‑Q3 | Add secure apps enable support | 🟡 in progress |
| 2025‑Q3 | Implement own fingerprint database | ⚪ planned |
| 2025‑Q4 | Multi‑thread fingerprint pre‑fetcher to hide queue latency | ⚪ planned |
| 2025‑Q4 | Implement a more advanced patcher for prints | ⚪ planned |

---

## Changelog 📜 <a id="16-changelog"></a>

### [3.2.7] – 2025‑04‑22
- Custom Server support for fingerprint obtaining.  
- Updated BAS engine.  
- Minor bug fixes.  

### [3.2.6] – 2025‑04‑12
- Increased speed of account creation.  
- Script correction after Google sign‑up form update.  
- Minor bug fixes.  

### [3.2.5] – 2025‑04‑09
- Improved fingerprint filter function.  

Complete change log available on <https://youtube-booster.space/google-accounts-creator/>

---

## FAQ ❓ <a id="18-faq"></a>

- **Q:** What should I buy besides the Gmail creator app itself?  
  **A:** Premium key of FingerprintSwitcher – $20 per month. High‑quality proxies (mobile, residential, or server proxies). Service for SMS activations (optional, for phone verifications).  

- **Q:** What proxies are suitable?  
  **A:** Mobile LTE proxies (rotating IP via API requests) – strongly recommended. Residential proxies (a good alternative). Server proxies (static IPv4, IPv6).  

- **Q:** What is the percentage of account bans?  
  **A:** Account bans heavily depend on usage, software quality, and proxies. When used with YouTube Booster software, typically fewer than 5 % of accounts are banned.  

- **Q:** How long do accounts created with this Gmail creator bot typically last?  
  **A:** Accounts created with natural browser profiles and stable proxies can last for several years, depending primarily on usage patterns and proxy quality.  

- **Q:** Is the script bound to specific hardware?  
  **A:** Yes. The licence is bound to one computer or server. If you need to migrate to a new device, simply contact support to reset the binding.  

- **Q:** Is there a tutorial included?  
  **A:** Yes, a comprehensive tutorial is provided.

## More info: https://youtube-booster.space/google-accounts-creator/
