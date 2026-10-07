# Privacy Policy — GitOps Cockpit for Argo CD

*Last updated: October 6, 2026*

## Who is responsible

Michael Latta Software is the controller for the optional plugin analytics described here. For privacy questions or deletion requests, contact [m.latta.pro@gmail.com](mailto:m.latta.pro@gmail.com).

## Optional plugin analytics

GitOps Cockpit asks whether you want to share product usage analytics. Analytics are off until you explicitly choose “Share anonymous usage.” Choosing “No thanks” does not limit the plugin. You can change your choice in **Settings → Tools → GitOps Cockpit Privacy**.

If you opt in, the plugin creates a random, persistent installation identifier. It connects events across projects and IDE launches without using your name or account. Because it persists, and because the analytics processor receives network metadata, this data is more precisely described as **pseudonymous** than strictly anonymous.

Each event contains a fixed event type, UTC timestamp, event UUID, installation identifier, schema and plugin versions, IDE product and build, predefined feature and trigger categories, a licensing category, predefined result and failure categories where applicable, and whether a server was configured at first observation. The licensing category describes an observed entitlement, not a purchase. Events concern plugin opening, server configuration, connection and application loading, explicit application and resource selection, displayed inspections, and Pro feature attempts or prompts. The plugin sends no arbitrary text fields.

Analytics events do **not** include source code, manifest or log contents, repository names or URLs, Argo CD server URLs, application or resource names, namespaces, file paths, branches, commit hashes, credentials or tokens, usernames or email addresses, raw exception messages, license stamps, operating system names, or session identifiers.

## Processing and retention

Product analytics are sent to **PostHog Cloud EU** and processed in its EU-hosted environment. The plugin disables PostHog person profiles and geolocation enrichment; it does not use identification, autocapture, or session recording. As with any network request, PostHog receives connection metadata such as the source IP address. This is separate from the event fields listed above.

Analytics events are retained according to the PostHog Free-plan retention period, currently up to one year. This event-retention period does not describe PostHog's separate network or service logs, which are governed by its own processor policies.

The plugin keeps pending events only in memory. Turning analytics off stops future collection, cancels pending delivery, discards queued events, and clears the local installation identifier. A request already accepted by PostHog cannot be recalled by changing the setting. Events previously transmitted are not automatically deleted when you opt out; they remain until retention expires or a deletion request is completed. Opting in again creates a new identifier.

To request deletion of events associated with your installation, copy the identifier shown in **GitOps Cockpit Privacy** settings **before** turning analytics off, then email it to [m.latta.pro@gmail.com](mailto:m.latta.pro@gmail.com). Michael Latta Software will arrange deletion through PostHog. Without that identifier, it may not be possible to locate your events because no account or name is attached to them.

## Credentials and Argo CD communication

Argo CD credentials are stored locally through IntelliJ Platform PasswordSafe according to your IDE's credential-store configuration. The plugin uses the Argo CD server URLs you configure to perform its requested operations. Credentials, manifests, logs, and other Argo CD content are not included in product analytics.

## This website

The marketing site is hosted on GitHub Pages. It does not include PostHog, website analytics scripts, tracking cookies, or session replay. GitHub Pages logs visitor IP addresses for security purposes under [GitHub's privacy practices](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection).

## Changes

Updates to this policy will be posted on the [privacy page](privacy/).
