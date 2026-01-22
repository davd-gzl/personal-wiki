# Contributing to personal-wiki

This is a personal knowledge base. **Direct contributions are not accepted**, but I welcome suggestions! 

If you'd like to share knowledge or recommend resources, please [open an issue](https://github.com/Davphla/personal-wiki/issues). I appreciate any interesting links, corrections, or ideas.

---

**The rest of this document is primarily for AI coding assistants** to understand how this wiki is organized and maintained.

## Structure

```
README.md          # Main wiki with categorized links
blog/README.md     # Personal writing/articles (WIP)
```

## Content Format

### Entry Format
All links follow this pattern:
```markdown
- Title/Name - URL - Optional description
```

For content in other languages, prefix with flag emoji:
```markdown
- 🇫🇷 French content title - URL - description
```

### Hierarchy
- `#` Top-level categories (Documentations, Books, Videos, etc.)
- `##` Subcategories (Blockchain, Cryptography, Programming)
- `###` Further nesting as needed (Consensus, Layer 2, Algorithm)

## Ordering Conventions

### Language Order
Within each section, entries are ordered by language:
1. English (no prefix)
2. French (🇫🇷)
3. Other languages

### Section-Specific Order
- **Documentations**: By addition date
- **Blogs, Videos, Youtube channels**: By preference
- **FOSS**: Alphabetically by category name

## Table of Contents

The README contains a **manual** Table of Contents at the top. **Always update it** when adding/removing/renaming sections.

### GitHub Anchor Link Rules
- Spaces → hyphens
- Special characters removed (except emoji which uses `-`)
- Duplicate headings get `-1`, `-2` suffix

Example: `## 📌 Tech popularization` → `#-tech-popularization`

## Adding New Content

1. Find the appropriate category (or create one if needed)
2. Add the entry using the standard format
3. For URLs, include a short description (keep it simple and concise)
4. If adding a new section, update the Table of Contents
5. Maintain the language and section-specific ordering

## Content Categories

- **Documentations**: Technical docs, tutorials, whitepapers
- **Blogs**: Personal blogs with ongoing content, organized by theme
- **Books**: Book recommendations with purchase links
- **Videos**: Individual video links (include creator name)
- **Youtube channels**: Channel links organized by topic
- **FOSS**: Open source software with GitHub/repository links
- **My Gears**: Physical products with product page links
- **Linux Setup**: Personal system configuration
