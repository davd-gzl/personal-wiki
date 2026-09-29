# Agent Rules

Rules and structure documentation for AI assistants working on this wiki.

---

## How This Wiki Works

### Structure

```
README.md                # Main wiki with categorized resources
WHOAMI.md                # About me
CONTRIBUTING.md          # Human contribution guide
AGENT.md                 # This file — AI assistant rules
awesome/                 # Curated resource lists
  ├── digital-nomad.md   # Remote work & travel resources
  └── offline-traveller.md # Offline-first apps
blog/                    # Personal articles
  └── travel/            # Travel stories
data/                    # Datasets & IPFS links
skills/                  # Agent skills & capabilities
  └── README.md          # Skills documentation + Copilot instructions
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
- `#` = Main categories (Blogs, Books, Documentations, Films, FOSS, Games, etc.)
- `##` = Subcategories (Blockchain, Cryptography, Programming)
- `###` = Specific topics (Consensus, Layer 2, Argon2)
- The last level is always the **year of addition**, one below the deepest
  heading that holds entries

### Ordering Rules

#### Global
All main sections (`#`) and subsections (`##`, `###`) are in **alphabetical order**.
Year headings are the exception: they are ordered by year, newest first.

#### By Addition Year
Every entry sits under the year it was added, one level below the deepest
heading that holds entries. Only the current year is a heading. Every earlier
year folds into a collapsed block below it, one per year, newest first, so old
entries take one line until opened. `markdown="1"` makes Jekyll render the list
inside; the blank lines do the same on GitHub:

```markdown
## Cyber-security
### 2027
- Newer entry - URL - Description

<details markdown="1">
<summary>2026</summary>

- Older entry - URL - Description

</details>
```

Under `### Algorithm` the year heading is a `####`, and under a `#` with no
subsection it is a `##`. A section with no entry from the current year keeps
only its blocks. When the year turns, the previous year's heading becomes such a
block.

Within a year, the section's own rule below applies unchanged.

#### By Language
Within each section, entries are ordered:
1. English (no prefix)
2. French (🇫🇷)
3. Other languages

#### By Section Type
- **Documentations**: By addition date within the year (newest last)
- **Blogs, Videos, Youtube channels**: By preference
- **FOSS**: Alphabetically

### Table of Contents

The README has a **manual** Table of Contents that must be updated when sections change.
Year headings are **not** listed in it.

#### GitHub Anchor Link Format
- Spaces become hyphens: `Tech popularization` → `tech-popularization`
- Special characters removed, except emoji becomes `-`: `📌 Tech` → `-tech`
- Duplicate headings get numbered: `#blockchain`, `#blockchain-1`, `#blockchain-2`

**Example**: `## 📌 Tech popularization` → `#-tech-popularization`

### Content Categories

- **Blogs**: Ongoing blog websites you follow (recurring content sources)
- **Books**: Book recommendations with links to purchase/info pages
- **Documentations**: Individual articles, guides, whitepapers, tutorials (one-off reads)
- **Films**: Film recommendations
- **FOSS**: Open source software projects (GitHub or repository links)
- **Games**: Web games and interactive tools
- **Linux Setup**: Personal system configuration and preferences
- **My Gears**: Physical products I use (with product page links)
- **Videos**: Individual educational/informative videos (include creator)
- **Youtube channels**: Channel links, organized by content type/topic

### Adding New Content

1. Determine the appropriate category
2. Use the standard entry format with a concise description
3. For new URLs, fetch the webpage to write an accurate description
4. Place the entry under the current year's heading, creating that heading above
   the older years' collapsed blocks if it does not exist yet
5. Within the year, respect alphabetical order and language ordering
6. If creating a new section, update the Table of Contents with correct anchor
7. Keep all sections in alphabetical order

---

## Formatting Rules

### Videos section — link format

Use **single brackets** for the link label and always add a **dash separator** before it:

```markdown
- Title - [link](https://...) - Author
- Title - [YouTube](https://...) - Author
```

Do **not** use double brackets (`[[link]]` or `[[YouTube]]`).
