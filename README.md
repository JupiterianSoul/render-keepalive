# render-keepalive

Pings a Render web service every 10 minutes so the free instance doesn't spin down.

The URL is stored in the `PING_URL` repository secret. GitHub pauses scheduled workflows in public repos after 60 days without activity, so `stay-active.yml` commits a timestamp on the 1st of every month.
