# Custom Nav Banner — Shopify Section

Hero banner section for bundle landing pages. Fully configurable via the Shopify Theme Editor.



## Approach

The goal was to build a custom Shopify banner section for a bundle page A/B test using Intelligems.

A custom-banner.liquid section was created with full Theme Editor controls — heading, CTA, images, overlay — so the client can manage content without touching code.
The section is included in the **Control URL** of the Intelligems test, while the Variation runs the same bundle pack without it — keeping the test clean and isolated.
**Add to Cart Rate** and **Revenue Per Session** are tracked as metrics to measure whether the banner drives more conversions.
Responsive fixes ensure the layout works across all screen sizes, with a dedicated mobile image.
All changes (alt tags, CTA, responsive fixes) were made directly in the section file to keep the codebase minimal and easy to maintain.

---

## Files
- `custom-banner.liquid` — Section markup, styles, and schema
- `custom_navbar.liquid` — Custom navigation bar section

---

## Theme Editor Settings
- **Content:** Heading, highlighted text, subtext, highlight color
- **CTA Button:** Button text, link, background, text color, hover color
- **Images:** Desktop image, mobile image, background images, logo
- **Navigation:** Menu link list

---

## Task Status

| Task | Status |
|---|---|
| Alt attributes on all images | ✅ Done |
| README added to GitHub | ✅ Done |
| View: [Live](https://ankush-kumar-digital-design.myshopify.com/products/herbal-daily-multivitamin-with-natural-plant-extracts-minerals) | 🔗 |
| Intelligems primary & secondary metrics configured | ✅ Done |
| Target page set to Product Page (PDP) | ✅ Done |
| A/B test: Control vs Variation (both bundle packs; this section in Control URL) | ✅ Done |

---

## Intelligems A/B Test

| | Details |
|---|---|
| **Test ID** | `1fcbb94a-5c30-49de-b06f-16eb3c0de911` |
| **Control Group ID** | `53e3b4ce-895f-4ade-94af-9eecd626d61c` |
| **Variation ID** | `411bd667-4291-4792-80ca-ed88dc76f02b` |
| **Primary Metric** | Add to Cart Rate |
| **Secondary Metric** | Revenue Per Session |

**Preview URLs**

- Control: `https://ankush-kumar-digital-design.myshopify.com/products/herbal-daily-multivitamin-with-natural-plant-extracts-minerals?ig-preview=1fcbb94a-5c30-49de-b06f-16eb3c0de911&igTg=53e3b4ce-895f-4ade-94af-9eecd626d61c&preview_theme_id=157371990147&pb=0`
- Variation: `https://ankush-kumar-digital-design.myshopify.com/products/herbal-daily-multivitamin-with-natural-plant-extracts-minerals/?ig-preview=1fcbb94a-5c30-49de-b06f-16eb3c0de911&igTg=411bd667-4291-4792-80ca-ed88dc76f02b&preview_theme_id=157371990147&pb=0`

**Integration Keys**
- Control: `9eecd626d61c`
- Variation: `ed88dc76f02b`
| Responsive layout errors fixed | ✅ Done |
| CTA button and link added | ✅ Done |


