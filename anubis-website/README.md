# ANUBIS website recovery and deployment preparation

Recovered on October 25, 2026 from https://anubis-audio.pages.dev/.
This is the served static website, not a claim to have recovered an original authoring project or private build configuration.

## Files

- `site/`: deployable static site with SEO improvements.
- `original-live-backup/`: unchanged served HTML, CSS, JavaScript, and image.

## Verified current state

- ANUBIS-Website initially contained only README.md.
- Cloudflare project: anubis-audio; production hostname: anubis-audio.pages.dev.
- Cloudflare currently points at meredithc050-cmd/ANKH, production branch main, automatic deployments enabled.
- ANKH contains only README.md and .gitattributes, not the served website.
- Current production deployment: c2f2a417-26eb-41a9-8e31-4d33e9ff7b2a; previous deployment: 36633af0-8835-46de-a194-7cc8e0654152.
- No environment variables or resource bindings were shown in project settings.

## SEO prepared

Descriptive search title, canonical URL, Open Graph and Twitter metadata, SoftwareApplication structured data with factual free pricing, robots.txt, and a one-page sitemap. Anchor sections are not separate sitemap pages. Existing description, design, text, and installer links are preserved. No ratings, reviews, or unverified platform support are claimed.

## Safe deployment integration

1. Review and merge the recovery branch into ANUBIS-Website only after checking the preview.
2. Keep the current Pages project and its deployments intact. Do not click retry on the ANKH-based build or push website files to ANKH.
3. Before reconnecting, record production and previous deployment IDs above and verify that rollback remains available.
4. In the existing project's Git repository settings, disconnect ANKH and connect ANUBIS-Website only once its main branch contains the tested site. If the interface requires creating another project, stop and choose the hostname migration deliberately; do not delete this project to reclaim its name.
5. If Cloudflare requests GitHub access, the user should grant the Cloudflare GitHub app access to **only ANUBIS-Website**. Codex GitHub access and Cloudflare GitHub access are separate permissions. Never paste tokens into repository files or chat.
6. Production branch: main. Framework: None. Build command: blank. Repository root: default. Output directory: site.
7. Verify a preview first: homepage, stylesheet/script/image, all section links, mobile layout, and the GitHub download destination. Check robots.txt, sitemap.xml, canonical URL, and structured data. Publish only the verified source.
8. After publishing, verify the production hostname and submit https://anubis-audio.pages.dev/sitemap.xml through the user's Google Search Console account after ownership verification.

The canonical hostname is the existing pages.dev address. Update canonical, sharing, schema, and sitemap URLs together if a custom domain becomes primary.

## Validation and upload status

Sitemap XML and structured-data JSON parse successfully. CSS, JavaScript, and the plugin image match the original backup byte for byte. The live site's content and download destinations were inspected in the browser. The local preview could not be reached from the browser environment, so a visual check of the prepared version remains required before deployment.

Creating the review branch through the GitHub connection returned HTTP 403, Resource not accessible by integration. No branch, pull request, or repository file was created. The user must review the GitHub connection's repository write authorization before upload can continue. The repository API's admin/push flags describe the account and do not guarantee that the integration can write.

Cloudflare documentation: https://developers.cloudflare.com/pages/configuration/git-integration/ and https://developers.cloudflare.com/pages/configuration/build-configuration/.
