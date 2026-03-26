# Custom Nav Banner — Shopify Section

Hero banner section for bundle landing pages. Fully configurable via the Shopify Theme Editor.

---

## Approach

The goal was to build a custom Shopify banner section for a bundle page A/B test using Intelligems.

- A `custom-banner.liquid` section was created with full Theme Editor controls — heading, CTA, images, overlay — so the client can manage content without touching code.
- The section is included in the **Control URL** of the Intelligems test, while the Variation runs the same bundle pack without it — keeping the test clean and isolated.
- **Add to Cart Rate** and **Revenue Per Session** are tracked as metrics to measure whether the banner drives more conversions.
- Responsive fixes ensure the layout works across all screen sizes, with a dedicated mobile image.
- All changes (alt tags, CTA, responsive fixes) were made directly in the section file to keep the codebase minimal and easy to maintain.

---

## Files
- `custom-banner.liquid` — Section markup, styles, and schema
- `custom_nav_banner.liquid` — Custom navigation bar section

#URL Targeting Rules Followed( Only worked Product Page ):

Include: /products/*
Exclude: Homepage (/), Collection pages (/collections/*)

---

## Theme Editor Settings
- **Content:** Heading, highlighted text, subtext, highlight color
- **CTA Button:** Button text, link, background, text color, hover color
- **Images:** Desktop image, mobile image, background images, logo
- **Overlay:** Overlay color and opacity (0–100)
- **Navigation:** Menu link list

---

## Task Status

| Task | Status |
|---|---|
| Alt attributes on all images | ✅ Done |
| README added to GitHub | ✅ Done |
| Figma reference: [Live Preview](https://ankush-kumar-digital-design.myshopify.com/products/herbal-daily-multivitamin-with-natural-plant-extracts-minerals) | 🔗 |
| Intelligems primary & secondary metrics configured | ✅ Done |
| Target page set to Product Page (PDP) | ✅ Done |
| A/B test: Control vs Variation (both bundle packs; this section in Control URL) | ✅ Done |

---

## Intelligems A/B Test

| | Details |
|---|---|
| **Test ID** | `1fcbb94a-5c30-49de-b06f-16eb3c0de911` |
| **Variation  ID** | `53e3b4ce-895f-4ade-94af-9eecd626d61c` |
| **Control ID** | `411bd667-4291-4792-80ca-ed88dc76f02b` |
| **Primary Metric** | Add to Cart Rate |
| **Secondary Metric** | Revenue Per Session |

**Preview URLs**

- Control: `https://ankush-kumar-digital-design.myshopify.com/products/herbal-daily-multivitamin-with-natural-plant-extracts-minerals/?ig-preview=1fcbb94a-5c30-49de-b06f-16eb3c0de911&igTg=411bd667-4291-4792-80ca-ed88dc76f02b&preview_theme_id=157371990147&pb=0`

- Variation: `https://ankush-kumar-digital-design.myshopify.com/products/herbal-daily-multivitamin-with-natural-plant-extracts-minerals/?ig-preview=1fcbb94a-5c30-49de-b06f-16eb3c0de911&igTg=53e3b4ce-895f-4ade-94af-9eecd626d61c&preview_theme_id=157371990147&pb=0`

**Integration Keys**
- Variation: `9eecd626d61c`
- Control: `ed88dc76f02b`
| Responsive layout errors fixed | ✅ Done |
| CTA button and link added | ✅ Done |

> Client confirmed: stock PDP in use.

---



### Folder Structure
```
/
├── sections/
│   ├── custom-banner.liquid
│   └── custom_nav_banner.liquid
└── README.md
```

### Setup Steps
1. Clone the repository
2. Upload `custom-banner.liquid` and `custom_navbar.liquid` to your Shopify theme under `sections/`
3. In the Theme Editor, add **Bundle Banner Section** to the desired template
4. Configure all settings (images, CTA, overlay) via the Theme Editor
5. Use the Intelligems preview URLs to verify Control and Variation before going live