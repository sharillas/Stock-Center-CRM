# Stock Center CRM

Aplicação web de gestão de **stock** e **distribuição de equipamento de vídeo/LED por datas** (eventos/projetos).

## Funcionalidades

- **Visão Geral** — dashboard com stock, eventos, alocações e conflitos.
- **Inventário** — stock por equipamento, com *pico de uso* calculado por datas (reutilização entre eventos sem sobreposição).
- **Eventos** — projetos com datas e local.
- **Alocações** — atribuição de equipamentos a eventos.
- **Calendário de Distribuição** — linha temporal por datas, com deteção de conflitos (sobre-alocação).

## Como usar

É uma aplicação de **ficheiro único** (`index.html`), sem build nem dependências de runtime — só browser.

Os dados são guardados localmente no browser (`localStorage`) e podem ser **exportados/importados** em JSON (botões no topo).

## Deploy

Basta servir o `index.html` com qualquer servidor estático. Exemplo com nginx:

```bash
mkdir -p /var/www/stock.smartchoice.tech
cp index.html /var/www/stock.smartchoice.tech/
```

## Nota

Aplicação criada por um agente de IA (OpenHands) em nome de sharillas.
