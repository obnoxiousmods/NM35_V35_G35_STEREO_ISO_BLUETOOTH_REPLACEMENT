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
## 📼 Option 4: Bluetooth Cassette Tape Adapter

> **Difficulty:** Trivial · **Sound Quality:** Decent · **Factory Look:** ❌ No (cable visible)

If your NM35/V35/G35 still has the factory **cassette deck** (many JDM models do), this is the second-easiest option after an FM transmitter — and it sounds better.

### How It Works

1. Insert the cassette-shaped adapter into the tape deck.
2. A thin cable comes out of the cassette and plugs into your phone's headphone jack (or a Bluetooth receiver dongle).
3. The tape deck's read head picks up the signal magnetically — no radio interference, no hiss.

### Bluetooth Version

You can buy cassette adapters with **built-in Bluetooth** (battery-powered, rechargeable via USB) — no cable to your phone at all. The cassette sits in the deck and pairs wirelessly.

| Type | Link |
|------|------|
| Wired 3.5mm cassette adapter | [Amazon](https://www.amazon.com/s?k=cassette+tape+aux+adapter) |
| Bluetooth cassette adapter (rechargeable) | [Amazon](https://www.amazon.com/s?k=bluetooth+cassette+adapter+rechargeable) |

### Pros
- Better sound than FM transmitters — no static, no frequency hunting.
- Zero install — pop it in and go.
- Cheap — $5–20.

### Cons
- Cable dangling from the tape deck (wired version).
- The cassette mechanism whirs — some adapters are louder than others.
- Tape deck must be functional — if the belt's gone, this won't work.
- Looks a bit janky.

---

## 💿 Option 5: Burning CDs

> **Difficulty:** Trivial · **Sound Quality:** Excellent · **Factory Look:** ✅ Yes

It's 2026 and this feels ridiculous, but the **CD player still works** and CD audio quality is genuinely good (16-bit / 44.1 kHz uncompressed).

### How It Works

1. Burn your music to a **CD-R** (not CD-RW — old Clarion units are picky).
2. Burn as **Audio CD** format (not MP3/data — the factory Clarion won't read MP3 CDs).
3. That's ~80 minutes / ~15–20 tracks per disc.
4. Keep a stack in the glovebox.

### Pros
- **Best possible sound quality** through the factory system — no compression, no interference.
- Zero install, zero wiring.
- Steering wheel controls work perfectly.
- Dirt cheap — blank CD-Rs cost pennies.

### Cons
- 80 minutes per disc. You'll be swapping constantly.
- No streaming, no playlists, no Bluetooth calls.
- Burning CDs in 2026 feels like using a fax machine.
- CD-RW discs usually don't work — one-time burns only.

> Honestly? Burning a few CDs as a stopgap while you figure out a permanent solution is totally valid. Don't let anyone shame you.

---

## 🔧 Option 6: Boot / Trunk Install (Amp or Bluetooth in Rear Cargo Area)

> **Difficulty:** Medium–Hard · **Sound Quality:** Excellent · **Factory Look:** ✅ Yes (hidden)

Instead of touching the dash, you can install an amplifier or Bluetooth receiver in the **rear cargo area (boot)**, tapping into existing wiring back there. There are plenty of YouTube videos and forum guides on amp installs in G35/V35 boots — the NM35 wagon has even more room to work with.

### General Approach

1. Mount a small amp or Bluetooth receiver board in the **left or right rear cargo trim pocket**.
2. Tap **12V constant** from the rear fuse box or battery (the NM35 battery is in the boot!).
3. Tap **ACC (ignition)** from the rear 12V accessory socket if equipped.
4. Run speaker wires forward, or tap into the factory speaker wiring where it passes through the rear.
5. Ground to a solid chassis point in the cargo area.

Search YouTube for: *"G35 amp install trunk"*, *"V35 amplifier boot install"*, *"Nissan Stagea audio install"*.

### NM35-Specific: Navigation AV / TV Tuner Route

Japanese-market NM35 Stageas often came with navigation and TV equipment mounted in the rear cargo area:

- A **navigation computer** (usually behind trim on the left side of the boot).
- A **TV tuner module**.
- **AV wiring** running between the dash screen and the rear modules.

The Clarion PN-2413E head unit in these cars supports AV input from the TV tuner and navigation. This means you might be able to **inject audio through the rear AV/TV tuner input** rather than messing with the CD changer or front harness.

```
Phone
  ↓ Bluetooth receiver
AV input / TV tuner input (in rear cargo area)
  ↓
Factory AV wiring
  ↓
Factory screen / head unit
  ↓
Factory audio system
```

#### Potential AV Input Sources to Tap

- **TV tuner audio input** — if your car has the TV button on the head unit.
- **Reverse camera input** — some units have an AV input for the backup camera.
- **Navigation audio input** — nav voice prompts route through the stereo.

> ⚠️ **Untested — theory only.** This path is less documented than the CD changer route, but it's worth investigating if you have the rear modules. The advantage is you don't need to pull the dash apart. The disadvantage is that JDM nav/TV systems can be deeply integrated and hard to reverse-engineer.
>
> If you've tapped the rear AV/TV input on an NM35 — **please open an Issue!**

---
## �🔀 Comparison

| Method | Cost | Sound | Install Effort | Factory Look | Steering Wheel Controls |
|--------|------|--------|---------------|--------------|------------------------|
| **XW-M521 Amp + ISO Harness** (main README) | ~$30–60 | ⭐⭐⭐⭐ | 2–4 hrs | ❌ No head unit | ❌ No |
| **Yatour / GROM CD Changer** | ~$50–150 | ⭐⭐⭐⭐⭐ | 30–60 min | ✅ Yes | ✅ Yes |
| **Bluetooth FM Transmitter** | ~$10–25 | ⭐⭐ | 30 sec | ❌ No | ❌ No |
| **Metra Double DIN Conversion** (untested) | ~$50–400+ | ⭐⭐⭐⭐⭐ | 3–6 hrs | ❌ No (aftermarket) | Depends on HU |
| **Bluetooth Cassette Adapter** | ~$5–20 | ⭐⭐⭐ | 10 sec | ❌ No (cable) | ❌ No |
| **Burning CDs** | ~$5 (spindle of CD-Rs) | ⭐⭐⭐⭐⭐ | 5 min per disc | ✅ Yes | ✅ Yes |
| **Boot / Trunk Install** | ~$30–200 | ⭐⭐⭐⭐ | 2–4 hrs | ✅ Yes (hidden) | Depends on setup |

---

## 📝 Contributing

Have you tried the Yatour or GROM on an NM35? Or found another method? Open an Issue or PR — I'll add it here with credit.
