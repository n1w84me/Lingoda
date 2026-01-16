# Lingoda Project Instructions for GitHub Copilot

## Tech Context
- **Framework:** Google Blogger (Blogspot) XML Theme Engine.
- **Syntax:** XHTML 1.0 Strict (XML-compliant HTML).
- **Core Files:** `theme.xml` is the primary entry point.

## Blogger Skin & Variables
- When editing CSS inside `<b:skin>`, use Blogger variables syntax: `$(variable.name)`.
- Variable definitions follow this format: `<Variable name="key" description="desc" type="color" default="#fff" value="#fff"/>`.
- Groups are used to categorize variables in the Blogger Theme Designer: `<Group description="Name" selector=".class">`.

## XML Logic Rules
- Always use the `b:`, `data:`, and `expr:` namespaces.
- Favor `expr:attribute` for dynamic values (e.g., `<div expr:class='data:post.class'>`).
- Use `<b:includable>` and `<b:include>` for modularizing widget code.

## Code Quality
- All tags MUST be self-closed: `<br />`, `<hr />`, `<img ... />`.
- Wrap all JavaScript in CDATA blocks: `//<![CDATA[ ... //]]>`.
- Use 2-space indentation to keep the 3,500+ line XML file readable.
