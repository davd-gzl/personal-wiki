# Contributing to personal-wiki

This is a personal knowledge base. **PRs are not accepted**, but I welcome resource suggestions!

👉 [**Open an issue**](https://github.com/Davphla/personal-wiki/issues/new?title=Resource%20suggestion:&body=**URL:**%0A%0A**Category:**%0A%0A**Why%20it's%20interesting:**) to share knowledge!

---

## How This Wiki Works
*This section documents the organization for both humans and AI assistants.*

### Structure

```
README.md              # Main wiki with categorized resources
WHOAMI.md              # About me
blog/                  # Personal articles
  └── travel/          # Travel stories
awesome/               # Curated resource lists
  ├── digital-nomad.md # Remote work & travel resources
  └── offline-traveller.md # Offline-first apps
skills/                # Agent skills & capabilities
data/                  # Datasets & IPFS links
```

### Content Organization

#### Entry Format
All entries follow this pattern:
```markdown
- Title/Name - URL - Brief description
```

Keep descriptions **simple and concise** (one sentence or less).

#### Language Prefixes
Content in languages other than English uses flag emoji:
```markdown
- 🇫🇷 Title in French - URL - Description
```

#### Section Hierarchy
- `#` = Main categories (Documentations, Blogs, Videos, etc.)
- `##` = Subcategories (Blockchain, Cryptography, Programming)
- `###` = Specific topics (Consensus, Layer 2, Argon2)

### Ordering Rules

#### By Language
Within each section, entries are ordered:
1. English (no prefix)
2. French (🇫🇷)
3. Other languages

#### By Section Type
Different sections use different ordering:
- **Documentations**: By addition date (newest last)
- **Blogs, Videos, Youtube channels**: By preference
- **FOSS**: Categories alphabetically, entries by preference

### Table of Contents

The README has a **manual** Table of Contents that must be updated when sections change.

#### GitHub Anchor Link Format
- Spaces become hyphens: `Tech popularization` → `tech-popularization`
- Special characters removed, except emoji becomes `-`: `📌 Tech` → `-tech`
- Duplicate headings get numbered: `#blockchain`, `#blockchain-1`, `#blockchain-2`

**Example**: `## 📌 Tech popularization` → `#-tech-popularization`

### Content Categories

- **Documentations**: Technical documentation, tutorials, whitepapers, guides
- **Blogs**: Personal blogs and ongoing content series, organized by theme
- **Books**: Book recommendations with links to purchase/info pages
- **Videos**: Individual educational/informative videos (include creator)
- **Youtube channels**: Channel links, organized by content type/topic
- **FOSS**: Open source software projects (GitHub or repository links)
- **My Gears**: Physical products I use (with product page links)
- **Linux Setup**: Personal system configuration and preferences

### Adding New Content (For AI Assistants)

1. Determine the appropriate category
2. Use the standard entry format with a concise description
3. For new URLs, fetch the webpage to write an accurate description
4. Place entry respecting language and section-specific ordering
5. If creating a new section, update the Table of Contents with correct anchor
6. Keep FOSS categories in alphabetical order
