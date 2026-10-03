# clawperator.com

Preserved Clawperator landing site, extracted from `androperator/androperator`.

## Build and preview

Use Node.js 22 and npm:

```sh
npm ci
npm run build
npx serve out
```

Cloudflare Pages configuration: repository root, build command `npm ci && npm run build`, output directory `out`. Node.js version: 22.

`app/` contains authored pages; `public/` contains the preserved installer, agent guidance, documentation snapshot, sitemap files, headers, and redirects. The initial extraction preserves those files without regenerating documentation from Androperator. Sitemap files are tracked; update their URLs and timestamps deliberately when content changes.

Extraction provenance: source `sites/landing-clawperator/` in the Androperator repository. Git history remains available there. This repository begins with a content-preserving snapshot.

Deploy and verify a Pages preview before transferring `clawperator.com` and `www.clawperator.com`. Keep the existing `clawperator-preserved` project available for rollback. Remove the original site from Androperator only after the new deployment and both domains have been verified.
