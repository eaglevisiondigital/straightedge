# STRAIGHT EDGE - APPROVED HOMEPAGE REBUILD

Status: **Rebuild branch only. Not approved for publication.**

## Source of truth
- `approved-full-homepage-reference.png` is the approved FLATTENED VISUAL COMPOSITION (948 x 1659). The user approved its photographs, mailbox, layout, exact compositions, type, fade and red/black/white styling.
- Original company logo source supplied in chat must replace the mockup-derived header crop before acceptance.
- The only separately available high-resolution rendered asset is `illuminated-mailbox.png` (1254 x 1254), which must be checked against the approved version and kept at the curb, metal front door toward street, number 27 on side, soft light between slabs.
- `hero-approved-right.jpg` (1106 x 866) is a flattened portion of the mockup. It includes design artifacts and cannot produce a clean editable hero background.
- **The service image files below are flattened low-resolution mockup crops, not original full-resolution source photography.** They must NOT be enlarged as final production assets.

## Inventory and image acceptance

| Role | Existing file | Current dimensions | Release decision |
|---|---|---:|---|
| Whole-page approved visual | approved-full-homepage-reference.png | 948×1659 | Reference only |
| Header logo cropped out of mockup | approved-header-logo-crop.png | 816×216 | Replace with exact original logo |
| Hero home/background | hero-approved-right.jpg | 1106×866 | BLOCKED: must obtain clean, high-resolution version matching approved photo |
| Mailbox | illuminated-mailbox.png | 1254×1254 | Candidate; inspect alpha and compare |
| Fencing | fencing.jpg | 396×236 | BLOCKED: source image needed |
| Construction | construction.jpg | 480×236 | BLOCKED: source image needed |
| Lawn and landscape | lawn-landscape.jpg | 426×236 | BLOCKED: source image needed |
| Deck and dock | deck-dock.jpg | 414×236 | BLOCKED: source image needed |
| Doors and locks | doors-locks.jpg | 592×238 | BLOCKED: source image needed |
| Drywall and more | drywall.jpg | 552×238 | BLOCKED: source image needed |
| Custom mailboxes card | custom-mailboxes.jpg | 588×238 | BLOCKED: needs scene with approved mailbox and curb |
| Property care condos | property-care.jpg | 834×428 | BLOCKED: original uncropped photo needed |

## Design contract

- Maintain exact section sequence: dark branded header, Florida white coastal exterior hero with superimposed illuminated mailbox and soft left-to-right fade, 4+3 seven-service cards, property-care banner with beachfront condo, why-us icons + CTA, footer.
- Retain the user-approved heading: EXCEPTIONAL CRAFTSMANSHIP. UNCOMPROMISING INTEGRITY.
- Retain brand red / white / charcoal, structural proportions, image scenes and crops, typography, baseline spacing and CTAs.
- Render hero text/buttons as selectable HTML above separate full-resolution photo; `::before` background should extend edge-to-edge, and use a CSS gradient over it, not an opaque black rectangle with an abrupt edge.
- Every approved photo must be checked for source identity, sufficient actual pixels, aspect and focal point, not simply matched by subject description. If the original source is irretrievable, request explicit approval for that one replacement before shipping.
- Do not claim existing JPG crops are full-resolution images.
- Use semantic accessible markup; functional responsive nav/phone/estimate form, Netlify Forms kept intact.
- Do not replace existing Netlify project; preserve `main` and production.

## Build and release gates
1. Recover original image sources and logo. Store in repo with descriptive immutable paths and a photo/source manifest. Do not silently regenerate.
2. Build desktop components and full-bleed graduated hero. Compare screenshots at identical viewport dimensions with approved reference.
3. Verify no sharp left-edge transition, no phantom embedded text, no squashed or pixelated service images, no fake letters/logos in photography.
4. Review desktop 1440 / 1024 / 768, mobile 390 / 320 and test actual Netlify form submission/notification settings.
5. Create PR into `main`, examine Git-connected Netlify Deploy Preview and obtain explicit visual approval before merge.
6. After publication, verify production deploy SHA and live screenshots.
