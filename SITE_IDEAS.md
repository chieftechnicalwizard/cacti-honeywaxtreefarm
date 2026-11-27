# Honey Wax Tree Farm — Sanctuary Portal & Multi-Site Roadmap

**Target Domains:**
- **Primary Homestead Hub:** `https://www.honeywaxtreefarm.com` (Google Sites — Diplomat Pine Green theme)
- **Cactus Sanctuary Subdomain:** `https://cacti.honeywaxtreefarm.com` (`index.html` standalone & Google Sites Full-Page Embed compatible)
- **Sister Sanctuary:** `https://www.shekinahshine.org/` (Midnight-slate `#020617` 72 Angels Clock, Calendar & Contemplative Archive)

---

## 1. Unified Navigation & Information Architecture

Keeping both `www.honeywaxtreefarm.com` and `cacti.honeywaxtreefarm.com` unmistakable as wings of the same living homestead requires matching visual anchors (Playfair Display headings, `hwtf_crest.svg`, Diplomat pine + Shekinah midnight-slate surfaces, and gold hairline framing) paired with clear domain roles:

### Proposed Top-Level Nav for `www.honeywaxtreefarm.com`
1. **Home / Living Homestead** — Seasonal overview featuring the farm motto (*“Honey, Wax, Trees, Fruits, Nuts, and Culinary Mushrooms of all types!”*), hero sanctuary imagery, and quick portals.
2. **Apiary (Honey & Wax)** — Hive health notes, raw comb/beeswax harvests, and pollinator forage calendars.
3. **Orchards & Guilds (Trees, Fruits, Nuts)** — Polyculture guilds, rootstock logs, grafting notes, and frost-protection updates.
4. **Mycology (Culinary Mushrooms)** — Inoculation logs, substrate trials, fruiting chamber conditions, and partner links (e.g., Sonoran Spores).
5. **Cactus Sanctuary (`cacti.honeywaxtreefarm.com`)** — Full-Page Embed of `index.html` or direct portal link to the 24/7 Live Cam Studio + 17-Cross / 23-Clone Archive.
6. **Sacred Calendar & Audio (`shekinahshine.org` + FM-1 Radio)** — Cross-link to the 72 Angels Clock and contemplative audio streams.
7. **Stewardship & Donate** — Unified groundkeeping support (`PayPal`, `CashApp`, `Venmo`) and community links.

### Navigation Inside `cacti.honeywaxtreefarm.com`
- **Top Sanctuary Bar:** Crest lockup -> In-page smooth anchors (`Live Cams`, `17 Crosses`, `23 Clones`, `Labels`, `Support`) -> External constellation pills (`HoneyWaxTreeFarm.com`, `Shekinah Shine`, `GitHub`) -> Gold `Donate` CTA.
- **Embed Compatibility Rule:** All outbound links use `target="_blank" rel="noopener noreferrer"` so links clicked inside a Google Sites iframe open cleanly without hitting `X-Frame-Options` blocks.

---

## 2. 24/7 Live Cam Showcase Upgrades

The current broadcast studio (`TopDown Greenhouse Main Cam`, `SideCam 2K PTZ`, `Outdoor Habitat Cam`, `Indoor Sanctuary Cam`, plus the 13-video `Cactus Cam Playlist` and `2×2 Quad Live Wall`) sets the foundation. Next high-impact enhancements:

1. **Harmonic PTZ Tour Phase Indicator:**
   - The broadcast scripts (`TopDown` `900s`, `SideCam` `1800s`, `Indoor` `1800s`, `Outdoor` `5400s`) already lock to a unified tour epoch. Adding a tiny client-side phase pill (`Next Motorized PTZ Tour in MM:SS`) lets viewers know exactly when `SideCam` or `Outdoor` will glide across close-up specimens (`Super Pedro × Yowie`, `Dayman Pup`, `Tall Grafted El Serpente`).
2. **Live "Now Playing" Narration & Soundscape Ribbon:**
   - Publish a tiny, sanitized static JSON file every 60 seconds (e.g., `status/now_playing.json` via Cloudflare/CDN or GitHub raw without exposing private IPs) displaying the current audiobook chapter title and 48 kHz ambient soundscape act accompanying each camera.
3. **Standby & 850nm IR Transparency Pill:**
   - Explain clearly to nighttime or mobile viewers when a camera enters `850nm IR Night Mode` (revealing stark monochrome spine/areole geometry) or dual-WAN `Audio Sanctuary Standby` (preserving uninterrupted 48 kHz narration during rural link congestion).
4. **Specimen Hotspots Drawer:**
   - Beneath each camera switcher card, allow clicking featured specimen tags (`Kimach × Jessica #0211`, `TBM Multi-Node`, `Volcano 3 × Ganesha`) to pop open a short botanical note card and graft date.

---

## 3. FieldWatch Specimen Ledger Integration

Integrating field observations and nursery bench inventory turns the static archival dossier into a living operational ledger without sacrificing offline/iframe simplicity:

1. **Extended Local Bench State + JSON Backup (`sp_seedling_dossier_labeled_v1`):**
   - Keep `localStorage` wrapped in `try/catch` for iframe safety while adding optional **Export/Import Bench JSON** alongside CSV export so growers can record pot counts, sowing dates, graft stock (`Pereskiopsis`, `PC`, `Sun Goddess`), and overwintering bay locations per cross (`#01`–`#17`).
2. **QR / NFC Accession Stake Generation:**
   - Enhance the `Printable Stake Labels & CSV` view to generate compact inline SVG QR codes encoding `https://cacti.honeywaxtreefarm.com/#cross-01` (or `#clone-ss02`) right on each 3-up printed pot stake. Scanning a greenhouse stake with a phone opens that exact cross's mother/father provenance instantly.
3. **FieldWatch Telemetry & Photo Checkpoints:**
   - Pair periodic macro captures and environmental sensor summaries (greenhouse canopy temperature, PAR/grow-light photoperiod, humidity) from the homestead monitoring stack into an optional `ledger.json` feed so each named stand or cross shows latest season growth delta and flower-bud alerts.

---

## 4. Seasonal Seed, Pup & Cut Exchange Log

To support preservation sharing and community trading cleanly without running an insecure database backend:

1. **Static `exchange.json` Inventory Block:**
   - A small, human-editable JSON table rendering a seasonal **Sanctuary Exchange Ledger** (`Available Cuts`, `Rooting Pups`, `Seed Batches`, `Waiting List / NFS Mother Stands`).
   - Each row links directly to the corresponding Cross (`#01`–`#17`) or Parent Clone (`SS02`, `Ogun`, `BK09511.7`, `Cahuilla`, `Althea`, etc.) card so recipients receive full verifiable pedigree before requesting a cut or seed pack.
2. **Provenance Verification Badge:**
   - Include origin traceability (`OP Listing`, `Mother Stand`, `Year Acquired`, `Graft vs. Own Roots`) and link to community etiquette hubs like `r/sanpedrocactusforsale` and trusted growers (`Dave's Bud`, `Medicactus`, `East Austin Succulents`).
3. **Seasonal Windows Banner:**
   - Automatic seasonal banner indicating active shipping/cutting months vs. winter dormancy preservation hold, protecting cuttings from transit freeze damage.

---

## 5. FM-1 Hardware Synth Radio Player & Audio Sanctuary Link

Music, generative ambient soundscapes, and spoken-word narration are core to the Honey Wax Tree Farm broadcast identity:

1. **Dedicated FM-1 Radio Card & Sticky Mini-Bar Option:**
   - Add a lightweight **FM-1 Hardware Synth Radio** card inside the Broadcast Studio and Ecosystem Hub linking directly to the live hardware synth / generative radio stream URL once exposed over HTTPS (`audio/mpeg` or `HLS` endpoint, or dedicated player route).
   - Provide a one-click **"Mute Quad Video + Play FM-1 Audio"** workflow so visitors viewing all 4 cactus cams in `2×2 Quad Live Wall` mode can enjoy a single unified synth or ambient audio stream instead of overlapping YouTube tracks.
2. **72 Angels Clock Cross-Link (`shekinahshine.org`):**
   - Pair the nocturnal conservatory experience with a subtle celestial link to Shekinah Shine's 72 Angels Clock & Calendar for late-night contemplative viewers.

---

## 6. Deployment & Google Sites Embed Hygiene

- **Zero-Build Static Footprint:** Keep `index.html` self-contained with local `assets/` (`hwtf_crest.svg`, `hero_sanctuary.webp`, `cam_*.webp`) so it deploys instantaneously to Cloudflare Pages, GitHub Pages, or local Nginx with zero bundler drift.
- **Google Sites Full-Page Embed Checklist:**
  - Confirm `X-Frame-Options` allows embedding on `sites.google.com` (or use Cloudflare Transform Rules / default permissive framing on `cacti.honeywaxtreefarm.com` without `DENY`).
  - Keep `referrerpolicy="strict-origin-when-cross-origin"` on every YouTube `<iframe>` so nested YouTube playback works cleanly inside Google Sites embeds.
  - Maintain `try/catch` guards around `localStorage` and clipboard calls for cross-origin sandbox resilience, and preserve `@media print` rules for one-click greenhouse stake printing.
