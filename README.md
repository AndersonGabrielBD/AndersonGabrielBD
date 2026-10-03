### Olá, sou o Anderson Gabriel 👋

Desenvolvedor Backend focado em **Python, AWS e dados**, atuando no setor de **healthtech** na IntuitiveCare.

**Stack:** Python · AWS (Lambda, ECS Fargate, SQS, EventBridge) · Celery · SQL · SQLAlchemy · Pydantic · Pandas/Polars · pytest · CI/CD

### 🎮 Em destaque: [steam-price-tracker](https://github.com/AndersonGabrielBD/steam-price-tracker)

Rastreador de preços da Steam em tempo real, em reais (R$) — não só mais um CRUD com gráfico:

- **Fila assíncrona de verdade**: Celery + Redis checando preços periodicamente, não um `setInterval` disfarçado — Beat e Worker como processos separados, do jeito que roda em produção.
- **Dado real, não mockado**: histórico de preço importado do IsThereAnyDeal e validado empiricamente contra a API antes de confiar nele; preço atual direto da Steam com `cc=br`.
- **Atualização ao vivo**: preço muda → evento no Redis pub/sub → WebSocket → gráfico atualiza sozinho no React, sem dar refresh.
- **Mentalidade de produção**: health check que testa Postgres e Redis de verdade, cache com fallback gracioso, rate limiting, logging estruturado em JSON — as decisões (o *porquê*, não só o *como*) estão documentadas no README do projeto.

**Stack:** FastAPI · Celery · Redis · PostgreSQL · SQLAlchemy · structlog · React · Recharts · Docker

---

**Outros projetos:** [ClinNext](https://github.com/AndersonGabrielBD/ClinNext) — SaaS de gestão para clínicas, do backend à interface · [webscraping](https://github.com/AndersonGabrielBD/webscraping) — pipeline de dados públicos da ANS (scraping, ETL, API) · [ladinpageclinnext](https://github.com/AndersonGabrielBD/ladinpageclinnext) — landing page de vendas do ClinNext

📫 Contato: gaabrieelbarbosaa@gmail.com · [linkedin](https://www.linkedin.com/in/andersongabriel1/)
