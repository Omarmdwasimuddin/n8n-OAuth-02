# 🔐 n8n OAuth2 — Google Sheets & Docs Integration Guide

> n8n এ Google Sheets ও Google Docs সংযুক্ত করার ধাপে ধাপে গাইড।

🔗 **পূর্বশর্ত:** আগে [n8n Self-Host Setup](https://github.com/Omarmdwasimuddin/n8n-Self-Host-Setup) সম্পন্ন করো।

---

## 🌐 Google Cloud Console সেটআপ

### ✅ ধাপ ১ — Google Cloud Console এ যাও

🔗 [console.cloud.google.com](http://console.cloud.google.com/) ভিজিট করো।
Free trial এর জন্য 🔗 [Google Docs](https://docs.cloud.google.com/) দেখো — **৯০ দিনের ফ্রি ট্রায়াল** পাবে।

---

### ✅ ধাপ ২ — APIs & Services এ ক্লিক করো

![APIs & Services](https://imgur.com/gUEX1Ob.png)

---

## 📋 Google Sheets API Enable করো

### ✅ ধাপ ৩ — Enable APIs & Services এ ক্লিক করো

![Enable APIs & Services](https://imgur.com/SssMr3V.png)

### ✅ ধাপ ৪ — "Google Sheets API" সার্চ করো

![Search Google Sheets API](https://imgur.com/P9WRsJ1.png)

### ✅ ধাপ ৫ — Google Sheets API তে ক্লিক করো

![Google Sheets API](https://imgur.com/DpwSyLB.png)

### ✅ ধাপ ৬ — Enable বাটনে ক্লিক করো

![Enable Button](https://imgur.com/LLOFdzP.png)

---

## 📄 Google Docs API Enable করো

### ✅ ধাপ ৭ — আবার Enable APIs & Services এ ক্লিক করো

![Enable APIs & Services](https://imgur.com/SssMr3V.png)

### ✅ ধাপ ৮ — "Google Docs API" সার্চ করো

![Search Google Docs API](https://imgur.com/257WFEw.png)

### ✅ ধাপ ৯ — Google Docs API তে ক্লিক করো

![Google Docs API](https://imgur.com/B5pOzhl.png)

### ✅ ধাপ ১০ — Enable বাটনে ক্লিক করো

![Enable Button](https://imgur.com/N94awNV.png)

---

## ⚙️ n8n Workflow সেটআপ

### ✅ ধাপ ১১ — Create Workflow এ ক্লিক করো

![Create Workflow](https://imgur.com/9h61ou5.png)

### ✅ ধাপ ১২ — "Google Sheets" সার্চ করো

![Search Google Sheets](https://imgur.com/kOSEJ6l.png)

### ✅ ধাপ ১৩ — "Create Spreadsheet" সিলেক্ট করো

![Create Spreadsheet](https://imgur.com/qTNY7kl.png)

---

## 🔒 OAuth Consent Screen সেটআপ

### ✅ ধাপ ১৪ — OAuth Consent Screen এ ক্লিক করো

![OAuth Consent Screen](https://imgur.com/N2En5qT.png)

### ✅ ধাপ ১৫ — Get Started বাটনে ক্লিক করো

![Get Started](https://imgur.com/gB402yk.png)

### ✅ ধাপ ১৬ — App Information দাও

![App Information](https://imgur.com/brYzXoD.png)

### ✅ ধাপ ১৭ — বাকি সেটিংস পূরণ করো

নিচের ধাপগুলো অনুসরণ করো:
- **External** সিলেক্ট করো
- নিজের **Email** দাও
- **Continue** সিলেক্ট করো
- **Create** বাটনে ক্লিক করো

![External Select](https://imgur.com/dvFrrb5.png)
![Email Input](https://imgur.com/f64KbIE.png)
![Continue & Create](https://imgur.com/1UnFUPZ.png)

---

## 🗝️ OAuth Client তৈরি করো

### ✅ ধাপ ১৮ — Create OAuth Client এ ক্লিক করো

![Create OAuth Client](https://imgur.com/cXl7aJb.png)

### ✅ ধাপ ১৯ — Application Type ও Name সেট করো

- **Application type:** Web application
- **Name:** যা আছে রাখো বা নিজের মতো দাও

![Application Type](https://imgur.com/m0UOAKD.png)

---

## 🔗 Credential সংযুক্ত করো

### ✅ ধাপ ২০ — "Set up Credential" এ ক্লিক করো

![Set up Credential](https://imgur.com/CAdIrBC.png)

### ✅ ধাপ ২১ — OAuth Redirect URL কপি করো

![Copy OAuth Redirect URL](https://imgur.com/pFd18uV.png)

### ✅ ধাপ ২২ — Authorized Redirect URLs এ Paste করো এবং Create করো

![Paste Redirect URL & Create](https://imgur.com/xMxfRsL.png)

### ✅ ধাপ ২৩ — Client ID কপি করো

![Copy Client ID](https://imgur.com/m3YFLI0.png)

### ✅ ধাপ ২৪ — Client ID Paste করো

![Paste Client ID](https://imgur.com/TwmkGgo.png)

### ✅ ধাপ ২৫ — Web Client 1 এ ক্লিক করো

![Web Client 1](https://imgur.com/EsVAArN.png)

### ✅ ধাপ ২৬ — নিচে Scroll করে Client Secret কপি করো

![Copy Client Secret](https://imgur.com/VW0w2Q8.png)

### ✅ ধাপ ২৭ — Client Secret Paste করো

![Paste Client Secret](https://imgur.com/oGfrD99.png)

---

## 🌍 App Publish করো

### ✅ ধাপ ২৮ — Audience → Publish App এ ক্লিক করো

![Publish App](https://imgur.com/gNuLtCc.png)

### ✅ ধাপ ২৯ — Confirm এ ক্লিক করো

![Confirm](https://imgur.com/k30TrvP.png)

---

## 🔑 Google Sign-In সম্পন্ন করো

### ✅ ধাপ ৩০ — "Sign in with Google" বাটনে ক্লিক করো

![Sign in with Google](https://imgur.com/oGfrD99.png)

### ✅ ধাপ ৩১ — Advanced এ ক্লিক করো

![Advanced](https://imgur.com/4OMUVPs.png)

### ✅ ধাপ ৩২ — "Go to n8n (unsafe)" এ ক্লিক করো

![Go to n8n unsafe](https://imgur.com/1wYzK1l.png)

### ✅ ধাপ ৩৩ — Select All করো এবং Continue তে ক্লিক করো

![Select All](https://imgur.com/86SDdLN.png)
![Continue](https://imgur.com/nrTWJEe.png)

---

## 🎉 Setup সম্পন্ন!

OAuth সেটআপ সফলভাবে সম্পন্ন হয়েছে!

![Setup Complete](https://imgur.com/0vkiiIb.png)

---

## ▶️ Workflow চালাও

### ✅ ধাপ ৩৪ — Execute Workflow এ ক্লিক করো

![Execute Workflow](https://imgur.com/uKCRh3o.png)

> ✔️ Workflow সফলভাবে চললে Google Drive এ **"Sheet 1"** নামে একটি নতুন ফাইল তৈরি হবে।

---

## 📋 Quick Reference

| ধাপ | কাজ | কোথায় |
|-----|-----|--------|
| ১–২ | Console এ প্রবেশ | Google Cloud |
| ৩–৬ | Sheets API Enable | Google Cloud |
| ৭–১০ | Docs API Enable | Google Cloud |
| ১১–১৩ | Workflow তৈরি | n8n |
| ১৪–১৭ | Consent Screen | Google Cloud |
| ১৮–২৭ | OAuth Client & Credentials | Google Cloud + n8n |
| ২৮–২৯ | App Publish | Google Cloud |
| ৩০–৩৩ | Google Sign-In | Browser |
| ৩৪ | Workflow Execute | n8n |

---

*এই গাইড অনুসরণ করলে n8n থেকে Google Sheets ও Docs সম্পূর্ণরূপে নিয়ন্ত্রণ করা যাবে।*
