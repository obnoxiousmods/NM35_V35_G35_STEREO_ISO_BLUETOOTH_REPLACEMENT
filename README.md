# NM35 / V35 / G35 Stereo ISO Harness + Bluetooth Amp Replacement

> **Vehicle:** Nissan Stagea NM35 — VQ25DET AWD Turbo  
> **Also applies to:** Infiniti G35 (V35), Nissan Skyline V35  
> **Amp used:** 9603 / XW-M521 4×50W Bluetooth Amplifier Board

A DIY guide to replacing the factory head unit with a compact Bluetooth amplifier board, using a standard 1995–2007 Nissan ISO harness for clean, reversible wiring — no cutting of factory loom required.

---

## 🧰 Parts & Links

| Part | Link / Model | Notes |
|------|-------------|-------|
| **Amp Board** — 4×50W Digital Amplifier | [Amazon.ca](https://www.amazon.ca/dp/B0D5HWQ5N4) / [Amazon (search)](https://www.amazon.com/s?k=Digital+Audio+Amplifier+Board+4+Channels+4X50W+HiFi) / [AliExpress](https://www.aliexpress.com/wholesale?SearchText=4+channel+amp+PCB+12V+50W) | Search "4 Channel Amp PCB 12V 50W", look for TDA7850 boards, XW-M521, etc. — see buying guide below |
| **ISO Harness** — Aerpro APP8SP3 (Nissan 1995–2007) | [Aerpro APP8SP3](https://aerpro.com/app8sp3) / [Amazon](https://www.amazon.com/s?k=Aerpro+APP8SP3+Nissan+ISO+harness) | The key piece — gives you labelled ISO wires |
| **Alternative ISO Harness** (generic) | [Amazon](https://www.amazon.com/s?k=Nissan+ISO+stereo+harness+1995-2007) | Search "Nissan ISO Stereo Wiring Harness 1995-2007" |
| **Bluetooth 6 USB to AUX Adapter** (optional) | [Amazon](https://www.amazon.com/s?k=bluetooth+USB+to+AUX+adapter+car) | If your amp board doesn't have built-in Bluetooth |
| **Heat Shrink / Electrical Tape** | Any auto store | For insulating all joins |
| **Spade Connectors / Ferrule Crimps** | Any auto store | For clean connections to the amp terminals |

### 🛒 What to Look for in an Amp Board

- **4 channels** — you need Front Left, Front Right, Rear Left, Rear Right.
- **At least 10W per channel**, but realistically **30–50W+** to match or beat the factory stereo. TDA7850-based boards are a solid choice.
- **AUX input at minimum** — 3.5mm jack so you can plug in a phone or Bluetooth adapter.
- **Bluetooth built-in is a bonus** — one less dongle to deal with.
- **AUX output is nice but not needed** — lets you daisy-chain a sub amp later without a line-out converter.
- **Screw-down terminals for power, ground, and speakers** — way easier to install than JST connectors or soldering to pads. Spring-loaded or phoenix-style terminals are ideal.

---

## 🔌 Wiring Guide

### ISO Harness Pinout (Nissan 1995–2007)

The Aerpro APP8SP3 (and similar generic harnesses) plugs into the factory Nissan radio connectors and breaks out to standard ISO colour codes:

| ISO Wire Colour | Function | Connect To |
|----------------|----------|------------|
| **Yellow** | 12V Constant (Battery) ✅ | Amp `B+` / `+12V` |
| **Red** | 12V ACC (Ignition Switched) ✅ | Amp `ACC` / `REM` |
| **Orange / Orange-White** | **Ground** ⚠️ (on NM35 Stagea — not illumination!) | Amp `GND` |
| **Black** | **UNKNOWN** ⚠️ | *Tape off — do not connect* |
| **Blue** | **UNKNOWN** ⚠️ | *Tape off — do not connect* |
| **White** | Front Left (+) | Amp `FL+` |
| **White / Black** | Front Left (−) | Amp `FL−` |
| **Gray** | Front Right (+) | Amp `FR+` |
| **Gray / Black** | Front Right (−) | Amp `FR−` |
| **Green** | Rear Left (+) | Amp `RL+` |
| **Green / Black** | Rear Left (−) | Amp `RL−` |
| **Purple** | Rear Right (+) | Amp `RR+` |
| **Purple / Black** | Rear Right (−) | Amp `RR−` |

> ⚠️ **NM35 Stagea anomaly:** On a normal Nissan ISO harness, Orange = Illumination and Black = Ground. On the NM35 Stagea, **Orange = Ground** and Black is something else (unknown). Blue is also unknown. **Always verify with a multimeter.**

### Amp Board Terminal Mapping (9603 / XW-M521)

The XW-M521 board typically has screw terminals or a JST connector with:

```
B+   → Yellow (12V Constant)
GND  → Orange / Orange-White (Ground — yes, really, on NM35)
ACC  → Red (Ignition / Accessory)
FL+ FL− → White / White-Black
FR+ FR− → Gray / Gray-Black
RL+ RL− → Green / Green-Black
RR+ RR− → Purple / Purple-Black
```

> ⚠️ **Double-check your specific board's silkscreen labels.** Some variants label the remote/ACC line as `REM`, `ACC`, or `EN`.
> ⚠️ **GND on the NM35 is Orange, not Black.** See pinout table above.

### Factory Harness Pinout (NM35 Stagea — 10-pin + 6-pin Connectors)

The factory radio connectors on the NM35 are a **10-pin** and a **6-pin** plug. Here's what's been confirmed so far:

#### Confirmed ✅

| Factory Wire Colour | Connector | Function | ISO Harness Equivalent |
|---------------------|-----------|----------|------------------------|
| **Yellow (thick)** | 10-pin | 12V Constant (Battery) | Yellow |
| **Light Green** | 10-pin | 12V ACC (Ignition) ⚠️ *confirm with DMM* | Red |
| **Red / Blue** | 10-pin | Ground | Orange (yes, Orange) |
| **Yellow** | 10-pin | Right Speaker pair | — |
| **Brown** | 10-pin | Right Speaker pair | — |
| **Pink** | 10-pin | Left Speaker pair | — |
| **Blue** | 10-pin | Left Speaker pair | — |

> ⚠️ The Yellow/Brown and Pink/Blue pairs are **100% speaker wires** but which is front vs rear, and which is + vs − within each pair hasn't been noted yet. Use a DMM to check continuity between pairs — **speaker pairs will have continuity**. On the ISO harness side, **the wire with the black stripe is the negative (−)**.

#### Unknown / Unconfirmed ❓

| Factory Wire Colour | Connector | Notes |
|---------------------|-----------|-------|
| **Green / White** | 10-pin | Unknown — possibly another speaker pair, possibly data/CAN |
| **Red** | 10-pin | Unknown |
| **Black** | 10-pin | Unknown |
| **Gray** | 10-pin | Unknown |

> There are roughly **2–4 wires whose purpose is currently unknown**. If you figure any of them out (especially if one of them is the climate control data line), **please open an Issue or PR!**
>
> **How to help:** Use a digital multimeter (DMM) to check continuity between the mystery wires and the corresponding pins on the ISO harness. Note down the factory colour → ISO colour mapping and submit it.

---

## 🛠️ Step-by-Step

### 1. Disconnect the Battery
Negative terminal off. Always.

### 2. Remove Factory Head Unit
- Pop the centre console trim (pry tools recommended).
- Unbolt the factory radio (4× Philips screws on NM35).
- Unplug the factory radio connectors.

### 3. Plug in the ISO Harness
The Aerpro harness clicks straight into the factory Nissan plugs — no cutting.

### 4. Wire the ISO Harness → Amp Board
Match wires as per the table above:
- **Stagger your joins** so no two bare-wire joints line up — reduces short risk.
- Use **crimp connectors**, **solder + heat shrink**, or **Wago-style lever nuts**.
- **Twist and tape is the bare minimum** — but upgrade to crimps when you can.

### 5. Insulate Every Join
- Heat shrink each individual wire join.
- Wrap bundles with cloth Tesa tape or electrical tape.
- Make sure **no bare copper is exposed anywhere**.

### 6. Mount the Amp
- The XW-M521 is compact — fits behind the dash, in the glovebox, or under the centre console.
- Use zip ties or VHB double-sided tape.
- Ensure airflow — these little Class-D / TDA7850-style boards get warm.

### 7. Reconnect Battery & Test
- Turn ignition to ACC — amp should power on (Bluetooth LED flashing).
- Pair your phone to `"BT-Audio"` or the default BT name.
- Test all four channels with balance/fader.

### 8. Tidy Up
- Bundle excess harness length with zip ties.
- Secure any loose wiring away from moving parts (gear selector, steering column, pedals).

---

## ⚠️ Editor's Note — Climate Control Issue

> **As of writing (June 2026), after installing this setup my climate control (A/C, heater controls, fan speed, vent mode) has stopped working.**
>
> I am actively diagnosing this and will post the solution here once I have it. Possible leads:
> - The factory stereo may be part of the CAN-BUS or LAN loop on JDM NM35s — removing it could break communication with the A/C amplifier.
> - Some NM35 trims have the A/C control integrated into the factory head unit or share a data line.
> - A resistor or jumper may be needed across certain pins on the factory radio connector to keep the climate bus alive.
>
> **If you've solved this — please open an Issue or PR!**

---

## � Extras

See the [`extras/`](extras/) folder for:
- Harness connected to amp board
- Factory connector pinout reference
- Amp mounting location
- Wiring close-ups
- PDFs, pinout diagrams, and reference docs

Also check out [`ALTERNATE_METHODS.md`](ALTERNATE_METHODS.md) for other ways to get audio into your NM35/V35/G35 (Yatour/GROM CD changer adapter, FM transmitter, etc.).

---

## 📝 Notes

- **Speaker impedance:** The factory NM35 speakers are likely 4Ω — most amp boards (TDA7850, etc.) are rated for 4Ω loads. Confirm before cranking the gain.
- **ISO wire with a black stripe = negative (−).** Speaker pairs have continuity — use a DMM to verify which wires are paired if you're working from the factory harness side.
- **No RCA pre-outs on most cheap amp boards** — they're speaker-level-only. If you want to add a sub later, you'll need a line-out converter or a board with AUX out.
- **FM Radio is lost** unless you add a separate tuner module. This setup is Bluetooth / AUX only.
- **Steering wheel controls are lost.** An aftermarket SWC adapter (e.g. PAC SWI-RC) could potentially be wired in if you retain a head unit with remote input — the bare amp board won't support it.
- **Missing wires:** There are still 2–4 factory wires with unknown purpose. One may be related to the climate control bus. If you identify any, please contribute!

---

## 🤝 Contributing

If you've done this mod on an NM35, V35, or G35 — especially if you've solved the climate control issue — please open a PR or drop a note in Issues.

---

## 📄 License

MIT — do whatever you want, but don't blame me if your dash catches fire. Disconnect the battery, tape your joins, and double-check your wiring.
