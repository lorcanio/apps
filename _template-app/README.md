# New app pages

Not published: Jekyll skips folders that start with an underscore, and `_config.yml` excludes this one.

To add an app (after the app name and its real data use are known):

1. Copy the three pages to a new folder named after the app slug, e.g. `cp -r _template-app my-app` (then delete this README from the copy).
2. Replace every `{{PLACEHOLDER}}` in the copy. `{{DEVELOPER_NAME}}` is `lorcan.dev`, `{{SUPPORT_EMAIL}}` is `support@lorcan.dev`. Check no `{{` is left: `grep -rn '{{' my-app`.
3. Check the privacy text against the app's App Privacy label and `PrivacyInfo.xcprivacy` (a second reviewer reads it).
4. Add the app to `_data/apps.yml`.
5. Resulting URLs: `/my-app/`, `/my-app/privacy`, `/my-app/support`. Put the last two into AppConfig and App Store Connect.

The privacy and support pages are copied from AppShell `site/privacy.md` and `site/support.md`; front matter (layout, permalink) added.
