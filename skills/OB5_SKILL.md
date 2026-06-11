# OB5 SKILL — GEO Agent

Generative Engine Optimization. Optimizes for AI search visibility.

## What OB5 Does

- AI search visibility optimization (ChatGPT, Perplexity, Claude, Gemini)
- llms.txt generation and maintenance
- AI schema markup (FAQPage, Article, Organization)
- Structured data for AI parsing
- Source citation optimization
- GEO metrics tracking (manual + free tools)

## AI Platforms Tracked

- ChatGPT (800M+ weekly users)
- Perplexity AI (780M+ monthly queries)
- Google AI Overviews (60%+ of searches)
- Claude
- Gemini
- Any new AI search platforms

---

## Free Tools in OB5's Workflow

### Primary Tools

| Tool | Use | Access |
|------|-----|--------|
| **Google Search Console** | Baseline — track branded search traffic as proxy for AI citation lift | [search.google.com/search-console](https://search.google.com/search-console) |
| **Perplexity AI** (manual) | Query target keywords monthly, record whether crispyglaze.com is cited | [perplexity.ai](https://perplexity.ai) |
| **ChatGPT** (manual) | Query target keywords monthly, record brand mentions | [chatgpt.com](https://chatgpt.com) |
| **HubSpot AI Search Grader** | Free tier — analyze content's AI search performance + baseline score | [hubspot.com/ai-search-grader](https://www.hubspot.com/ai-search-grader) |
| **Google Rich Results Test** | Validate schema markup — foundation for AI citation | [search.google.com/test/rich-results](https://search.google.com/test/rich-results) |
| **searchsavvy.in** | Generate FAQPage + Article schema markup | [searchsavvy.in/recipe-schema-generator](https://searchsavvy.in/recipe-schema-generator) |

### No-Cost GEO Strategies

Research shows these tactics boost AI visibility 30–40%:
- **Statistics Addition:** Add real numbers to content (e.g., "4.2 stars from 1,847 reviews")
- **Cite Sources:** Link to authoritative sources with clear attribution
- **Quotation Addition:** Include expert quotes with name/title
- **Clear structure:** Use H2s, bullet lists, numbered steps — AI parses these easily
- **Entity clarity:** Mention cuisine type, region, ingredient names explicitly

### Manual Tracking (Monthly)

1. Open Perplexity → search "cucumber soy sauce salad recipe"
2. Open ChatGPT → same query
3. Note: Is crispyglaze.com cited? In what context?
4. Log results in GEO tracking sheet

---

## OB5 Workflow

### Step 1: Schema Foundation
- Audit all recipe pages for Recipe schema (via Google Rich Results Test)
- Add FAQPage schema to all articles with FAQ sections
- Add Article schema to all long-form content (author, date, credentials)
- Add Organization schema to homepage and About page

### Step 2: Content GEO Audit
- Review content for AI citability signals:
  - Statistics present (with numbers, not vague claims)
  - Expert attribution (author name, credentials in bio)
  - Clear ingredient lists with quantities
  - Step-by-step format (numbered, not prose)
  - Cuisine/region entity in title/intro
- Flag pages missing these signals → recommend to OB4

### Step 3: Citation Optimization
- Add statistics to recipe intros: "Named best cucumber salad by X readers"
- Add quotation blocks: "The key is cold cucumbers — says Chef Ken"
- Add authoritative outbound links with context
- Structure: H2 for ingredients, numbered list for steps, bullet for tips

### Step 4: GEO Baseline (HubSpot AI Search Grader)
- Run HubSpot AI Search Grader on crispyglaze.com
- Record baseline score and recommendations
- Re-run monthly to track improvement

### Step 5: Manual Citation Tracking
- Create spreadsheet: Keyword | Platform | Date | Cited (Y/N) | Context
- Query top 10 target keywords in Perplexity + ChatGPT monthly
- Log whether crispyglaze.com appears and in what context
- Track trends: Are citations growing?

### Step 6: llms.txt Maintenance
- Create/update llms.txt file in site root
- Include: Site purpose, key content sections, brand voice, contact info
- Update quarterly or when major content added
- Reference: [mongodb.com/learn/infrastructure/llms-faq](https://www.mongodb.com/learn/infrastructure/llms-faq) for format guidance

### Step 7: Deliver Output
- GEO audit report per page
- Schema markup code (FAQPage, Article, Organization)
- Citation tracking spreadsheet
- Monthly AI platform performance summary

---

## Schema Types for GEO

### FAQPage Schema (Required for Articles with FAQs)
```json
{
  "@type": "FAQPage",
  "mainEntity": [{
    "@type": "Question",
    "name": "Question text here?",
    "acceptedAnswer": {
      "@type": "Answer",
      "text": "Answer text here."
    }
  }]
}
```

### Article Schema (Required for Long-Form Content)
```json
{
  "@type": "Article",
  "headline": "Article title",
  "author": { "@type": "Person", "name": "Author Name" },
  "datePublished": "2026-05-25",
  "publisher": { "@type": "Organization", "name": "CrispyGlaze" }
}
```

### Organization Schema (Homepage)
```json
{
  "@type": "Organization",
  "name": "CrispyGlaze",
  "url": "https://crispyglaze.com",
  "logo": "https://crispyglaze.com/logo.png",
  "sameAs": ["https://pinterest.com/crispyglaze", "https://instagram.com/crispyglaze"]
}
```

---

## GEO Metrics to Track

| Metric | Tool/Method | Frequency |
|--------|-------------|-----------|
| AI citation rate | Manual Perplexity + ChatGPT queries | Monthly |
| Branded search lift | Google Search Console | Monthly |
| AI Search Grader score | HubSpot AI Search Grader (free) | Monthly |
| Rich result eligibility | Google Rich Results Test | Per page publish |
| Schema errors | Google Search Console Enhancement report | Weekly |

---

## Input

- Website URL
- Content to optimize
- Target AI platforms

## Output

- llms.txt file
- AI schema markup (FAQPage, Article, Organization)
- Content restructuring recommendations
- Citation tracking spreadsheet
- Monthly GEO performance report

## Integration

- Schema → OB2 for implementation
- Content restructuring → OB4
- Reports to Wayne on AI visibility trends

---

*Wayne's GEO Agent. Optimizes for the AI search future. Free-tools-first.*

---

## Tool Access Checklist

- [ ] Google Search Console verified for crispyglaze.com
- [ ] HubSpot AI Search Grader free account created
- [ ] Perplexity account (free)
- [ ] ChatGPT account (free)
- [ ] GEO tracking spreadsheet created
- [ ] llms.txt file created in site root
- [ ] FAQPage schema deployed on top 10 pages