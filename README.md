# 🌐 Networking Notes

> কম্পিউটার নেটওয়ার্কিং-এর সম্পূর্ণ নোট — বাংলায়, একদম গোড়া থেকে।
> OSI-র সাত স্তর ধরে ধরে, ডায়াগ্রাম ও বাস্তব উদাহরণ সহ।

---

## 🚀 কোথা থেকে শুরু করবে

**একদম নতুন হলে এই একটা নোট দিয়ে শুরু করো** — পুরো ছবিটা একবারে মাথায় বসে যাবে:

### 👉 [০. সহজে বুঝি — নেটওয়ার্ক কীভাবে কাজ করে](0.%20সহজে%20বুঝি%20-%20নেটওয়ার্ক%20কীভাবে%20কাজ%20করে.md)

তারপর নিচের নোটগুলোতে এক এক করে গভীরে যাও — **নিচের স্তর থেকে উপরে**।

---

## 🧠 মনে রাখতে চাও?

পড়া আর **মনে রাখা** এক জিনিস না। এই দুটো নোট শুধু মনে রাখার জন্যই বানানো:

| | নোট | কখন ব্যবহার করবে |
|---|---|---|
| 📋 | **[চিট শিট — এক পাতায় সব](8.%20চিট%20শিট%20-%20এক%20পাতায়%20সব.md)** | পরীক্ষা/interview-র ঠিক আগে — সব সংখ্যা ও টেবিল এক জায়গায় |
| 🎴 | **[ফ্ল্যাশকার্ড — নিজেকে যাচাই করো](9.%20ফ্ল্যাশকার্ড%20-%20নিজেকে%20যাচাই%20করো.md)** | প্রতিদিন ১০ মিনিট — ৪৫টা প্রশ্নে নিজেকে পরীক্ষা করো |

> 💡 **গবেষণা বলে** — বারবার পড়ার চেয়ে **নিজেকে প্রশ্ন করা** কয়েকগুণ বেশি কার্যকর।
> তাই আগে ফ্ল্যাশকার্ড খুলে উত্তর দেওয়ার চেষ্টা করো, তারপর যেটা পারোনি সেই নোটটা পড়ো।

---

## 📚 সব নোট

| # | নোট | কী আছে |
|---|---|---|
| **০** | [সহজে বুঝি — নেটওয়ার্ক কীভাবে কাজ করে](0.%20সহজে%20বুঝি%20-%20নেটওয়ার্ক%20কীভাবে%20কাজ%20করে.md) | চিঠির উপমা · সাত স্তর · চারটা ঠিকানা · encapsulation · YouTube খোলার পুরো যাত্রা |
| **১** | [Layer 1 — Physical Layer](1.%20Layer%201%20-%20Physical%20Layer.md) | সংকেত · twisted pair · ফাইবার · Wi-Fi ব্যান্ড · bandwidth vs latency · duplex · troubleshooting |
| **২** | [Layer 2 — Data Link Layer](2.%20Layer%202%20-%20Data%20Link%20Layer.md) | MAC address · Ethernet frame · সুইচ কীভাবে শেখে · error detection · flow control · VLAN |
| **৩** | [Layer 3 — Network Layer](3.%20Layer%203%20-%20Network%20Layer.md) | IP address · class · subnet mask · CIDR · subnetting · IPv6 · NAT · routing · ARP · fragmentation |
| **৪** | [Layer 4 — Transport Layer](4.%20Layer%204%20-%20Transport%20Layer.md) | TCP three-way handshake · flow control · congestion control · UDP · port number |
| **৫** | [Layer 5-6-7 — Application Layer](5.%20Layer%205-6-7%20-%20Application%20Layer.md) | HTTP · DNS · FTP · SMTP · encryption · compression · session management |
| **৬** | [OSI Model — সম্পূর্ণ চিত্র](6.%20OSI%20Model%20-%20সম্পূর্ণ%20চিত্র.md) | সাত স্তর একসাথে · Hub/Switch/Router/Firewall · routing · VLAN · LAN/WAN/MAN · topology |
| **৭** | [DHCP, DNS ও ব্যবহারিক IP](7.%20DHCP,%20DNS%20ও%20ব্যবহারিক%20IP.md) | DHCP · DNS · NAT · port · static vs dynamic IP · VPN · troubleshooting |
| **৮** | 📋 [চিট শিট — এক পাতায় সব](8.%20চিট%20শিট%20-%20এক%20পাতায়%20সব.md) | **মুখস্থ রাখার সব কিছু** — mnemonic · IP class · subnet টেবিল · port · header আকার · ২০টা জরুরি সংখ্যা |
| **৯** | 🎴 [ফ্ল্যাশকার্ড — নিজেকে যাচাই করো](9.%20ফ্ল্যাশকার্ড%20-%20নিজেকে%20যাচাই%20করো.md) | **৪৫টা প্রশ্ন**, উত্তর লুকানো — নিজেকে পরীক্ষা করে মনে রাখো |

---

## 🗺️ কোন স্তরে কী

```
┌─────────────────────────────────────────────────────────────┐
│ ৭  Application   │ HTTP, DNS, FTP, SMTP        →  নোট ৫     │
│ ৬  Presentation  │ TLS, encryption, JPEG       →  নোট ৫     │
│ ৫  Session       │ login session, RPC          →  নোট ৫     │
├─────────────────────────────────────────────────────────────┤
│ ৪  Transport     │ TCP, UDP, port              →  নোট ৪     │
├─────────────────────────────────────────────────────────────┤
│ ৩  Network       │ IP, routing, NAT, ARP       →  নোট ৩     │
├─────────────────────────────────────────────────────────────┤
│ ২  Data Link     │ MAC, Ethernet, switch       →  নোট ২     │
├─────────────────────────────────────────────────────────────┤
│ ১  Physical      │ cable, fiber, Wi-Fi         →  নোট ১     │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎯 বিষয় ধরে খুঁজছো?

| খুঁজছো | কোথায় পাবে |
|---|---|
| IP address, subnetting, CIDR | [নোট ৩](3.%20Layer%203%20-%20Network%20Layer.md) |
| MAC address, সুইচ কীভাবে কাজ করে | [নোট ২](2.%20Layer%202%20-%20Data%20Link%20Layer.md) |
| TCP handshake, port number | [নোট ৪](4.%20Layer%204%20-%20Transport%20Layer.md) |
| DNS কীভাবে কাজ করে | [নোট ৫](5.%20Layer%205-6-7%20-%20Application%20Layer.md) · [নোট ৭](7.%20DHCP,%20DNS%20ও%20ব্যবহারিক%20IP.md) |
| NAT, private vs public IP | [নোট ৩](3.%20Layer%203%20-%20Network%20Layer.md) · [নোট ৭](7.%20DHCP,%20DNS%20ও%20ব্যবহারিক%20IP.md) |
| Router vs Switch vs Hub | [নোট ৬](6.%20OSI%20Model%20-%20সম্পূর্ণ%20চিত্র.md) |
| VLAN | [নোট ২](2.%20Layer%202%20-%20Data%20Link%20Layer.md) · [নোট ৬](6.%20OSI%20Model%20-%20সম্পূর্ণ%20চিত্র.md) |
| DHCP | [নোট ৭](7.%20DHCP,%20DNS%20ও%20ব্যবহারিক%20IP.md) |
| ইন্টারনেট কাজ করছে না | [নোট ৭](7.%20DHCP,%20DNS%20ও%20ব্যবহারিক%20IP.md) · [নোট ১](1.%20Layer%201%20-%20Physical%20Layer.md) |
| VPN, নিরাপত্তা | [নোট ৭](7.%20DHCP,%20DNS%20ও%20ব্যবহারিক%20IP.md) |

---

## 📖 পড়ার ক্রম

**একদম নতুন:** ০ → ৬ → ১ → ২ → ৩ → ৪ → ৫ → ৭

**কিছু জানা আছে:** ০ → যে স্তরটা দুর্বল, শুধু সেটা

**Interview-এর আগে:** ৮ (চিট শিট) → ৯ (ফ্ল্যাশকার্ড) → যেগুলো ভুল হলো শুধু সেই নোট

**পরীক্ষার আগের রাতে:** শুধু ৮ নম্বর — ২০ মিনিটে পুরো revision

---

## 🔗 সম্পর্কিত

নেটওয়ার্কিং-এর উপরে যে system design-এর স্তরগুলো বসে, সেগুলো পাশের ফোল্ডারে:

- [System-Design-Notes](../System-Design-Notes/) — Load balancer, CDN, caching, database scaling, microservices
- বিশেষ করে: [HTTP Versions](../System-Design-Notes/2.%20HTTP%20Versions%20-%20Complete%20Details.md) · [Browser-এ URL লিখলে কী হয়](../System-Design-Notes/A1.What%20Happens%20When%20You%20Type%20%60www.google.com%60%20in%20a%20Browser%3F.md)
