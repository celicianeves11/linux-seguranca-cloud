# Plano de Hardening Inicial (Nginx)

## 1. Riscos Específicos do Serviço (Nginx)
- Ausência de cabeçalhos de segurança HTTP (ex.: `X-Frame-Options`, `X-Content-Type-Options`).
- Exposição da versão do Nginx no cabeçalho `Server`.
- Permissões de ficheiros inadequadas no diretório `/var/www/html/`.

## 2. Medidas Aplicadas Nesta Fase
- **Ajuste de permissões:** Leitura estrita para o utilizador `www-data` (`chmod -R 755 /var/www/html/topico-03`).
- **Filtragem de tráfego:** Bloqueio de todas as portas de entrada não utilizadas via `UFW`.
- **Atualização de pacotes:** Atualização do sistema operativo via `apt update && apt upgrade`.

## 3. Medidas Recomendadas para Tópicos Seguintes
- **Ocultar versão do Nginx:** Configurar `server_tokens off;` no ficheiro `/etc/nginx/nginx.conf`.
- **Implementar TLS/SSL (HTTPS):** Configurar certificados digitais com *Let's Encrypt* na porta 443.
- **Implementar Rate Limiting:** Limitar pedidos por IP para mitigar ataques de força bruta e DoS.
