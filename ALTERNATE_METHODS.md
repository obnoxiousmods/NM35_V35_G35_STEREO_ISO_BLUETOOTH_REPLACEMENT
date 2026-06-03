# Alternate Methods — Audio in NM35 / V35 / G35

If you don't want to rip out the factory head unit and wire in a bare amp board, here are other ways to get Bluetooth/AUX audio into these cars.

---

## 🎵 Option 1: Yatour or GROM CD Changer Emulator

> **Difficulty:** Medium · **Sound Quality:** Excellent · **Factory Look:** ✅ Yes

These devices plug into the **CD changer port** on the back of the factory Nissan head unit and emulate a CD changer, tricking the stereo into playing audio from Bluetooth, USB, or AUX.

### Compatible Devices

| Device | Link | Notes |
|--------|------|-------|
| **Yatour YT-M06 / YT-USB** | [Amazon](https://www.amazon.com/s?k=Yatour+Nissan+Bluetooth+adapter) / [eBay](https://www.ebay.com/sch/i.html?_nkw=Yatour+Nissan+Bluetooth) | Most common — supports Bluetooth, USB, SD card, AUX |
| **GROM Audio NIS02** | [GROM Audio](https://gromaudio.com/store/all-nis02.html) | Higher-end — Bluetooth + USB, better DAC |
| **GROM USB2P** | [GROM Audio](https://gromaudio.com/store/usb_adapters/) | USB + AUX only, no Bluetooth |

### How It Works

1. The Yatour/GROM box plugs into the **CD changer / SAT port** on the back of the factory radio.
2. The factory head unit thinks a CD changer is connected — you switch to "CD" or "CHG" or "SAT" mode.
3. Audio plays through the factory amp and speakers with zero wiring to the speaker harness.

### Nissan Wiring Notes

- The CD changer port on the NM35 / V35 / G35 Clarion head unit is typically a **12-pin or 13-pin round DIN** or a **rectangular multi-pin** connector — the Yatour/GROM kit includes the correct adapter cable for your specific radio.
- Some Nissan models use the **SAT** button (satellite) instead of **CHG** (changer) — the adapter works on either; just press the corresponding source button.
- **Steering wheel controls usually still work** for volume and track skip via the adapter.

### ⚠️ Untested on NM35

> **I have not personally tested this on the NM35 Stagea.** In theory it should work — NM35s use a Clarion head unit that shares the CD changer protocol with other 2000s Nissans (350Z, G35, Maxima). However, JDM NM35s may have a different firmware or a locked-out changer port.
>
> If you try it — please open an Issue with your results!

### Where to Buy

- **Yatour:** Search "Yatour Nissan Bluetooth" on Amazon, eBay, AliExpress — ~$50–80 USD
- **GROM:** [gromaudio.com](https://gromaudio.com) — ~$100–150 USD (better support, firmware updates)

---

## 📻 Option 2: Bluetooth FM Transmitter

> **Difficulty:** Trivial · **Sound Quality:** Low–Mediocre · **Factory Look:** ❌ No

### How It Works

A Bluetooth FM transmitter plugs into your **cigarette lighter / 12V socket** and broadcasts your phone's audio over an unused FM frequency. You tune the factory radio to that frequency, and the audio plays through the car speakers.

### Pros
- **Zero install.** Plug it in, pair your phone, set the FM station. Done in 30 seconds.
- **Works in any car** with an FM radio and a 12V socket.
- **Cheap** — $10–25 on Amazon.

### Cons
- **Sound quality is bad.** FM radio bandwidth is limited — expect compressed, tinny audio with background hiss. Noticeably worse than a direct AUX or Bluetooth connection.
- **Interference.** Driving through cities means constantly finding a clear frequency. What's clear in one suburb is static in the next.
- **Clutter.** A dongle hanging out of your 12V socket with a cable.
- **Volume mismatch.** You have to crank the head unit volume higher than normal, which amplifies the hiss.

### Recommended Units

| Device | Link |
|--------|------|
| Anker Roav F0 / F2 | [Amazon](https://www.amazon.com/s?k=Anker+Roav+Bluetooth+FM+transmitter) |
| Nulaxy KM18 / KM29 | [Amazon](https://www.amazon.com/s?k=Nulaxy+Bluetooth+FM+transmitter) |
| LIHAN USB-C FM Transmitter | [Amazon](https://www.amazon.com/s?k=LIHAN+Bluetooth+FM+transmitter) |

### When to Use This

- You don't care about audio quality and just want *something*.
- You're in a rural area with lots of empty FM frequencies.
- You're selling the car soon and don't want to invest time/money.
- You want a temporary solution while you figure out the permanent one.

---

## �️ Option 3: Metra Double DIN Conversion Kit

> **Difficulty:** Hard · **Sound Quality:** Depends on head unit · **Factory Look:** ❌ No (aftermarket)

If you want a **modern double-DIN head unit** (CarPlay, Android Auto, etc.), the Metra dash kit for the Infiniti G35 **may** fit the NM35 Stagea — but it hasn't been confirmed.

### The Kit

| Part | Model | Link |
|------|-------|------|
| **Metra Dash Kit** | 99-7605 (or 95-7605) | [Metra Online](https://metraonline.com) / [Amazon](https://www.amazon.com/s?k=Metra+99-7605+dash+kit) |
| **Metra Wiring Harness** | 70-7551 | [Amazon](https://www.amazon.com/s?k=Metra+70-7551+Nissan+harness) |
| **Antenna Adapter** | 40-NI10 | [Amazon](https://www.amazon.com/s?k=Metra+40-NI10+antenna+adapter) |

> 📄 The Metra 95-7605 installation PDF is included in the [`extras/`](extras/) folder for reference.

### ⚠️ NM35 Fitment — UNTESTED

> **I have NOT tried this on the NM35 Stagea.** The G35 (V35) interior is almost identical — same dash shape, same radio opening, similar trim clips. However:
>
> - The JDM NM35 may have **different mounting brackets or screw points** behind the trim.
> - The **climate control integration** issue (noted in the main README) still applies — removing the factory radio may break the A/C controls regardless of what you replace it with.
> - The Metra kit includes brackets and a trim bezel designed for **LHD USDM G35s** — RHD JDM Stagea fitment is unverified.
>
> **If you've installed a double-DIN in an NM35 — please open an Issue with photos!**

### What You'd Need

1. **Metra 99-7605 (or 95-7605)** dash kit — includes the plastic bezel and mounting brackets.
2. **Metra 70-7551** wiring harness — adapts factory Nissan plugs to standard ISO/aftermarket colours.
3. **Any double-DIN head unit** — Pioneer, Sony, Kenwood, Alpine, or an Android Auto / CarPlay unit.
4. **A solution for the climate control** (once discovered — see main README editor's note).

### Why Go Double DIN?

- Full CarPlay / Android Auto with a big touchscreen.
- Proper EQ, time alignment, crossovers — actual tuning.
- RCA pre-outs for subwoofers and external amps.
- DAB+ digital radio, hands-free calling, reverse camera input.

---

## �🔀 Comparison

| Method | Cost | Sound | Install Effort | Factory Look | Steering Wheel Controls |
|--------|------|--------|---------------|--------------|------------------------|
| **XW-M521 Amp + ISO Harness** (main README) | ~$30–60 | ⭐⭐⭐⭐ | 2–4 hrs | ❌ No head unit | ❌ No |
| **Yatour / GROM CD Changer** | ~$50–150 | ⭐⭐⭐⭐⭐ | 30–60 min | ✅ Yes | ✅ Yes |
| **Bluetooth FM Transmitter** | ~$10–25 | ⭐⭐ | 30 sec | ❌ No | ❌ No |
| **Metra Double DIN Conversion** (untested) | ~$50–400+ | ⭐⭐⭐⭐⭐ | 3–6 hrs | ❌ No (aftermarket) | Depends on HU |
| **Cassette Tape Adapter** (if equipped) | ~$5–10 | ⭐⭐⭐ | 10 sec | ❌ No | ❌ No |

---

## 📝 Contributing

Have you tried the Yatour or GROM on an NM35? Or found another method? Open an Issue or PR — I'll add it here with credit.
