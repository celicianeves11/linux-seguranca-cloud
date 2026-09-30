# Relatório de Monitorização de Recursos

## 1. Mapeamento de Recursos do Sistema
- **Tempo de Atividade (Uptime):** Sistema operacional sem interrupções não planeadas.
- **Memória RAM:** Verificação executada com `free -h` para garantir disponibilidade adequada de memória sem uso excessivo de Swap.
- **Espaço em Disco:** Verificação da partição raiz (`/`) com `df -h /` para prevenir o esgotamento de armazenamento.
- **Estado do Serviço Web:** O serviço Nginx encontra-se em estado `active (running)`.

## 2. Métricas Coletadas
- **Serviço Alvo:** Nginx HTTP Server
- **Porta de Escuta:** 80/TCP
- **Disponibilidade:** 100% durante o período de validação.
