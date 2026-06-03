# Attribution

The **`kickoff`** skill in this plugin is the **`brainstorming`** skill from
[Superpowers](https://github.com/obra/superpowers) by Jesse Vincent, used **verbatim** under
the MIT License. The only changes are the two forced by repackaging:

- the frontmatter `name:` is `kickoff` (not `brainstorming`), to avoid a skill-name collision
  when Superpowers is also installed, and
- the skill's single reference to its own visual-companion path points to `skills/kickoff/`
  instead of `skills/brainstorming/`.

The methodology — every other line — is unchanged. The following files under
`skills/kickoff/` are also copied from Superpowers unmodified:

- `skills/kickoff/visual-companion.md`
- `skills/kickoff/spec-document-reviewer-prompt.md`
- `skills/kickoff/scripts/` (the visual-companion server and helpers)

The **`approved-tools`** skill and the registers in `skills/approved-tools/references/`
(`approved-tools.md`, `github-rules.md`) are Calo's own work, not from Superpowers.

## Upstream license

```
MIT License

Copyright (c) 2025 Jesse Vincent

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
