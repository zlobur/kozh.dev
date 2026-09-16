---
title: 'Логи докер-контейнера за последние 10 минут'
date: 2026-09-14
draft: false
type: text
tags: ['docker', 'cli']
---

Самый простой способ — флаг `--since`, он понимает относительное время:

```bash
docker logs --since 10m <container>
```

Если нужно ещё и следить за новыми строками:

```bash
docker logs --since 10m -f <container>
```

`--since` принимает не только `10m`, но и `2h`, `30s`, а также абсолютное время
(`2026-09-14T12:00:00`) или Unix-таймстамп — удобно, если нужен точный интервал,
а не «от текущего момента».

Через `docker compose` то же самое, но с именем сервиса из `docker-compose.yml`:

```bash
docker compose logs --since 10m <service>
```
