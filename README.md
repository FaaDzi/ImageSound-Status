# ImageSound Status

A tiny landing page for ImageSound, which runs on a home laptop behind a
Cloudflare quick tunnel whose URL changes on every start.

The page reads the current URL from a GitHub Gist (updated by the server's
launcher), checks the server's `/api/health`, and redirects to the login page
when it's up. Otherwise it shows that the server is offline and keeps checking.
