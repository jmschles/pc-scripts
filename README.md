### Overview

This repository contains snapshots of the convenience scripts we use to start, stop, and restart app servers.  I will try to keep it up to date as the servers evolve.

### The Scripts

Scripts are organized by machine, since they vary depending on the needs of the server.
* dev-sf, qa1-sf, staging-sf, and sandbox-sf currently have identical setups and therefore share a folder.  The scripts start/stop all apps (cms_api, cms, storage, uploader, and jobs) in development mode.
* cms-prod scripts start/stop cms_api, cms, and storage in production mode.
* upload-prod scripts start/stop the uploader in production mode only.
* unused scripts on each server are in the `unused/` folder.  Maybe they'll be useful later!

### The .bashrc Snippets

The .txt files in this folder correspond to servers, and contain the snippets in twist-dev's .bashrc file that create aliases for the scripts above.  When included, they allow you to run, for example, `start_cms` from anywhere on the dev-sf machine.  **These snippets assume that your scripts live in `/home/twist-dev/bash_scripts` and will not work otherwise.**
