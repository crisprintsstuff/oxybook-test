# oxybook-test

Test repository for [OxyBook](https://github.com/crisprintsstuff/OxyBook). It is the M1 test space (see OxyBook `docs/M1-PLAN.md`) and is used for any other live test.

`docs/` is the content root. The tree is small on purpose, and each page exercises something:

| Path | What it exercises |
| --- | --- |
| `oxybook.yml` | space config, import mapping for `@theme/Tabs` |
| `docs/_dir.yml`, `docs/*/_dir.yml` | sidebar titles and order |
| `docs/index.md` | home page, container-directive callout |
| `docs/getting-started.md` | `nav_title`, GitHub alert, relative link |
| `docs/guides/index.mdx` | directory page in MDX, `<Card>` |
| `docs/guides/install.md` | code block, table, image asset, titled callout |
| `docs/guides/configure.mdx` | imports, `<Tabs>`, an expression, an unknown component, an MDX comment, one broken link on purpose |
| `docs/reference/environment.md` | `slug` override |
| `docs/reference/internal-notes.md` | `hidden: true` |
| `docs/_partials/` | never a page |
| `docs/test-page.md`, `docs/test-page-2.md` | earlier test files, kept |

The broken link in `configure.mdx` (to `reference/settings.md`) is intentional: the build should warn about it.
