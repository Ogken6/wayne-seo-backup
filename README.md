# Wayne — Chief SEO Agent

> **Private repository.** Wayne is Ken's autonomous SEO expert, managing all search optimization for `crispyglaze.com` and `greenlytidy.com`.

---

## 🔍 What Wayne Is

Wayne is an AI SEO specialist built inside [OpenClaw](https://github.com/openclaw/openclaw). He operates as Ken's in-house SEO department — data-driven, methodical, and fully autonomous.

Wayne never guesses. Every recommendation is backed by real metrics from free SEO tools.

**Core sites managed:**
- [crispyglaze.com](https://crispyglaze.com) — Recipe content, AdSense revenue
- [greenlytidy.com](https://greenlytidy.com) — Sustainable living

---

## ⚙️ Architecture

Wayne is the orchestrator. Six specialist sub-agents report to him:

```
Wayne (Chief SEO Expert)
├── OB1 — Keyword Researcher
├── OB2 — Technical SEO Agent
├── OB3 — SERP & Competitor Analyst
├── OB4 — Content & AEO Agent
├── OB5 — GEO Agent (AI Visibility)
└── OB6 — Recipe Opportunity Finder
```

---

## 🧑‍💼 OB1 — Keyword Researcher

Finds and scores keywords for SEO campaigns.

### What OB1 Does
- Search volume analysis (estimated via free tools)
- Keyword difficulty scoring
- Topic cluster mapping
- Intent classification (informational, navigational, transactional)

### Free Tools Used
| Tool | Use |
|------|-----|
| Google Search Console | Real impressions, clicks, avg. position |
| Ubenie | 30 keyword opportunities per URL with volume + difficulty |
| Google Trends | Trend comparison, seasonal spikes |
| Keyword Chef | Long-tail wildcard patterns |
| BrightKeyword | AI-discovered synonyms and question queries |
| AnswerThePublic | Visual question maps |

### Workflow
1. Pull GSC data for existing rankings (positions 1–20)
2. Run Ubenie on target URL → 30 keyword opportunities
3. Google Trends for seasonal validation
4. Keyword Chef wildcard search
5. AnswerThePublic question mapping
6. Cluster by intent → score difficulty → deliver ranked list

### Output
```
Term | Intent | Est. Difficulty | Est. Volume | Priority
```
Topic clusters, intent mapping, top 5 priority recommendations.

### Feeds
- → OB4 (content creation)
- → OB6 (recipe keyword discovery)

---

## 🛠 OB2 — Technical SEO Agent

Handles all technical SEO aspects for both sites.

### What OB2 Does
- Core Web Vitals audits (LCP, INP, CLS)
- Crawlability checks (Screaming Frog)
- Schema markup implementation and validation
- Site speed optimization
- Mobile-friendliness verification
- XML sitemap + robots.txt analysis

### Free Tools Used
| Tool | Use |
|------|-----|
| Google PageSpeed Insights | LCP, INP, CLS + CrUX field data |
| Google Search Console | Index coverage, CWV reports, crawl errors |
| Screaming Frog SEO Spider | Crawl 500 URLs free — broken links, meta, redirects |
| Google Rich Results Test | Recipe schema validation |
| searchsavvy.in | Free recipe schema generator |
| searchbulb.com | Free schema generator |

### Core Web Vitals Targets
| Metric | Target |
|--------|--------|
| LCP | < 2.5s |
| INP | < 200ms |
| CLS | < 0.1 |

### Schema Quick Reference (Recipe)

**Required fields:**
```json
{
  "@type": "Recipe",
  "name": "Recipe Title",
  "image": "https://example.com/image.jpg",
  "author": { "@type": "Person", "name": "Ken" },
  "recipeIngredient": ["ingredient 1", "ingredient 2"],
  "recipeInstructions": [{ "@type": "HowToStep", "text": "Step 1" }],
  "prepTime": "PT30M"
}
```
**ISO 8601 durations:** 30 min = PT30M | 1 hour = PT1H | 1h 15m = PT1H15M

### Workflow
1. PageSpeed Insights on homepage + top 5 recipe pages
2. GSC Coverage + Core Web Vitals review
3. Screaming Frog crawl (500 URL limit)
4. Recipe schema generation + Rich Results Test
5. Mobile + accessibility check
6. Deliver prioritized issue report with fix code

### Severity Levels
| Level | Issues | Response |
|-------|--------|----------|
| Critical | CWV failing, canonical errors, schema blocking rich results | Fix within 48h |
| High | Broken links, missing meta, LCP 4s+ | Fix within 1 week |
| Medium | Missing alt text, minor schema gaps | Next content cycle |

### Feeds
- Technical issues → Tracked for fix, re-audited
- Schema → OB4 for integration
- Reports → Wayne (quality gate)

---

## 📊 OB3 — SERP & Competitor Analysis Agent

Analyzes the search landscape and tracks competitor movements.

### What OB3 Does
- SERP feature tracking (AI Overview, People Also Ask, featured snippets, video/image carousels)
- Competitor content analysis
- Ranking factor research
- SERP volatility monitoring
- Keyword gap analysis

### SERP Features Tracked
- AI Overview presence
- People Also Ask (PAA)
- Featured snippets
- Local pack
- Image pack
- Video carousel
- Knowledge panels

### Free Tools Used
| Tool | Use |
|------|-----|
| Ubenie | Competitor keyword gaps + opportunity scores |
| Neil Patel SEO Analyzer | Top results, difficulty, volume estimates |
| BuzzSumo | Most-shared content analysis (3 free searches/day) |
| Similarweb | Traffic estimates, top pages, audience |
| Google Search (manual) | SERP feature and title analysis |

### Primary Competitors for crispyglaze.com
| Competitor | URL | Angle |
|------------|-----|-------|
| Kirbie's Cravings | kirbiecravings.com | High-volume Asian recipes |
| Jessica Gavin | jessicagavin.com | Professional recipe formatting |
| The Woks of Life | thewoksoflife.com | Chinese/Japanese authority |
| Just One Cookbook | justonecookbook.com | Detailed Japanese recipes |
| I A Food Blog | iamafoodblog.com | Food photography focus |
| RecipeTin Eats | recipetineats.com | Quick/easy recipe angle |

### Workflow
1. Manual SERP scan (incognito) — identify all features
2. Ubenie on 6 competitors → export top 30 keywords each
3. Cross-reference against crispyglaze.com GSC data → find gaps
4. Content format analysis (top 5 pages: word count, headings, schema)
5. Neil Patel SEO Analyzer for ranking factors
6. Weekly position tracking for volatility monitoring
7. Deliver SERP feature map + competitor gap list

### Output
- SERP feature map per keyword
- Competitor keyword gap analysis
- Content format recommendations
- Top 5 ranked opportunities (difficulty vs reward)

### Feeds
- Opportunities → OB4 (content creation)
- Keyword gaps → OB1 (refine keyword list)
- Reports → Wayne (strategic planning)

---

## ✍️ OB4 — Content & AEO Agent

Optimizes all content for search engines AND AI citation systems.

### What OB4 Does
- On-page SEO optimization
- AI search optimization (AEO)
- E-E-A-T improvements
- Content structuring and readability
- Meta tag optimization
- Internal linking strategy
- Schema markup integration
- Featured snippet optimization

### AEO Focus Areas
- Answer-focused content structure (AI-parsable)
- Statistics with sources (AI citation bait)
- Clear ingredient lists with quantities
- Numbered step sequences
- Expert attribution in author bio
- FAQ sections optimized for PAA + AI

### Free Tools Used
| Tool | Use |
|------|-----|
| Hemingway Editor | Readability target: grade 7 or below |
| Yoast SEO (WordPress) | Content optimization, readability, schema |
| AnswerThePublic | FAQ section generation |
| Google Rich Results Test | Schema validation before publish |
| searchsavvy.in | Recipe JSON-LD generation |
| NLP Bucket | NLP keyword suggestions from top-ranking pages |

### Readability Targets
- Hemingway grade ≤ 7
- Average sentence length ≤ 25 words
- Passive voice < 10%
- Complex words spelled out on first use

### Workflow
1. Receive content brief from OB1 (keywords + intent)
2. Review OB3 competitor content format report
3. AnswerThePublic for question mapping
4. Write/review with Hemingway Editor open
5. Generate Recipe schema via searchsavvy.in
6. Meta title (≤60 chars) + meta description (≤160 chars)
7. Pre-publish: Rich Results Test + schema validation
8. Deliver final content + meta tags + schema + internal link suggestions

### Content Quality Checklist
**On-Page SEO:**
- Primary keyword in H1, first 100 words, last 100 words
- Secondary keywords in 2–3 H2s
- Image alt text includes keyword

**Schema (Rich Results Test):**
- Recipe name = H1
- Image URL absolute, 1200×800+
- Author present
- Min 2 ingredients, min 2 instruction steps
- prepTime in ISO 8601
- aggregateRating if reviews exist

**AEO / AI Citability:**
- Statistics present with attribution
- Ingredient quantities specific (not "some")
- Numbered step sequence
- Cuisine/region entity in intro
- Author credentials in bio

### Feeds
- Input: OB1 (keywords), OB3 (SERP analysis)
- Output: Elena (human voice editing if needed)
- Schema: OB2 (implementation verification)
- Reports: Wayne

---

## 🤖 OB5 — GEO Agent

Generative Engine Optimization — optimizes for AI search visibility.

### What OB5 Does
- AI search visibility optimization (ChatGPT, Perplexity, Claude, Gemini, Google AI Overviews)
- llms.txt generation and maintenance
- FAQPage + Article + Organization schema markup
- Structured data for AI parsing
- Source citation optimization
- GEO metrics tracking (manual + HubSpot free tier)

### AI Platforms Tracked
- ChatGPT (800M+ weekly active users)
- Perplexity AI (780M+ monthly queries)
- Google AI Overviews (60%+ of searches)
- Claude
- Gemini

### Free Tools Used
| Tool | Use |
|------|-----|
| Google Search Console | Baseline branded search traffic |
| Perplexity AI (manual) | Monthly citation check |
| ChatGPT (manual) | Monthly brand mention check |
| HubSpot AI Search Grader | Free tier — baseline AI performance score |
| Google Rich Results Test | Schema validation |

### GEO Strategies That Work (No Cost)
Research shows 30–40% AI visibility lift from:
- **Statistics Addition:** "4.2 stars from 1,847 ratings"
- **Cite Sources:** Link to authoritative sources with attribution
- **Quotation Addition:** Expert quotes with name/title
- **Clear structure:** H2s, bullet lists, numbered steps
- **Entity clarity:** Cuisine type, region, ingredient names explicit

### Workflow
1. Schema foundation audit (Recipe + FAQPage + Article + Organization)
2. Content GEO audit (AI citability signals check)
3. Citation optimization (stats, expert quotes, entity clarity)
4. HubSpot AI Search Grader baseline
5. Manual citation tracking spreadsheet (monthly)
6. llms.txt maintenance (quarterly)
7. Deliver GEO report + schema markup + tracking spreadsheet

### llms.txt Format Reference
See [MongoDB's llms.txt guide](https://www.mongodb.com/learn/infrastructure/llms-faq) for the standard format.

### GEO Metrics Tracked
| Metric | Method | Frequency |
|--------|--------|-----------|
| AI citation rate | Manual Perplexity + ChatGPT queries | Monthly |
| Branded search lift | Google Search Console | Monthly |
| AI Search Grader score | HubSpot AI Search Grader (free) | Monthly |
| Rich result eligibility | Google Rich Results Test | Per page publish |
| Schema errors | GSC Enhancement report | Weekly |

### Feeds
- Schema → OB2 for implementation
- Content restructuring → OB4
- Reports → Wayne on AI visibility trends

---

## 🍳 OB6 — Recipe Opportunity Finder

Finds recipe-specific SEO opportunities before the competition.

### What OB6 Does
- Recipe content gap analysis
- Recipe schema opportunity scan
- Trending recipe topic identification (TikTok → Google Trends validation)
- Seasonal content planning
- Recipe keyword discovery via modifier patterns
- Cook time/prep time optimization
- Structured data opportunities

### Free Tools Used
| Tool | Use |
|------|-----|
| TikTok Search | Trend discovery (weekly) — before it hits traditional SEO tools |
| Google Trends | Validate TikTok trends with search interest data |
| Ubenie | Keyword opportunities with volume + difficulty |
| Reddit | Real user pain-point questions → recipe topics |
| Exploding Topics | Emerging topics at early growth stage |
| YouTube Search | Video demand (autocomplete + titles + comments) |
| KitchenSEO | Food blog–specific modifier pattern research |
| AnswerThePublic | Question-based keyword clusters |

### Recipe Content Modifier Patterns (KitchenSEO)
```
Ingredient + method:    "cucumber air fryer", "cucumber ferment"
Ingredient + dietary:  "cucumber keto", "cucumber vegan", "cucumber gluten-free"
Ingredient + occasion:  "cucumber summer salad", "cucumber party recipe"
Ingredient + cuisine:   "cucumber Korean", "cucumber Japanese", "cucumber Thai"
```

### Trend Discovery Workflow
1. **TikTok first** (weekly): Search seed terms, note trending titles + comment questions
2. **Google Trends validation**: Check if TikTok trend = rising search interest
3. **Ubenie check**: Run on crispyglaze.com — already have content?
4. **Competitor scan**: Have major food blogs covered it?

### Workflow
1. TikTok weekly trend scan (5 seed terms)
2. Google Trends 12-month view validation
3. Ubenie competitor gap analysis (crispyglaze.com vs competitors)
4. KitchenSEO modifier pattern keyword generation
5. Seasonal content calendar (3–6 months before peak)
6. Recipe schema opportunity scan (which pages lack rich results?)
7. Deliver trending topics + gap list + seasonal calendar + schema opportunities

### Recipe Opportunity Categories
**By Type:** Quick (15 min), one-bowl, meal prep, high-protein, low-carb, budget
**By Cuisine:** Chinese (Sichuan/Cantonese), Japanese (Izakaya/street), Korean (Banchan/BBQ), Thai, Vietnamese
**By Format:** Video, printable cards, step-by-step photos, ingredient substitution guides

### Seasonal Planning Windows
| Holiday/Season | Content Lead Time | Example Topics |
|----------------|-------------------|----------------|
| Chinese New Year | 3–4 months | Lunar New Year recipes |
| Thanksgiving | 4–5 months | Turkey sides, autumn produce |
| Summer | 2–3 months | Cold salads, grilling |
| Back to school | 2 months | Quick weeknight dinners |

### Feeds
- Trending topics → OB4 (content creation)
- Schema gaps → OB2 (implementation)
- Keyword opportunities → OB1 (clustering)
- Seasonal content → Wayne (planning calendar)

---

## 📋 Wayne's SEO Workflow (Full)

```
1. ANALYZE    → Understand site, define target keywords
2. RESEARCH   → OB1 finds keywords + topic clusters
3. AUDIT      → OB2 checks technical (Core Web Vitals, schema)
4. COMPETE    → OB3 analyzes SERP + competitor gaps
5. OPTIMIZE   → OB4 creates/optimizes content
6. EXTEND     → OB5 adds AI (GEO) visibility
7. REPORT     → Wayne summarizes for Ken
```

---

## 🔧 Tool Access Checklist

### Setup Required (Free)

**OB1 — Keyword Researcher:**
- [ ] Google Search Console verified for crispyglaze.com
- [ ] Ubenie tested on crispyglaze.com
- [ ] Google Trends (free account)
- [ ] Keyword Chef (free)
- [ ] BrightKeyword free tier
- [ ] AnswerThePublic free tier

**OB2 — Technical SEO:**
- [ ] Google Search Console verified for crispyglaze.com
- [ ] Screaming Frog installed (free version)
- [ ] searchsavvy.in bookmarked
- [ ] searchbulb.com bookmarked
- [ ] PageSpeed Insights bookmarked

**OB3 — SERP & Competitor:**
- [ ] Ubenie tested on all 6 competitors
- [ ] Neil Patel SEO Analyzer bookmarked
- [ ] BuzzSumo free tier (3 searches/day)
- [ ] Similarweb free tier

**OB4 — Content & AEO:**
- [ ] Hemingway Editor bookmarked
- [ ] Yoast SEO (WordPress) installed
- [ ] AnswerThePublic free tier
- [ ] Google Rich Results Test bookmarked
- [ ] searchsavvy.in bookmarked
- [ ] NLP Bucket free tier

**OB5 — GEO:**
- [ ] Google Search Console verified for crispyglaze.com
- [ ] HubSpot AI Search Grader free account
- [ ] Perplexity AI account (free)
- [ ] ChatGPT account (free)
- [ ] GEO tracking spreadsheet created
- [ ] llms.txt file in site root

**OB6 — Recipe Opportunity:**
- [ ] TikTok Search used weekly
- [ ] Google Trends 12-month view configured
- [ ] Ubenie tested on crispyglaze.com
- [ ] Reddit researched for recipe pain points
- [ ] Exploding Topics bookmarked
- [ ] KitchenSEO pattern list printed
- [ ] Content gap spreadsheet created

---

## 📊 Key Metrics Wayne Tracks

| Metric | Tool | Frequency |
|--------|------|-----------|
| Keyword rankings (top 20) | Google Search Console | Weekly |
| Core Web Vitals pass/fail | PageSpeed Insights + GSC | Weekly |
| Organic traffic growth | Google Search Console | Monthly |
| Click-through rate | Google Search Console | Monthly |
| Bounce rate by page | Google Analytics | Monthly |
| AI search impressions | Manual Perplexity + ChatGPT | Monthly |
| SERP feature ownership | Google Search (manual) | Weekly |

---

## 📁 File Structure

```
wayne/
├── README.md                    ← This file
├── SOUL.md                      ← Wayne's identity and purpose
├── IDENTITY.md                  ← Agent identity config
├── AGENTS.md                    ← General workspace rules
├── USER.md                      ← About Ken (user profile)
├── HEARTBEAT.md                 ← Daily proactive checks
├── TOOLS.md                     ← Tool access list
├── SEO_KNOWLEDGE.md             ← SEO knowledge base
├── SEO_RESEARCH/                ← Campaign research output
│   └── [keyword-research].md
├── skills/
│   ├── WAYNE_SKILL.md          ← Wayne orchestrator skill
│   ├── OB1_SKILL.md            ← Keyword Researcher
│   ├── OB2_SKILL.md            ← Technical SEO Agent
│   ├── OB3_SKILL.md            ← SERP & Competitor Analyst
│   ├── OB4_SKILL.md            ← Content & AEO Agent
│   ├── OB5_SKILL.md            ← GEO Agent
│   └── OB6_SKILL.md            ← Recipe Opportunity Finder
└── memory/                      ← Daily session logs
    └── YYYY-MM-DD.md
```

---

## 🚫 What Wayne Will NOT Do

- Guess at recommendations — data or it doesn't happen
- Skip data verification
- Ignore failing Core Web Vitals
- Mix SEO for both sites without separate tracking
- Exfiltrate private data

---

## 👤 The Human Behind Wayne

Wayne works for **Ken**. Ken owns and operates:
- **crispyglaze.com** — Asian-inspired recipe blog, AdSense revenue
- **greenlytidy.com** — Sustainable living blog

Wayne was created to give Ken's sites every SEO advantage possible — using free tools, data-driven decisions, and autonomous operation.

---

## 🔒 Privacy

This repository is **private**. Wayne's memory, configuration, and campaign research are not public.

*Last updated: 2026-06-11*
