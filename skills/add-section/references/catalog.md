# Jiro Build catalog reference

Use these values with `search_components`. Categories can change. If a category is rejected, the response lists every valid one in `valid_categories`.

## Groups (`group`)

- `marketing-blocks`: page sections
- `ui-components`: small UI pieces
- `templates`: complete landing pages

## Section categories (`group: marketing-blocks`)

| Category slug | What it holds |
|---|---|
| `header` | Heroes and navbars, the top of the page |
| `about-us` | About and story sections |
| `features` | Feature grids and feature highlights |
| `how-it-works` | Step-by-step process sections |
| `why-choose-us` | Benefits and comparison sections |
| `brands` | Logo clouds ("trusted by") |
| `integration` | Integration and partner grids |
| `stats-metrics` | Numbers and KPI sections |
| `testimonial` | Reviews and social proof |
| `team` | Team members |
| `pricing` | Pricing tables and plans |
| `faq` | Questions and answers |
| `calls-to-action` | Call-to-action banners |
| `contact-us` | Contact forms and details |
| `blogs-articles` | Blog and article grids |
| `footer` | Page footers |

Common words map automatically: "hero" and "navbar" go to `header`, "cta" to `calls-to-action`, "testimonials" or "reviews" to `testimonial`, "logos" to `brands`, "stats" to `stats-metrics`.

## UI component categories (`group: ui-components`)

`background`, `button`, `cards`

## Template categories (`group: templates`)

`agency`, `ai-agents-chatbots`, `ai-creative-media-tools`, `developer-tools`, `e-commerce`, `education-careers`, `events-conferences`, `fintech`, `health-wellness`, `local-services`, `marketing-sales`, `media-publishing`, `nonprofit-charity`, `portfolio`, `productivity-automation`, `professional-services`, `real-estate-construction`, `travel-hospitality`

## Filter values

- `theme`: `light`, `dark`, `colorful`
- `look`: `bold`, `creative`, `elegant`, `futuristic`, `minimal`, `modern`, `playful`, `professional`, `retro`
- `layout`: `centered`, `split`, `grid`, `stacked`, `asymmetric`, `full-bleed`
- `motion`: `true` for sections that animate with framer-motion, GSAP or three.js
- `accents` (any of): `green`, `lime`, `orange`, `purple`, `blue`, `teal`, `pink`, `red`, `gold`, `mint`, `black`, `white`, `gray`, `burgundy`
- `industries` (any of, up to 3): `agency`, `ai`, `coaching`, `creative`, `developer tools`, `ecommerce`, `education`, `events`, `finance`, `health & wellness`, `marketing`, `media & blog`, `nonprofit`, `portfolio`, `productivity`, `real estate`, `recruitment`, `saas`, `startup`, `technology`, `travel`
- `tags` (all must match, up to 7): `3d`, `accordion`, `animated`, `animated numbers`, `animated text`, `avatars`, `badges`, `black & white`, `bold`, `brand logos`, `brutalist`, `carousel`, `colorful`, `comparison table`, `dark`, `dashboard preview`, `elegant`, `futuristic`, `glassmorphism`, `gradient`, `grid`, `interactive`, `large type`, `light`, `marquee`, `minimal`, `modern`, `monthly/yearly toggle`, `neon`, `newsletter`, `pastel`, `photography`, `playful`, `retro`, `stats`, `tabs`, `video`, `video background`
- `premium`: `true` for premium items only, `false` for free items only. Leave it out for both.

Tags must all match, so one or two tags work better than five.
