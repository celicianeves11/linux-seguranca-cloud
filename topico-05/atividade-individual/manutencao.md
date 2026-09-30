# Procedimentos de Manutenção Preventiva

## 1. Rotinas Recomendadas
- **Atualização de Pacotes:** Execução periódica de `sudo apt update && sudo apt upgrade -y`.
- **Rotação e Limpeza de Logs:** Verificação do serviço `logrotate` para impedir o crescimento desmedido dos ficheiros em `/var/log/nginx/`.
- **Limpeza de Ficheiros Temporários:** Remoção de ficheiros antigos em `/tmp/`.
