# Dormant fork

This fork is **no longer used to deploy CIPP** for Novix IT.

On 28 September 2026 our self-hosted CIPP instance (resource group `cipp-prod`) was
migrated from the Function App + Static Web App setup to a single Linux container
Web App (`cippsanf2`), following
https://docs.cipp.app/setup/maintaining-cipp/migrating-to-the-new-infrastructure.

The Web App runs the upstream image `ghcr.io/cyberdrain/cipp` and updates itself
(CIPP → Container Management → Status & Updates). Nothing in this repository is
built or deployed any more, so the deploy and upstream-sync workflows have been removed.

- Live instance: https://manage.novixit.co.uk
- Upstream: https://github.com/KelvinTegelaar/CIPP and https://github.com/KelvinTegelaar/CIPP-API

Only revive this fork if we need to run our own code changes, which would mean building
and hosting our own container image.
