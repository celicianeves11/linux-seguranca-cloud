# Atividade prática individual - Tópico 3

## Nível realizado
Nível 2 - Intermédio

## Objetivo
Criar, publicar, validar e documentar um pequeno site com duas páginas e CSS em ambiente Linux.

## Ambiente utilizado
VM local (Ubuntu no VirtualBox)

## Rota de publicação
Nginx

## Ficheiros criados
- `site/index.html`
- `site/sobre.html`
- `site/style.css`
- `comandos.txt`
- `publicacao.md`
- `validacao.md`
- `README.md`

## URLs testados
- `http://localhost/topico-03/`
- `http://localhost/topico-03/sobre.html`

## Evidências produzidas
- Validação com `curl -I` que confirmou a resposta `200 OK` do servidor Nginx.

## Dificuldades encontradas
Comunicação entre a rede do hospedeiro Windows e a rede NAT da VM local.

## Link do repositório GitHub
https://github.com/vboxuser/linux-seguranca-cloud

## Próximos passos
No Tópico 04, aplicar regras de segurança com firewall (UFW) e análise de registos de acesso (logs) do Nginx.
