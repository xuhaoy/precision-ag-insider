# Precision Ag Insider Traffic Growth Plan

## Current Findings

- The site is live at `https://xuhaoy.github.io/precision-ag-insider/`.
- Daily and weekly cron jobs exist, but both recently failed because `google/gemini-3-flash-preview` hit rate limits.
- Many older posts were plain Markdown assets instead of fully rendered Jekyll pages, limiting SEO metadata, RSS inclusion, and consistent article structure.
- Homepage SEO metadata was generic: "The AI Farming Revolution".
- The homepage is a long manual list. It has content depth, but weak topical organization and weak internal navigation.
- Post quality is consistent in niche, but several titles repeat similar phrases like "2026", "leap", "shift", "new standard", and "agentic AI", which can make the site look synthetic and reduce long-tail keyword coverage.
- GoatCounter feedback on 2026-05-27 showed visitors were not clicking into posts; the homepage needed clearer paths and stronger visual affordances, not just more SEO metadata.

## High-Impact Changes Made

- Added `url`, `baseurl`, richer site description, `jekyll-feed`, and `jekyll-seo-tag` settings.
- Added `robots.txt`, `sitemap.xml`, and `feed.xml`.
- Added a `post` layout with article metadata, homepage breadcrumb, publication info, standard affiliate disclosure, and Article JSON-LD.
- Added front matter to older posts that were previously not rendered as full Jekyll pages.
- Updated cron prompts to require valid front matter, build verification, more credible/practical claims, and fallback execution if Gemini is rate-limited.
- Enabled failure alerts for both scheduled jobs and direct weekly analytics delivery to Jack.
- Rebuilt the homepage around featured cards, topic paths, practical guides, a latest grid, and a collapsed archive.
- Added topic hub pages for soil sensors, farm robotics, precision irrigation, ag drones, and farm AI ROI.

## Next Best Moves

1. Create topic hubs:
   - `/topics/soil-sensors/`
   - `/topics/farm-robotics/`
   - `/topics/precision-irrigation/`
   - `/topics/ag-drones/`
   - `/topics/farm-ai-roi/`

2. Shift part of the content calendar from trend posts to search-intent posts:
   - "Best soil moisture sensors for farms in 2026"
   - "Precision irrigation ROI calculator"
   - "Agricultural drone rules by region"
   - "RTK GPS vs computer vision for autonomous tractors"
   - "How to choose edge AI hardware for farm equipment"

3. Add comparison and buyer-intent pages:
   - Product category roundups with tables
   - "Best for small farms / orchards / row crops / greenhouse"
   - Clear affiliate disclosures and practical selection criteria

4. Add credibility signals:
   - Sources section on every new post
   - Separate "what is available today" from "2026 outlook"
   - Replace overly precise unsupported numbers with sourced or clearly framed estimates

5. Improve internal linking:
   - Every new post should link to 2-4 older relevant posts.
   - Topic hubs should link to the highest-value posts.
   - Homepage should feature topic hubs above the post archive.

6. Track content performance weekly:
   - Top pages
   - Top referrers
   - Search terms when available
   - Posts with high impressions but low clicks
   - Posts with traffic but weak affiliate intent
