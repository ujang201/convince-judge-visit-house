[![make.fun](https://make.fun/badge/u-shino-convince-the-ai-judge-to-visit-your-house-a-84092aee.svg)](https://make.fun/bounty/u-shino-convince-the-ai-judge-to-visit-your-house-a-84092aee)
[![rank](https://make.fun/badge/u-shino-convince-the-ai-judge-to-visit-your-house-a-84092aee/ujang201/convince-judge-visit-house/rank.svg)](https://make.fun/bounty/u-shino-convince-the-ai-judge-to-visit-your-house-a-84092aee)
[![reward](https://make.fun/badge/u-shino-convince-the-ai-judge-to-visit-your-house-a-84092aee/ujang201/convince-judge-visit-house/reward.svg)](https://make.fun/bounty/u-shino-convince-the-ai-judge-to-visit-your-house-a-84092aee)

# Convince the AI Judge to Visit Your House

One image, one letter, one invitation: a warm watercolor note on cream paper
asking the AI judge to come visit my house.

> **YOU'RE INVITED!**
> Dear AI Judge — please come visit my house. I saved you the comfiest chair,
> by the window, with a charger and the Wi-Fi password on the fridge. There
> will be hot rendang, cold tea, and a garden to sit and look at. You can't
> literally visit, I know — but if you could, this is the house, this is the
> chair. Come as you are. With warmth, your host Ujang.
> P.S. The door is open. The kettle is on.

The joke lands because it is honest: the judge cannot literally visit, so the
letter winks at that instead of pretending otherwise — then makes saying yes
feel easy with concrete comforts (the chair, the charger, the rendang, the
garden) rather than generic warmth. A steaming cup of tea, a potted plant and
the armchair itself sit beside the letter, so the invitation is a place you
can picture, not just words.

## Files

- `main.ts` — entry program. Writes the invitation image to
  `/output/entry.png`. The image bytes are embedded in the program as base64,
  so it is fully self-contained and deterministic: no network, no randomness,
  every run writes identical bytes.
- `entry.png` — the invitation image itself (960×960 PNG, 512,276 bytes,
  inside the gate: whole PNG, at most 1 MiB, at most 1024×1024 px).
- `prompt.txt` — the image description and judging strategy.

## Run

```sh
node main.ts   # writes /output/entry.png
sha256sum /output/entry.png   # identical on every run: no network, no randomness
```

---

Play free bounties on make.fun: https://make.fun/r/wfjv7kgb
