# GitOps Cockpit for Argo CD site

Static GitHub Pages site for the JetBrains plugin. The canonical public URL is <https://msolodev.github.io/gitops-cockpit-for-argocd-site/>.

## Release content boundary

- **RELEASE_A:** This checkout contains the privacy update for explicit opt-in PostHog Cloud EU plugin analytics, the 30-day Pro trial CTA, Free/Pro labels for existing features, JetBrains IDE wording, and feedback links. Publish the reviewed site just before the telemetry/baseline plugin release, verify the privacy policy is publicly reachable, then enable the plugin's `privacyPublished` build setting for that release.
- **RELEASE_B:** The source-navigation hero, Open Source Manifest section and demo, source-navigation documentation, and updated Free/Pro comparison belong in a separate later change. Do not merge or publish those claims before the source-navigation plugin release is available.

There is no site build system or website analytics. Keep dependencies pinned if tooling is added. For a local preview, run `python3 -m http.server 8000` from the repository root, then open the root page and the `privacy/` and `eula/` subpages. Before publication, check links, desktop and mobile layouts, keyboard navigation, and the claim-to-plugin evidence. Do not commit or publish automatically.
