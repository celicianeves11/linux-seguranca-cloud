# Publicação do Serviço Web

## Nível escolhido
Nível 2 - Intermédio

## Rota escolhida
Nginx

## Ficheiros criados
- index.html
- sobre.html
- style.css

## Local de publicação
`/var/www/html/topico-03/`

## Comandos principais utilizados
- `sudo apt install nginx`
- `sudo mkdir -p /var/www/html/topico-03`
- `sudo cp -r site/* /var/www/html/topico-03/`
- `sudo chown -R www-data:www-data /var/www/html/topico-03`

## Resultado obtido
Serviço publicado com sucesso e a responder localmente com código HTTP 200 OK.

## Limitações encontradas
Configuração de rede NAT do VirtualBox requer redirecionamento de portas para acesso externo a partir do sistema operativo hospedeiro.
