# AGENTS.md - Instructions for AI Coding Agents

## Project Overview
- **Name:** Lingoda
- **Type:** Blogger (Google) Custom Theme
- **Stack:** XHTML 1.0 Strict, CSS3 (Blogger Skin), XML (Blogger Data Tags)
- **Goal:** A clean, optimized Blogger theme focused on readability.

## Core Rules & Constraints
- **Strict Compliance:** All code MUST be XHTML 1.0 Strict compliant. 
- **Blogger Namespaces:** Use `b:`, `data:`, and `expr:` namespaces correctly. 
- **Self-Closing Tags:** Ensure all tags (like `<img>`, `<br>`, `<input>`) are self-closed (e.g., `<br />`).
- **No Unescaped JS:** JavaScript within XML must be wrapped in `//<![CDATA[` ... `//]]>` blocks.

## Naming Conventions
- **Blogger Widgets:** Use descriptive IDs (e.g., `id='Header1'`, `id='Blog1'`).
- **CSS Variables:** Use the `variable` format inside `<b:skin>` for the Blogger Theme Designer.

## Testing Instructions
- **Validation:** Run `xmllint --noout theme.xml` before proposing changes.
- **Manual Verification:** Changes must be tested by uploading to a Blogger test blog.

## AI Boundaries
- **NEVER** remove the `<b:section>` or `<b:widget>` structure unless explicitly asked.
- **NEVER** replace Blogger-specific data tags with hardcoded text.
