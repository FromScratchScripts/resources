<div align="center">

# FromScratch

```
  ______                    _____                 _       _     
 |  ____|                  / ____|               | |     | |    
 | |__ _ __ ___  _ __ ___ | (___   ___ _ __ __ _| |_ ___| |__  
 |  __| '__/ _ \| '_ ` _ \ \___ \ / __| '__/ _` | __/ __| '_ \ 
 | |  | | | (_) | | | | | |____) | (__| | | (_| | || (__| | | |
 |_|  |_|  \___/|_| |_| |_|_____/ \___|_|  \__,_|\__\___|_| |_|
```

**Bot smarter, not harder.**

</div>

---

Hey, I'm the dev behind FromScratch. I build scripts for the [DreamBot SDN](https://sdn.dreambot.org/scripts) that focus on doing things right — clean movement, smart progression, and not cutting corners on the stuff that matters.

## What's in this repo

Shared resources that my scripts download at runtime.

| File | What it does |
|------|-------------|
| `mousedata.json` | Mouse movement dataset for the SmartMouse algorithm |
| `media/` | Icons and banners |

## SmartMouse

I got tired of scripts that move the mouse like a robot. SmartMouse replays real recorded human mouse movements instead of generating them with math. Every path in the dataset came from actual hand movements, captured with per-step timing.

**How it works:**
- First time you run a script, it downloads `mousedata.json` and caches it locally
- Every mouse movement picks a real recorded path that matches the distance and direction
- V2 paths replay the exact timing from the recording, V1 paths use easing as a fallback
- No two movements are identical

## Scripts

Find my scripts on the [DreamBot SDN](https://sdn.dreambot.org/scripts) — search **FromScratch**.

---

<div align="center">
<sub>Built with caffeine and questionable life choices.</sub>
</div>
