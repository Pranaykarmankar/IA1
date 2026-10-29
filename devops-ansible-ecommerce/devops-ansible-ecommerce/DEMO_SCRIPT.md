# Demo Video Script (5-7 minutes)

Record with Zoom/Teams/Google Meet or OBS. Keep your face/voice on and share your screen.

| Time | What to show | What to say |
|---|---|---|
| 0:00-0:30 | Title slide or README top | "Hi, I'm <name>, roll no <...>. My case study is ShopEasy, an e-commerce application." |
| 0:30-1:30 | README lifecycle table + architecture diagram | Explain Plan -> Code -> Build -> Test -> Release -> Deploy -> Operate -> Monitor and how each applies to ShopEasy. Mention web, DB and monitoring tiers. |
| 1:30-2:15 | Development, testing, deployment, monitoring stages | Branching and pull requests; CI runs syntax check + lint; Ansible deploys; Prometheus/node_exporter and /health monitor. |
| 2:15-3:00 | `inventory.ini` | Explain groups `web`, `db`, `monitoring`, `[all:vars]`, and why grouping helps. |
| 3:00-4:30 | `site.yml` | Walk through 3 plays: Nginx + storefront, MySQL, node_exporter. Point out `template`, `notify`/handlers, `become`, variables from `group_vars`. |
| 4:30-5:30 | Terminal: `ansible all -m ping`, `--syntax-check`, then `ansible-playbook site.yml` | Show the PLAY RECAP with changed tasks. |
| 5:30-6:15 | Run playbook again | Show `changed=0` and explain idempotency. |
| 6:15-6:45 | Browser: site page, `/health`; GitHub Actions green run | Show end result and CI. |
| 6:45-7:00 | Closing | "This shows how DevOps and Ansible give repeatable, automated deployments. Thank you." |

## Tips
- Keep terminal font large and zoomed in.
- Rehearse once; run the playbook beforehand so packages are cached and the run is quick.
- Upload to Google Drive / YouTube (unlisted) and set sharing to "anyone with the link", then paste the link in the submission.
