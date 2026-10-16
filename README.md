# CDH & CONTACT AGILE WORK

Agile project management platform (Scrum & Kanban boards, user stories, sprints, issues, wiki) based on the open-source [Taiga](https://github.com/taigaio) project.

## Contents

| Folder | Component | Upstream | License |
|---|---|---|---|
| `taiga-back/` | Backend API (Python / Django) | [taigaio/taiga-back](https://github.com/taigaio/taiga-back) @ `c8264ac` | MPL-2.0 |
| `taiga-front/` | Web frontend (AngularJS) | [taigaio/taiga-front](https://github.com/taigaio/taiga-front) @ `367a4b8` | AGPL-3.0 |
| `taiga-events/` | Real-time events (WebSockets) | [taigaio/taiga-events](https://github.com/taigaio/taiga-events) @ `e411856` | MPL-2.0 |
| `taiga-protected/` | Protected attachments service | [taigaio/taiga-protected](https://github.com/taigaio/taiga-protected) @ `3fc1f92` | MPL-2.0 |
| `taiga-docker/` | Docker Compose deployment | [taigaio/taiga-docker](https://github.com/taigaio/taiga-docker) @ `e12c106` | MPL-2.0 |

## Running it

The quickest way is Docker:

```bash
cd taiga-docker
# edit .env (TAIGA_DOMAIN, SECRET_KEY, email settings, etc.)
./launch-all.sh
./taiga-manage.sh createsuperuser
```

Then open http://localhost:9000. See `taiga-docker/README.md` for full details.

## License & attribution

This repository redistributes Taiga, © Kaleidos INC and Taiga contributors. Each component keeps its original license file in its folder (MPL-2.0 or AGPL-3.0). Taiga is a trademark of Kaleidos INC; this project is not affiliated with or endorsed by Kaleidos.
