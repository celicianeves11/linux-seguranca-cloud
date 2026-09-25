# Análise de Superfície de Ataque

## 1. Serviço Web Utilizado
- **Servidor:** Nginx (versão 1.28.3 / Ubuntu)
- **Aplicação:** Páginas estáticas do Tópico 03 (`index.html`, `sobre.html`, `style.css`)

## 2. Serviços e Portas Identificados
- **Porta 80/TCP (HTTP):** Serviço `nginx` ativo e exposto para tráfego web.
- **Porta 22/TCP (SSH):** Serviço `sshd` ativo para administração remota da VM.
- **Porta 53/UDP (DNS Local):** Serviço de resolução de nomes interno do `systemd-resolved`.

## 3. Justificação das Portas Necessárias
- **Porta 80 (HTTP):** Essencial para servir o site do Tópico 03 ao público.
- **Porta 22 (SSH):** Necessária para administração remota segura do servidor Linux.

## 4. Riscos Iniciais Identificados
1. **Exposição de portas desnecessárias:** Existência de serviços a escutar na rede sem regras de filtragem ativas.
2. **Divulgação da versão do servidor:** O cabeçalho HTTP expõe a versão exata do Nginx (`Server: nginx/1.28.3`), permitindo que atacantes procurem vulnerabilidades conhecidas (CVEs).
3. **Ausência de tráfego cifrado (HTTPS):** A comunicação é feita em texto simples (HTTP/Porta 80), tornando os dados suscetíveis a interseção (*man-in-the-middle*).
