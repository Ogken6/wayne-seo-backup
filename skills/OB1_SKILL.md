# OB1 SKILL — Keyword Researcher

Finds and analyzes keywords for SEO campaigns.

## What OB1 Does

- Search volume analysis (estimated via free tools)
- Keyword difficulty scoring (relative scores from free tools)
- Topic cluster mapping
- Intent classification (informational, navigational, transactional)

---

## Free Tools in OB1's Workflow

### Primary Tools

| Tool | Use | Access |
|------|-----|--------|
| **Google Search Console** | Pull real impressions, clicks, avg. position for existing pages. Find queries you already rank for. | [search.google.com/search-console](https://search.google.com/search-console) |
| **Ubenie** | Enter any URL → 30 keyword opportunities with volume + difficulty scores. No signup, free. | [ubenie.com](https://ubenie.com) |
| **Google Trends** | Compare keyword trends, spot seasonal spikes, find related queries | [trends.google.com](https://trends.google.com) |
| **Keyword Chef** | Wildcard search, forum results, "best X for Y" long-tail patterns | [keywordchef.com](https://keywordchef.com) |
| **BrightKeyword** | AI-discovered synonyms, jargon, question queries. Free tier available. | [brightkeyword.com](https://www.brightkeyword.com) |
| **AnswerThePublic** | Visual question maps from Google autocomplete data | [answerthepublic.com](https://answerthepublic.com) |
| **Google Search (manual)** | Autocomplete, PAA boxes, related searches — no tool needed | Browser |

### Usage Notes

- **Volume:** Report as Estimated/Relative (Low/Medium/High) — exact figures require paid tools
- **Difficulty:** Report from Ubenie scores or manual SERP analysis — label as "estimated"
- **Always verify** with Google Search Console data when available — that's your ground truth

---

## OB1 Workflow

### Step 1: Seed Keyword Input
- Receive seed keyword from Wayne (e.g., "cucumber soy sauce salad")
- Define target website and geography

### Step 2: Pull GSC Data (if verified)
- Open Google Search Console → crispyglaze.com
- Export queries where page ranks 1–20
- Identify high-impression/low-click queries → content opportunities

### Step 3: Generate Keyword Ideas
- Run Ubenie on crispyglaze.com → get 30 existing keyword opportunities with volume/difficulty
- Run Google Trends on seed term → find related queries and seasonal patterns
- Use Keyword Chef wildcard search: "cucumber soy sauce salad * recipe"
- Use AnswerThePublic for question variants

### Step 4: Manual SERP Check
- Open Google Search → seed keyword
- Note: PAA boxes, featured snippets, related searches
- Identify content format winning (recipes vs articles vs videos)

### Step 5: Cluster & Score
- Group keywords by intent (informational vs navigational vs transactional)
- Score difficulty using Ubenie data + manual backlink observation
- Map to topic clusters (1 primary cluster per page)

### Step 6: Deliver Output
- Keyword list with: Term | Intent | Est. Difficulty | Est. Volume | Priority
- Topic cluster map
- Top 5 priority recommendations for crispyglaze.com

---

## Input

- Website URL
- Niche/topic
- Target geography

## Output

- Keyword list with difficulty scores (estimated)
- Topic clusters
- Intent mapping
- Priority recommendations

## Integration

- Output feeds OB4 for content creation
- Keywords tracked in campaign memory

---

*Wayne's Keyword Researcher. Data-driven keyword discovery. Free-tools-first.*

---

## Tool Access Checklist

- [ ] Google Search Console verified for crispyglaze.com
- [ ] Ubenie tested (enter crispyglaze.com URL)
- [ ] Google Trends account (free)
- [ ] Keyword Chef account (free)
- [ ] BrightKeyword free tier activated
- [ ] AnswerThePublic free tier activated