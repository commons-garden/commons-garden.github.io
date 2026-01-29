# commons.garden - Changelog

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

## v0.0.2 - 2026-01-29

### Fixed Hugo Build Error

**Problem:** Site wouldn't build due to deprecated `resources.ToCSS` function (removed in Hugo v0.128.0)
**Solution:** Updated to use `css.Sass` instead

**Changes:**
- Updated [layouts/partials/head.html](layouts/partials/head.html)
- Updated [layouts/_default/baseof.html](layouts/_default/baseof.html)
- ✅ Hugo now builds successfully

### Added MGMT Framework

**Problem:** No structured project management or status tracking
**Solution:** Implemented backstage MGMT framework

**Changes:**
- Created ROADMAP.md with migration plan and strategic vision
- Created CHANGELOG.md (this file)
- Created HEALTH.md with Hugo-specific tests
- Created POLICY.md for workflow rules
- Added 🤖 navigation block to README.md

---

## v0.0.1 - Phase 1 Complete (2023)

### Initial Platform Setup ✅

**Completed features:**
- ✅ Specs category
- ✅ About category
- ✅ Initiatives category
- ✅ Wireframes category

**Infrastructure:**
- ✅ Hugo site setup
- ✅ GitLab CI/CD deployment
- ✅ Custom layouts and templates
- ✅ Bootstrap + custom CSS
- ✅ Content organization structure

**Active initiatives documented:**
1. Invite-driven onboarding ([FigJam](https://www.figma.com/file/eG3RjraaGHIdv1nuUp667J/Invite-driven-onboarding))
2. P2P delete ([FigJam](https://www.figma.com/file/a3MVrJ2Z8UDILkHK0NUeYb/p2p-delete), [HackMD](https://hackmd.io/@praxis/p2p-delete))
3. Identity recovery ([FigJam](https://www.figma.com/file/Qkei1VgElbho66UinY9MzH/identity-recovery))
4. SSB moderation ([FigJam](https://www.figma.com/file/C9YFMDwsOIXbmt88QoxL2B/SSB-moderation), [HackMD](https://hackmd.io/@praxis/moderation))
5. Feature backlog ([FigJam](https://www.figma.com/file/UIQDqYS48Pkg0ARSY9Rpf4/feature-backlog))

**Recent content updates (Jan 2026):**
- redirect functionality
- knowledge sharing content
- simulator initiative
- links updates
- empowerment content

---

_See [ROADMAP](ROADMAP.md) for planned features and ongoing work_
