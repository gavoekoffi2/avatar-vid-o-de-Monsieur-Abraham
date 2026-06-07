# frame.md — Design Spec

Brand spec for the 30-second vertical ad targeting Québec/Canada healthcare
professionals (médecins, dentistes, pharmaciens) about tax / wealth optimization.
Direct-response, premium, trustworthy. CTA: comment « CONSULTATION ».

## Register / Mood

Premium financial authority meeting modern direct-response. The feel of a
private wealth advisor's office — calm, expensive, confident — but with the
punch of a scroll-stopping social ad. Dark, cinematic, gold-on-navy.

- Light or dark: **Dark** (finance / premium).
- One accent hue: **gold** (money, wealth, savings). Teal is a secondary,
  used sparingly for the professional/medical nod.

## Palette

| Token          | Hex       | Use                                                        |
| -------------- | --------- | ---------------------------------------------------------- |
| `--bg`         | `#0A1A33` | Midnight navy — primary background across all scenes       |
| `--bg-deep`    | `#06101F` | Deeper navy — vignette edges, scrims, gradients toward     |
| `--surface`    | `#13294D` | Raised panels, pills, the comment-field metaphor           |
| `--fg`         | `#F4F7FB` | Primary text, near-white (cool)                            |
| `--muted`      | `#9FB3D1` | Secondary text, kickers, labels (cool blue-gray)           |
| `--gold`       | `#E8B85C` | PRIMARY ACCENT — money, key numbers, CTA, focal hits       |
| `--gold-bright`| `#F4CE84` | Gold highlight / glow peak / cursor                        |
| `--teal`       | `#46C7B8` | Secondary accent — audience tags, small structural marks   |
| `--line`       | `#274063` | Hairline rules, borders (2px+ on video)                    |

- Tint all neutrals toward navy — no dead gray.
- Accent must be VISIBLE: gold at full saturation on focal elements, 12–22%
  for atmospheric glows. No 5% ghost accents.
- Never pure `#000` / `#fff` — use `--bg-deep` / `--fg`.

## Typography

Three voices (register switching), never two sans together:

| Voice                 | Family                | Weights      | Used for                                                   |
| --------------------- | --------------------- | ------------ | ---------------------------------------------------------- |
| Statement (display)   | **Bricolage Grotesque** | 800 / 600  | Headlines, audience callout, captions, CTA headline        |
| Emphasis (serif)      | **Fraunces**          | 600 / 400 *(opsz)* | The money phrase, elegant emphasis words, premium accents |
| Data / document (mono)| **JetBrains Mono**    | 700 / 500    | The « CONSULTATION » tag, $ figures, kickers, reg. marks    |

Tension: Bricolage Grotesque (contemporary, slightly disruptive grotesque) ×
Fraunces (classic literary wealth/trust) × JetBrains Mono (the tax-form /
input-field of officialdom). Modern disruption applied to old-money discipline.

- Weight contrast extreme: 800 display vs 400–500 body. Video, not web.
- Display tracking tight: `-0.03em` to `-0.04em`.
- Dark-bg adjustments: body line-height +0.05, never below 350 weight for body.
- `tabular-nums` on every $ figure.

## Scale (vertical 1080×1920)

| Element                | Size        |
| ---------------------- | ----------- |
| Hero / title headline  | 110–150px   |
| Section headline       | 72–96px     |
| Captions               | 64–84px     |
| Body / subline         | 36–46px     |
| Kicker / label (mono)  | 24–30px     |
| Decorative opacity     | 10–22%      |
| Borders / rules        | 2–4px       |

## Motion

- Premium = controlled, weighted. Entrances 0.5–0.8s, `power3.out` / `expo.out`
  for confident arrivals; small `back.out(1.4)` only on the gold money hit.
- Vary 3+ eases per scene. Ambient: slow gold-glow breathing, a drifting
  oversized `$` ghost, a gold progress line.
- Transitions between full-screen cards (title → avatar → outro): fade + soft
  directional wipe. No jump cuts. The avatar A-roll is continuous underneath.

## Do

- Anchor content; pin the kicker top-left, money bottom-heavy.
- Gold reserved for money + action. Teal only for the three professions.
- Captions: white statements, gold on money / impôt / économiser / CONSULTATION.
- Keep the presenter's face clear — captions sit in the lower third.

## Don't

- No gradient text, no cyan-on-dark neon, no purple gradients, no left-edge
  accent stripes, no pure black/white.
- Don't pair two sans. Don't let gold drift to orange or teal to cyan.
- Don't cover the avatar's eyes/mouth with captions or graphics.
- No banned fonts (Inter, Poppins, Outfit, Sora, Playfair, Syne, …).
