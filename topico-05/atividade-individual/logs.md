# Análise de Registos (Logs)

## 1. Registos do Sistema e do Serviço Web
Análise efetuada nos ficheiros `/var/log/nginx/access.log` e `/var/log/nginx/error.log` via `journalctl`.

## 2. Eventos Relevantes Identificados
- **Acessos HTTP Validados:** Pedidos `GET /topico-03/index.html` e `GET /topico-03/sobre.html` responderam com o código **`HTTP 200 OK`**.
- **Registo de Erros:** Não foram identificadas falhas críticas de sistema ou erros de permissão (`HTTP 403/500`) nos registos recentes.
- **Atividade de Rede:** Confirmação dos pedidos efetuados pelo cliente local via browser/curl.
