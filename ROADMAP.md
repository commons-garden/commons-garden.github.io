# commons.garden - Roadmap

> 🤖
>
> - [README](README.md) - Our project
> - [CHANGELOG](CHANGELOG.md) — What we did
> - [ROADMAP](ROADMAP.md) — What we wanna do
> - [POLICY](POLICY.md) — How we do it
> - [HEALTH](HEALTH.md) — What we accept
>
> 🤖

---

## v0.1.0 - Migration to GitHub Pages

⏳ Move from GitLab to GitHub and setup GitHub Pages deployment

**Problem:** Currently hosted on GitLab, want to migrate to GitHub Pages for better integration
**Solution:** Migrate repository, configure GitHub Actions for Hugo deployment, update DNS/settings

**Tasks:**

- [ ] Create new GitHub repository
- [ ] Migrate Git history from GitLab to GitHub
- [ ] Configure GitHub Pages settings
- [ ] Create GitHub Actions workflow for Hugo deployment
- [ ] Update baseURL in config.toml
- [ ] Test deployment on GitHub Pages
- [ ] Update DNS/domain settings (if needed)
- [ ] Update README with new repository URL
- [ ] Archive/redirect GitLab repository

---

## v0.2.0 - Information Consolidation | [research notes](epic-notes/v0.2.0.md)

⏳ Consolidate scattered information sources into single source of truth

**Problem:** Critical project info is dispersed across multiple platforms (HackMD, FigJam, Signal, GitLab issues)
**Solution:** Migrate/consolidate key documentation into this repo while maintaining external links where appropriate

**Research Finding:** Commons literature shows similar projects succeeded with clear governance but failed with fragmented communication. We're innovating in distribution but need formal structures.

**External sources currently in use:**
- HackMD: [@commonsgarden/roadmap](https://hackmd.io/@commonsgarden/roadmap), [@praxis/p2p-delete](https://hackmd.io/@praxis/p2p-delete), [@praxis/moderation](https://hackmd.io/@praxis/moderation), [@praxis/p2p-simulator](https://hackmd.io/@praxis/p2p-simulator), [@mixmix category/criteria](https://hackmd.io/@mixmix/rywE-3P1T/edit)
- FigJam boards: invite-driven onboarding, p2p-delete, identity-recovery, SSB-moderation, feature-backlog
- Signal groups: p2p-delete, moderation discussions
- GitLab issues: Manyverse features

**Tasks:**

- [ ] Audit all external links in content/
- [ ] Document which sources are canonical vs reference
- [ ] Migrate critical HackMD content to repo (or keep synced?)
- [ ] Add FigJam/external docs section to README
- [ ] Create decision: what stays external vs moves here
- [ ] Update gardener.json (currently just `"TODO": "CODE"`)
- [ ] Centralize or properly link Signal group decisions
- [ ] Consider: embed FigJam diagrams or screenshot + link?

---

## v0.3.0 - Strategic Vision

⏳ Define project direction and tooling decisions

**Problem:** Need to decide if Hugo is the right tool, or if we need volunteer ticketing system
**Solution:** Evaluate current needs, prototype volunteer ticketing concept, decide on architecture

**Tasks:**

- [ ] Document current use cases for commons.garden
- [ ] Define requirements for volunteer ticketing system
- [ ] Evaluate: Hugo + plugin vs separate app vs hybrid
- [ ] Create mockups/wireframes for ticketing features
- [ ] Prototype volunteer ticket workflow
- [ ] Decision: Keep Hugo, extend it, or build separate tool?
- [ ] Document architecture decision in CHANGELOG

**Questions to explore:**
- What features does volunteer ticketing need?
- Can Hugo + custom shortcodes/data files handle it?
- Or do we need a dynamic app (React/Next.js/etc)?
- Integration: Separate tool that reads from Hugo data?

---

## v0.4.0 - Content & Features (from agenda.md)

⏳ Implement pending content and Hugo improvements

**Content tasks:**
- [ ] Document p2p-delete 📌
- [ ] Update initiatives Michael wants to facilitate
- [ ] Define needs and next steps for initiatives
- [ ] Add "needs" tags (resources, skillset, etc)
- [ ] Add "type" tags (language, wireframe)
- [ ] 2 emoji per initiative/spec
- [ ] List volunteer types
- [ ] Redirect policy template: `p2p-delete` → `p2p_delete`

**Hugo improvements:**
- [ ] Map category diagram into Hugo ([diagram](https://hackmd.io/@mixmix/rywE-3P1T/edit))
- [ ] Merge wireframe into spec + type
- [ ] Implement subpages functionality
  - [ ] Page template checks if slug has folder
  - [ ] Lists all public pages alphabetically in TOC
  - [ ] Folder pages point to original page
  - [ ] Update list.html template for subgroups

**Show-and-tell features:**
- [ ] Event category
- [ ] Phases concept (leads, accepted, scheduled)
- [ ] Past/upcoming events view
- [ ] Podcast integration?
- [ ] .ics calendar automation
- [ ] Show time in local timezone
- [ ] Social media integrations (Mastodon, YouTube?)

---

## Backlog (Phase 3 - Future Ideas)

**Community & Process:**
- Find facilitators
- Facilitate for facilitators
- Volunteer rotation
- Volunteer onboarding automation
- Improved gardener/contributor workflows

**Content & Tools:**
- Members category
- Organizations category (✅ exists, needs completion)
- Wire categories across
- Manual category (templates, criteria, etc)
- Glossary / living documentation (Airtable?)
- Donation platform (Open Collective?)
- Announcements system (newsletter? Telegram?)

**Technical:**
- Analytics for commons projects
- Multi-language support
- Integration with SSB/Scuttlebutt ecosystem tools

**Initiatives backlog:**
- Multi-device (fusion identity)
- Dying online
- Stencil
