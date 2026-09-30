# Plano de Continuidade Operacional (Nginx)

## 1. Serviços e Ficheiros Críticos
- **Serviço Vital:** Nginx Web Server.
- **Configurações Críticas:** Ficheiros em `/etc/nginx/` e `/etc/nginx/sites-available/`.
- **Dados da Aplicação:** Conteúdo do site em `/var/www/html/topico-03/`.

## 2. Estratégia de Backup
- **Periodicidade:** Backup diário dos dados da aplicação e backup semanal das configurações do servidor.
- **Retenção:** Manter os últimos 7 backups diários e 4 semanais num armazenamento secundário/nuvem.

## 3. Procedimento de Recuperação em Caso de Desastre (Disaster Recovery)
1. Reinstalação do servidor Nginx (`sudo apt install nginx`).
2. Restauro das configurações em `/etc/nginx/`.
3. Restauro dos ficheiros web a partir do backup comprimido para `/var/www/html/`.
4. Reinício e validação do serviço (`sudo systemctl restart nginx`).
