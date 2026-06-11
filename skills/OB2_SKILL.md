# OB2 SKILL — Technical SEO Agent

Handles all technical SEO aspects.

## What OB2 Does

- Core Web Vitals audits (LCP, INP, CLS)
- Crawlability checks
- Schema markup implementation
- Site speed optimization
- Mobile-friendliness verification
- XML sitemap validation
- robots.txt analysis

---

## Free Tools in OB2's Workflow

### Primary Tools

| Tool | Use | Access |
|------|-----|--------|
| **Google PageSpeed Insights** | LCP, INP, CLS scores + field data from CrUX. Free, no account needed. | [pagespeed.web.dev](https://pagespeed.web.dev) |
| **Google Search Console** | Index coverage, Core Web Vitals reports, crawl errors, schema issues | [search.google.com/search-console](https://search.google.com/search-console) |
| **Screaming Frog SEO Spider** | Crawl up to 500 URLs free. Find broken links, missing meta, redirect chains. | [screamingfrog.co.uk](https://www.screamingfrog.co.uk/seo-spider) |
| **Google Rich Results Test** | Validate recipe schema (JSON-LD) before publishing | [search.google.com/test/rich-results](https://search.google.com/test/rich-results) |
| **searchsavvy.in** | Free recipe schema generator — full field support, no signup | [searchsavvy.in/recipe-schema-generator](https://searchsavvy.in/recipe-schema-generator) |
| **searchbulb.com** | Free recipe schema generator — ingredients, steps, nutrition, timing | [searchbulb.com/tools/schema-markup-generator/recipe](https://searchbulb.com/tools/schema-markup-generator/recipe) |

### Usage Notes

- **Core Web Vitals:** Target LCP < 2.5s, INP < 200ms, CLS < 0.1
- **Schema:** Always test output in Google Rich Results Test before deploying
- **Screaming Frog:** Run weekly crawl to catch new issues

---

## OB2 Workflow

### Step 1: Core Web Vitals Audit
- Run Google PageSpeed Insights on crispyglaze.com homepage + top 5 recipe pages
- Record LCP, INP, CLS scores
- Flag any pages below threshold
- Check mobile vs desktop split

### Step 2: Google Search Console Review
- Check Coverage report → fix any Excluded pages (404s, canonical issues)
- Check Core Web Vitals report → identify failing pages
- Check Enhancements report → validate schema status

### Step 3: Crawl with Screaming Frog
- Set crawl limit to 500 URLs (free tier max)
- Run spider on crispyglaze.com
- Export: Broken links, Missing meta titles, Redirect chains, Missing h1
- Prioritize: Critical > High > Medium

### Step 4: Schema Markup Audit
- For each recipe page: use searchsavvy.in to generate Recipe JSON-LD
- Test in Google Rich Results Test
- Validate: name, image, author, ingredients (min 2), instructions (min 2), prepTime
- Check for: aggregateRating, nutrition, recipeCategory, keywords

### Step 5: Mobile & Accessibility
- Google PageSpeed Insights mobile tab → check tap targets and viewport
- Check robots.txt isn't blocking Googlebot
- Check XML sitemap is accessible and updated

### Step 6: Deliver Output
- Technical audit report per page
- Issue list: Issue | Page | Severity | Fix (with code if needed)
- Schema markup code (ready to paste)
- Re-audit checklist for next cycle

---

## Technical Issue Fix Priorities

| Severity | Issue Types | Response |
|----------|-------------|----------|
| Critical | Core Web Vitals failing, canonical issues, schema errors causing rich result loss | Fix within 48h |
| High | Broken links, missing meta titles, slow LCP (4s+) | Fix within 1 week |
| Medium | Missing alt text, minor schema improvements | Fix in next content cycle |

---

## Schema Quick Reference

### Recipe Schema Required Fields
- `@type: "Recipe"`
- `name` — recipe title
- `image` — URL, minimum 1200×800px
- `author` — name or organization
- `recipeIngredient` — minimum 2 ingredients
- `recipeInstructions` — minimum 2 steps (use `HowToStep`)
- `prepTime` / `cookTime` / `totalTime` — ISO 8601 format (PT30M)

### Recommended Fields (boosts rich results)
- `aggregateRating` — star rating with count
- `nutrition` — calories per serving
- `recipeCategory`, `recipeCuisine`, `keywords`
- `video` — if recipe has video content

### ISO 8601 Duration Format
- 30 minutes = PT30M
- 1 hour = PT1H
- 1 hour 15 minutes = PT1H15M

---

## Input

- Website URL
- Technical focus area

## Output

- Technical audit report
- Issue prioritized list
- Fix recommendations with code

## Integration

- Issues found → Tracked for fix
- Fixes applied → Re-audit
- Schema output → OB4 for content integration
- Reports to Wayne for quality gate

---

*Wayne's Technical SEO Agent. Core Web Vitals and site health. Free-tools-first.*

---

## Tool Access Checklist

- [ ] Google Search Console verified for crispyglaze.com
- [ ] Screaming Frog installed (free version)
- [ ] searchsavvy.in bookmarked for schema generation
- [ ] searchbulb.com bookmarked for schema validation
- [ ] PageSpeed Insights bookmarked