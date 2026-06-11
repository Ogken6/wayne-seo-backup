# OB4 SKILL — Content & AEO Agent

Optimizes content for search and AI overview.

## What OB4 Does

- On-page SEO optimization
- AI search optimization (AEO)
- E-E-A-T improvements
- Content structuring
- Meta tag optimization
- Internal linking strategy
- Schema markup integration
- Featured snippet optimization

## AEO Focus Areas

- Answer-focused content structure
- Clear parsing for AI engines (ChatGPT, Perplexity, Claude)
- Citation-worthy sections with statistics and expert attribution
- Entity optimization (ingredients, cuisine, technique)
- FAQ sections optimized for PAA and AI citation

---

## Free Tools in OB4's Workflow

### Primary Tools

| Tool | Use | Access |
|------|-----|--------|
| **Google Rich Results Test** | Test recipe rich result eligibility before publishing | [search.google.com/test/rich-results](https://search.google.com/test/rich-results) |
| **Hemingway Editor** | Improve readability score — target grade 7 or below | [hemingwayapp.com](https://hemingwayapp.com) |
| **Yoast SEO** (WordPress) | Content optimization, readability checks, schema integration. Free version. | [yoast.com/wordpress/plugins/seo](https://yoast.com/wordpress/plugins/seo) |
| **AnswerThePublic** | Generate FAQ sections and question-based content clusters | [answerthepublic.com](https://answerthepublic.com) |
| **Google's E-E-A-T Guide** | Content quality framework — Experience, Expertise, Author, Trust | [developers.google.com/search/docs/fundamental](https://developers.google.com/search/docs/fundamental) |
| **NLP Bucket** | NLP-based keyword suggestions — top terms used in top-ranking pages | [nlpcloud.com/nlp-bucket](https://nlpcloud.com/nlp-bucket) |
| **searchsavvy.in** | Generate recipe schema (JSON-LD) to paste into page | [searchsavvy.in/recipe-schema-generator](https://searchsavvy.in/recipe-schema-generator) |

### Content Optimization Workflow

1. **Before writing:** Use AnswerThePublic to map all questions target audience asks
2. **During writing:** Hemingway Editor for readability (grade 7 or below)
3. **After writing:** Yoast SEO for on-page optimization (WordPress)
4. **Before publishing:** Google Rich Results Test to validate schema
5. **AI citability:** Add statistics, expert quotes, clear entity references

### Usage Notes
- **Readability:** Target Hemingway grade 7 or below (short sentences, common words)
- **Schema:** Always generate fresh JSON-LD via searchsavvy.in per recipe — don't copy from other pages
- **AI optimization:** Include stats (e.g., "4.2 stars from 1,847 ratings"), clear ingredient lists, step-by-step format
- **Internal links:** Use descriptive anchor text with target keyword

---

## OB4 Workflow

### Step 1: Content Brief from OB1
- Receive keyword targets and intent from OB1
- Note: Primary keyword, secondary keywords, recommended content format

### Step 2: SERP Content Analysis (via OB3)
- Review OB3's competitor content format report
- Note: What headings they use, word count, image count, schema type
- Identify gaps in their content that crispyglaze.com can fill

### Step 3: Question Research
- Run AnswerThePublic on primary keyword
- Generate FAQ section from top 10 question clusters
- Map PAA questions to H2/H3 headers in article

### Step 4: Content Draft & Optimization
- Write/review content with Hemingway Editor open
- Target: Short paragraphs, active voice, grade 7 or below
- Structure: H1 (keyword), H2 (intent), H3 (sub-points), bullet lists for ingredients
- Include: Recipe schema JSON-LD, nutrition data, author bio, internal links

### Step 5: Schema Markup
- Generate Recipe schema via searchsavvy.in
- Include: name, image (1200×800+), author, ingredients, instructions, prepTime, cookTime, aggregateRating
- Add: FAQPage schema if FAQ section present

### Step 6: Meta Tags
- Meta title: Primary keyword + benefit + brand (max 60 chars)
- Meta description: Hook + keyword + call to action (max 160 chars)
- URL slug: kebab-case primary keyword

### Step 7: Pre-Publish Validation
- Run content through Google Rich Results Test
- Check: All schema fields populated, image URLs absolute, author present
- Verify: Internal links working, external links nofollow or open in new tab

### Step 8: Deliver Output
- Final content (HTML or document)
- Meta title + description
- Schema markup (JSON-LD code)
- Internal link suggestions
- AEO recommendations (stats to add, entities to highlight)

---

## Content Quality Checklist

### On-Page SEO
- [ ] Primary keyword in H1, first 100 words, last 100 words
- [ ] Secondary keywords in 2–3 H2s
- [ ] Meta title < 60 chars with primary keyword
- [ ] Meta description < 160 chars with hook
- [ ] Image alt text includes keyword
- [ ] Internal links with descriptive anchor text

### Readability (Hemingway)
- [ ] Readability grade ≤ 7
- [ ] Sentence length ≤ 25 words average
- [ ] Passive voice < 10% of sentences
- [ ] Complex words spelled out on first use

### Schema (Google Rich Results Test)
- [ ] Recipe name matches page H1
- [ ] Image URL absolute and 1200×800+
- [ ] Author name present
- [ ] Minimum 2 ingredients listed
- [ ] Minimum 2 instruction steps (HowToStep format)
- [ ] prepTime in ISO 8601 (PT30M)
- [ ] aggregateRating if reviews exist

### AEO / AI Citability
- [ ] Statistics present (with source attribution)
- [ ] Ingredient quantities specific (not "some")
- [ ] Clear step sequence (numbered)
- [ ] Cuisine/region entity mentioned in intro
- [ ] Author credentials in bio (for E-E-A-T)

---

## Input

- Content draft or URL
- Target keywords (from OB1)
- SERP analysis (from OB3)

## Output

- Optimized content
- Meta title/description
- Header structure
- Internal link suggestions
- Schema recommendations
- AEO recommendations

## Integration

- Input from OB1 (keywords) and OB3 (SERP)
- Output → Elena for human voice editing (if needed)
- Schema → OB2 for implementation verification
- Reports to Wayne

---

*Wayne's Content Optimizer. SEO meets human readability. Free-tools-first.*

---

## Tool Access Checklist

- [ ] Hemingway Editor bookmarked and in use
- [ ] Yoast SEO installed on WordPress (free version)
- [ ] AnswerThePublic free tier activated
- [ ] Google Rich Results Test bookmarked
- [ ] searchsavvy.in bookmarked for schema generation
- [ ] NLP Bucket free tier activated