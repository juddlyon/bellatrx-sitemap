# BellatRx Sitemap Project

Interactive sitemap for BellatRx website redesign. Shared with client team.

## Live URL

https://bellatrx-sitemap.netlify.app

## Deployment

**DO NOT deploy without asking first.** This is shared with the client.

```bash
netlify deploy --prod --dir=.
```

## Source Documents

- `BellatRx-Website-Redesign-RFP-2026-02-Final.pdf` - Original RFP from client
- `Strategy & Messaging.md` - Strategy doc (post-RFP) defining visitor paths, messaging, success metrics

## Key Concepts

### Three Visitor Paths (from Strategy doc)

1. **Intent** - Ready to talk: book a call, request quote
2. **Interest** - Researching: playbooks, guides, nurture content
3. **Aftermarket** - Existing customers: parts, service, emergency support

### Big Idea

"Your Front of Line Starts Here" - distributed across product pages, not a single hub

### Success Metrics

- 30 MQLs/week
- 8 calls booked/week
- <15 min lead response time

## Site Structure

Single `index.html` with four tabs:

1. **Sitemap Tree** - D3.js interactive collapsible tree
2. **Page Types** - CMS template cards with slugs, Collection/Entry/Singleton badges
3. **User Paths** - Funnel visualization for Intent/Interest/Aftermarket visitors
4. **Current URLs** - Reference links to existing bellatrx.com pages

## Page Type Groups (color-coded)

- **Products** (blue): Product Finder, Product Category, Product Detail
- **Industries** (purple): Industries Overview, Industry Landing
- **Solutions** (cyan): Solutions Overview, Solution Detail, Luna Link
- **Aftermarket** (green): Aftermarket Hub, Aftermarket Service
- **Resources** (amber): Video Library, Brochures, Playbook/Guide, Case Studies, News & Events, Insights/Articles
- **Contact** (red): Book a Call, Request Quote, Contact Hub, Find a Rep, Campaign Landing
- **Company** (indigo): Company Hub, About, Careers, Partners/Agents, Privacy Policy

## URL Structure

Nested folder approach for clean IA:
- `/company/about/`, `/company/careers/`, `/company/partners/`, `/company/privacy/`
- `/contact/book-a-call/`, `/contact/request-quote/`, `/contact/find-a-rep/`
- `/resources/news/`, `/resources/insights/`, `/resources/videos/`, `/resources/brochures/`
- `/aftermarket/parts/`, `/aftermarket/service/`

## RFP Gaps (discussion items)

Items from RFP that need client clarification:
- Image Gallery / Library - separate from Video Library?
- Customer Logos Page - standalone or part of Testimonials?
- Testimonials vs Case Studies - same template or separate?

## Design Notes

- Colorblind-friendly: blue (#2563EB) for current, orange (#EA580C) for proposed
- No emojis per client preference
- Deploy timestamp in footer (greyed out)
