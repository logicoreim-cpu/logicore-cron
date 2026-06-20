# logicore-cron

Scheduled GitHub Actions workflow that pings `https://logicore.im/api/spotify/cron-poll`
every 15 minutes to pull recent Spotify plays for all connected Logicore users.

The endpoint is protected by a bearer token stored as the `CRON_SECRET` repository
secret (matching the `CRON_SECRET` env var on Vercel).
