<div align="center">

# FromScratch

**Bot smarter, not harder.**

---

```
  ______                    _____                 _       _     
 |  ____|                  / ____|               | |     | |    
 | |__ _ __ ___  _ __ ___ | (___   ___ _ __ __ _| |_ ___| |__  
 |  __| '__/ _ \| '_ ` _ \ \___ \ / __| '__/ _` | __/ __| '_ \ 
 | |  | | | (_) | | | | | |____) | (__| | | (_| | || (__| | | |
 |_|  |_|  \___/|_| |_| |_|_____/ \___|_|  \__,_|\__\___|_| |_|
```

</div>

## What's here?

This repo hosts shared runtime resources used by **FromScratch** scripts on the [DreamBot SDN](https://dreambot.org).

| File | Purpose |
|------|---------|
| `mousedata.json` | Pre-recorded human mouse movement dataset for the SmartMouse algorithm |

## SmartMouse

Our scripts use a custom mouse algorithm trained on real human input data — not random bezier curves, not simple wind physics. Thousands of recorded movements across every distance and direction, replayed with natural variance.

**How it works:**
- On first script launch, `mousedata.json` is downloaded and cached locally
- Subsequent runs load instantly from disk
- Each movement picks a real recorded path matching the distance + direction, then applies subtle per-step timing variance
- Falls back to a randomized physics model if the download fails

No two mouse paths are ever identical. Because yours aren't either.

## Scripts

Find our scripts on the [DreamBot SDN](https://sdn.dreambot.org/scripts) — search for **FromScratch**.

---

<div align="center">
<sub>Built with caffeine and questionable life choices.</sub>
</div>
