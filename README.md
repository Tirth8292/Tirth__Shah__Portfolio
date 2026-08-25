# Tirth Shah Portfolio — Render Web Service

This folder contains the same portfolio page and content as the original, but is packaged as a Node.js web service so it deploys as a Render **Web Service**.

## Deploy with the provided configuration

1. Create a new GitHub repository.
2. Upload all files from this folder without renaming them.
3. On Render select **New** > **Blueprint**, choose the repository, and click **Apply**.

The included `render.yaml` checks Node.js, then runs `npm start`. Do not choose Docker. No Dockerfile or external package is required.

## Manual Web Service configuration

If you select **New** > **Web Service** instead of Blueprint, use:

- Runtime: `Node`
- Build Command: `node --version`
- Start Command: `npm start`
- Health Check Path: `/healthz`

After deployment opens successfully, the homepage is available at the Render URL.
