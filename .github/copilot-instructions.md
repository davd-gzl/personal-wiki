# Copilot Instructions for personal-wiki

## Project Overview
A personal knowledge base/wiki containing curated links, resources, and notes organized by topic. Pure markdown, no build system.

## Structure
```
README.md          # Main wiki with categorized links
blog/README.md     # Personal writing/articles (WIP)
```

## Content Conventions

### Entry Format
Links follow this pattern:
```markdown
- Title/Name - URL - Optional description
```

For items in other languages, prefix with flag emoji:
```markdown
- 🇫🇷 French content title - URL - description
```

### Hierarchy
- `#` Top-level categories (Documentations, Books, Videos, etc.)
- `##` Subcategories (Blockchain, Cryptography, Programming)
- `###` Further nesting as needed (Gno.land, Layer 2, Algorithm)

### Table of Contents
The README contains a manual Table of Contents at the top. **Always update it** when adding/removing/renaming sections. Use GitHub-compatible anchor links:
- Spaces → hyphens
- Special chars removed (except for emoji which uses `-`)
- Duplicate headings get `-1`, `-2` suffix

Example: `## 📌 Tech popularization` → `#-tech-popularization`

## When Adding New Content
1. Find the appropriate category (or create one if needed)
2. Add the entry using the standard format
3. If adding a new section, update the Table of Contents
4. When asked to add a URL, fetch the webpage to generate a meaningful description

## Content Categories
- **Documentations**: Technical docs, tutorials, whitepapers
- **Blogs**: Personal blogs with ongoing content
- **Books**: Book recommendations with purchase links
- **Videos**: Individual video links (include creator name)
- **Youtube channels**: Channel links organized by topic
- **FOSS**: Open source software with GitHub links
- **My Gears**: Physical products with product page links
- **Linux Setup**: Personal system configuration
