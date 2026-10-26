# Software Cost & Value

A single-page public research library covering industry software prices, corporate purchases, and investments in software companies.

Expected project-site URL: https://airxcy.github.io/software-costs/

The local directory name `software-value` does not change the repository name or Pages URL. The configured remote is `airxcy/software-costs`.

## Contents

- 162 base research records: 90 software/configuration records and 72 corporate records.
- 63 priced configurations, 24 unpriced products, and 3 mixed procurement contexts within the price research.
- 9 investment and acquisition records, including the completed Synopsys acquisition of Ansys.
- 16 derived scenarios for 100 and 1,000 full paid users.
- Historical accounting subtotals retained as context within related purchase records.
- 163 external source pages, including Chinese-name references, and the original methodology notes.
- 49 records with verified Chinese names and source wording beside the English labels.

The five-year amounts retain their evidence type: known-fee scenario, actual contract, conditional service renewal, ceiling, or historical accounting subtotal. Acquisition consideration is not a software license price or five-year usage cost.

Chinese names from source material are displayed beside the English labels in tables, buyer filters, record details and the source library. The record details retain the precise buyer, supplier, project and source names when verified. Naming notes distinguish original wording, descriptive Chinese labels and legal entities that the cited evidence does not identify. Name-verification references are separate from evidence for transaction amounts. Both Chinese and English names can be searched.

## Publish with GitHub Pages

1. Review the pending changes. The repository already contained deleted working-data files before this site was prepared; the deployment preserves those deletions.
2. Commit the intended changes and push to `main` when ready.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**.
5. Save and wait for GitHub to report the deployment URL.

`index.html` contains its styles, scripts and public research data. No package installation, build service, external font, CDN, API key or separate JSON file is needed. `.nojekyll` marks the output as a plain static site. All research citations use external URLs; local PDFs are not required.

This preparation does not commit, push, configure the remote repository, or publish the site.

## Public data and private working material

The publication boundary is:

```text
Private working area / separate research repository
  original PDFs, source snapshots, intermediate JSON
  build scripts, templates, extraction and verification artifacts
             |
             | local build: select public fields and remove local paths
             v
Public website repository
  index.html  (public summaries, amounts, notes, citations)
  README.md, LICENSE, .nojekyll, .gitignore
```

Original reports and working data remain in a separate research workspace outside this website directory. Its generator is `build-index.mjs`. Run the generator in that private workspace and copy only the resulting `site/index.html` into this repository for later content updates.

There is no requirement to publish separate JSON datasets. However, the public fields embedded in `index.html` can be read, copied and extracted by visitors. Moving the same data to JavaScript, a different public repository or a public API does not make it confidential. Publish only information intended for public access.

To keep the complete raw dataset private while automating updates, use a private research/build repository or local build process and publish only the reviewed static artifact. GitHub Pages custom workflows can deploy a selected output directory. A private source repository does not, by itself, make its Pages website private.

If actual visitor-specific access restrictions are required, use a server with authentication and authorization, or an eligible GitHub Enterprise Cloud private project site. Ordinary public GitHub Pages cannot hide data already sent to the browser. Never embed a credential to a private data store in this page.

## Git history caveat

`.gitignore` limits accidental addition of new working files. It does not untrack existing files, remove prior commits, or make an already published dataset private. The old JSON/build files were tracked in this repository before consolidation. Their working-tree deletion is preserved, but their historical versions may remain in Git commits and any previously published copies.

No history rewrite was performed. If old research data must be removed from Git history, that requires a separate, deliberate history-cleanup decision and coordination with existing clones; it cannot retract copies already downloaded by others.

## Official publishing references

- [Configure a GitHub Pages publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Deploy a selected artifact using a custom Pages workflow](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages)
- [GitHub Enterprise Cloud project-site access control](https://docs.github.com/en/enterprise-cloud@latest/pages/getting-started-with-github-pages/changing-the-visibility-of-your-github-pages-site)

## License

The existing dual license is retained:

- **Code and rendering templates:** [MIT License](./LICENSE).
- **Curated report content and public research data:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (attribution required).

External cited publications remain subject to their respective owners' terms; this repository publishes curated facts and summaries with links rather than copies of the source documents.

Research date: 26 October 2026. FX snapshot: 23 October 2026. Prices and fees are point-in-time references, with scope and exclusions retained in each record; they are not vendor quotations or complete deployment budgets.

The [Chinese Markdown tables](software-costs-zh.md) provide a static companion covering all 162 base records and 16 user-scale scenarios, with historical subtotals in the related record notes. They cite the published website as their consolidated source.
