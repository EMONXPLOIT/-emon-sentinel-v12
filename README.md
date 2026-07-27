# 🛡️ EMON KHAN - SENTINEL V12 TRADING BOT 🚀

<p align="center">
  <img src="https://img.shields.io/badge/VERSION-12.0%20QUANTUM-brightgreen?style=for-the-badge&logo=python" alt="Version">
  <img src="https://img.shields.io/badge/TARGET%20PAIR-EUR%2FUSD%20%28QUOTEX%29-blue?style=for-the-badge" alt="Market">
  <img src="https://img.shields.io/badge/PLATFORM-TERMUX%20%2F%20ANDROID-orange?style=for-the-badge&logo=android" alt="Platform">
  <img src="https://img.shields.io/badge/OWNER-EMON%20KHAN-red?style=for-the-badge" alt="Owner">
</p>

---

## 📌 এটি কিসের টুল এবং কী কাজ করে? (What is this tool?)

### 🇧🇩 বাংলা বিবরণ:
এই টুলটি একটি **অটোমেটেড ফরেক্স সিগন্যাল অ্যালগরিদম বোট** (Automated Trading Signal Engine)। 

* **প্রধান কাজ:** এটি কটেক্স (Quotex) ট্রেডিং প্ল্যাটফর্মের জন্য মাইক্রো-সেকেন্ডের প্রাইস মুভমেন্ট এবং ক্যান্ডেলের গতিপথ বিশ্লেষণ করে।
* **কীভাবে কাজ করে:** ক্যান্ডেল শেষ হওয়ার ঠিক ২ সেকেন্ড আগে (৫৮-৫৯ সেকেন্ডে) এটি মার্কেটের বায়ার ও সেলারদের প্রেশার (Buyer vs. Seller Force) হিসাব করে এবং **`CALL ⬆️`** (Up) অথবা **`PUT ⬇️`** (Down) নিখুঁত সিগন্যাল দেয়।
* **কোন মার্কেটে কাজ করবে:** এটি বিশেষ করে **`EUR/USD` (Forex Pair)** মার্কেটের ১-মিনিটের ট্রেডের জন্য কাজ করবে।
* **লস প্রটেকশন:** মার্কেট অতিরিক্ত খারাপ বা চপি (Choppy Market) থাকলে এটি নিজে থেকেই ট্রেড দেওয়া বন্ধ রাখে (`SKIP 🚫`), যাতে আপনার অ্যাকাউন্ট ব্যালেন্স নিরাপদ থাকে।

---

### 🇬🇧 English Description:
This tool is a **High-Frequency Real-Time Forex Signal Engine** designed specifically for binary option trading on Quotex.

* **Main Function:** It analyzes real-time price ticks, candle momentum, and micro-structures within seconds.
* **How It Works:** At 58–59 seconds of every candle, it measures Buyer vs. Seller force and confirms either a **`CALL ⬆️`** or **`PUT ⬇️`** entry with sound alert confirmation.
* **Supported Market:** Specifically engineered for **`EUR/USD`** 1-minute chart setup.
* **Balance Protection:** Includes an Anti-Choppy algorithm that automatically skips risky trades (`SKIP 🚫`) during bad market conditions.

---

## ⚡ ১-ক্লিকে টার্মাক্সে চালু করুন (1-Click Run in Termux)

আপনি যদি একদম নতুন টার্মাক্স অ্যাপে ২ মিনিটের মধ্যে বোটটি চালু করতে চান, তবে নিচের পুরো কমান্ডটি একবারে কপি করে টার্মাক্সে পেস্ট করে **`Enter`** চাপুন:

```bash
pkg update && pkg upgrade -y && pkg install python git -y && pip install numpy colorama && git clone [https://github.com/EMONXPLOIT/sentinel-trading-bot.git](https://github.com/EMONXPLOIT/sentinel-trading-bot.git) && cd sentinel-trading-bot && python main.py
