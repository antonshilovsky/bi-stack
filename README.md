# BI Stack (Jupyter + PostgreSQL + Metabase + Samba)

Домашний BI-сервер на Docker.

## Состав
- PostgreSQL 16 — хранилище данных
- JupyterLab — загрузка и обработка CSV/Excel
- Metabase — визуализация и дашборды
- Samba — доступ к данным с Windows

## Архитектура
Windows → Samba → Jupyter → PostgreSQL → Metabase

## Запуск
```bash
docker compose up -d

## Доступ

Jupyter: http://<server-ip>:8899

Metabase: http://<server-ip>:3000

Samba: \<server-ip>\share
