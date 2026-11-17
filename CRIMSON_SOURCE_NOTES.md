# CRIMSON source notes

This first source milestone applies the CRIMSON product name, creator credit, icon artwork, and crimson visual tokens to the uploaded Millida Launcher 2.8.1 source. It intentionally does **not** claim that the original service integrations have been replaced or that Android has been ported.

## Build status

- Source archive extracted and key JSON metadata updated.
- Desktop and Android icon image files regenerated from the supplied CRIMSON artwork.
- Main boot/titlebar logo references changed to `public/crimson-mark.png`.
- Core launch engine has not been rewritten.
- No APK or desktop installer was built or runtime-tested in this environment.

## Backend and account dependencies

The original source contains Millida-specific account, social, cloud, skin, hosting, catalog-proxy, updater, and telemetry endpoints. Those integrations require a CRIMSON backend and CRIMSON-owned application registrations before a distributable fork can be considered independent. They have not been silently relabelled as CRIMSON services.

## Upstream attribution

This fork is based on Millida Launcher 2.8.1. The GPL-3.0-only `LICENSE`, `NOTICE`, `THIRD-PARTY.md`, and `TRADEMARK.md` are retained. The source copyright and third-party license notices remain in place.
