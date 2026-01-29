# commons.garden - Health Checks

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

> 🌟
>
> This project follows the [global backstage HEALTH](global/HEALTH.md)
> Do write all tests here as explained below
> [/backstage-start](.github/prompts/backstage-start.prompt.md) trigger tests
> For more policies, see [POLICY.md](POLICY.md)
>
> 🌟

### Test: Hugo Installation

```bash
hugo version
```

Expected: Hugo version should be installed
Pass: ✅ Command returns version number

---

### Test: Hugo Build

```bash
cd "/Users/nfrota/Documents/commons garden" && hugo --quiet
```

Expected: Site builds without errors
Pass: ✅ Exit code 0, public/ directory created

---

### Test: Hugo Server (Development)

```bash
cd "/Users/nfrota/Documents/commons garden" && timeout 3 hugo server -D --quiet || test $? -eq 124
```

Expected: Hugo dev server starts (timeout is expected)
Pass: ✅ Server starts on http://localhost:1313

---

### Test: Required Directories Exist

```bash
cd "/Users/nfrota/Documents/commons garden" && test -d content && test -d layouts && test -d static && echo "✅ All required directories exist"
```

Expected: Core Hugo directories present
Pass: ✅ content/, layouts/, static/ all exist

---

### Test: Config File Valid

```bash
cd "/Users/nfrota/Documents/commons garden" && test -f config.toml && hugo config | head -3
```

Expected: config.toml exists and is parseable
Pass: ✅ Hugo can read configuration

---

## Summary

**Project-specific checks ensure:**

- ✅ Hugo is installed and working
- ✅ Site builds successfully
- ✅ Dev server can start
- ✅ Required directory structure intact
- ✅ Configuration is valid

Before pushing, all checks must pass to ensure site integrity.
