# Configuração da Firewall (UFW)

## 1. Estado Inicial
O UFW encontrava-se inativo (`Status: inactive`), permitindo todo o tráfego de entrada para qualquer porta aberta no sistema.

## 2. Regras Aplicadas
- `sudo ufw allow ssh`: Permite tráfego na porta 22/TCP para gestão remota.
- `sudo ufw allow 'Nginx HTTP'`: Permite tráfego na porta 80/TCP para acesso ao serviço web.
- `sudo ufw enable`: Ativação da firewall com política padrão de bloqueio (*deny incoming*).

## 3. Estado Final e Validação das Regras
Output obtido com `sudo ufw status verbose`:

```text
Status: active
Logging: on (low)
Default: deny (incoming), allow (outgoing), disabled (routed)
New profiles: skip

To                         Action      From
--                         ------      ----
22/tcp                     ALLOW IN    Anywhere                  
80/tcp (Nginx HTTP)        ALLOW IN    Anywhere                  
22/tcp (v6)                ALLOW IN    Anywhere (v6)             
80/tcp (Nginx HTTP (v6))   ALLOW IN    Anywhere (v6)             
