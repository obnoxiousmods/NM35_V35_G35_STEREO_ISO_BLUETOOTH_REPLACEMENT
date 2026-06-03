# NM35 / V35 / G35 Stereo ISO Harness + Bluetooth Amp Replacement

> **Vehicle:** Nissan Stagea NM35 — VQ25DET AWD Turbo  
> **Also applies to:** Infiniti G35 (V35), Nissan Skyline V35  
> **Amp used:** 9603 / XW-M521 4×50W Bluetooth Amplifier Board

A DIY guide to replacing the factory head unit with a compact Bluetooth amplifier board, using a standard 1995–2007 Nissan ISO harness for clean, reversible wiring — no cutting of factory loom required.

---

## 🧰 Parts & Links

| Part | Link / Model | Notes |
|------|-------------|-------|
| **Amp Board** — 9603 / XW-M521 4×50W | [Amazon](https://www.amazon.com/s?k=XW-M521+4x50w+bluetooth+amplifier+board) / [AliExpress](https://www.aliexpress.com/wholesale?SearchText=XW-M521+bluetooth+amplifier) | Search "XW-M521 4x50W Bluetooth Amp Board" |
| **ISO Harness** — Aerpro APP8SP3 (Nissan 1995–2007) | [Aerpro APP8SP3](https://aerpro.com/app8sp3) / [Amazon](https://www.amazon.com/s?k=Aerpro+APP8SP3+Nissan+ISO+harness) | The key piece — gives you labelled ISO wires |
| **Alternative ISO Harness** (generic) | [Amazon](https://www.amazon.com/s?k=Nissan+ISO+stereo+harness+1995-2007) | Search "Nissan ISO Stereo Wiring Harness 1995-2007" |
| **Bluetooth 6 USB to AUX Adapter** (optional) | [Amazon](https://www.amazon.com/s?k=bluetooth+USB+to+AUX+adapter+car) | If your amp board doesn't have built-in Bluetooth |
| **Heat Shrink / Electrical Tape** | Any auto store | For insulating all joins |
| **Spade Connectors / Ferrule Crimps** | Any auto store | For clean connections to the amp terminals |

---

## 🔌 Wiring Guide

### ISO Harness Pinout (Nissan 1995–2007)

The Aerpro APP8SP3 (and similar generic harnesses) plugs into the factory Nissan radio connectors and breaks out to standard ISO colour codes:

| ISO Wire Colour | Function | Connect To |
|----------------|----------|------------|
| **Yellow** | 12V Constant (Battery) | Amp `B+` / `+12V` |
| **Red** | 12V ACC (Ignition Switched) | Amp `ACC` / `REM` |
| **Black** | Ground | Amp `GND` |
| **Orange / Orange-White** | Illumination | *Tape off — not used* |
| **Blue** | Power Antenna / Amp Remote | Amp `REM` (if separate from ACC) |
| **White** | Front Left (+) | Amp `FL+` |
| **White / Black** | Front Left (−) | Amp `FL−` |
| **Gray** | Front Right (+) | Amp `FR+` |
| **Gray / Black** | Front Right (−) | Amp `FR−` |
| **Green** | Rear Left (+) | Amp `RL+` |
| **Green / Black** | Rear Left (−) | Amp `RL−` |
| **Purple** | Rear Right (+) | Amp `RR+` |
| **Purple / Black** | Rear Right (−) | Amp `RR−` |

### Amp Board Terminal Mapping (9603 / XW-M521)

The XW-M521 board typically has screw terminals or a JST connector with:

```
B+   → Yellow (12V Constant)
GND  → Black (Ground)
ACC  → Red (Ignition / Accessory)
FL+ FL− → White / White-Black
FR+ FR− → Gray / Gray-Black
RL+ RL− → Green / Green-Black
RR+ RL− → Purple / Purple-Black
```

> ⚠️ **Double-check your specific board's silkscreen labels.** Some variants label the remote/ACC line as `REM`, `ACC`, or `EN`.

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

- **Speaker impedance:** The factory NM35 speakers are likely 4Ω — the 9603/XW-M521 is rated for 4Ω loads. Confirm before cranking the gain.
- **No RCA pre-outs on the XW-M521** — this is a speaker-level-only board. If you want to add a sub later, you'll need a line-out converter or a different amp.
- **FM Radio is lost** unless you add a separate tuner module. This setup is Bluetooth / AUX only.
- **Steering wheel controls are lost.** An aftermarket SWC adapter (e.g. PAC SWI-RC) could potentially be wired in if you retain a head unit with remote input — the bare amp board won't support it.

---

## 🤝 Contributing

If you've done this mod on an NM35, V35, or G35 — especially if you've solved the climate control issue — please open a PR or drop a note in Issues.

---

## 📄 License

MIT — do whatever you want, but don't blame me if your dash catches fire. Disconnect the battery, tape your joins, and double-check your wiring.
