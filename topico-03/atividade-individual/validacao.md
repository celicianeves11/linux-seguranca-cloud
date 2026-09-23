# Validação

## URLs testados
- `http://localhost/topico-03/index.html`
- `http://localhost/topico-03/sobre.html`

## Resultado dos testes
Ambos os ficheiros responderam com o código de estado `HTTP/1.1 200 OK`.

## Evidências
- Validação no terminal via `curl -I http://localhost/topico-03/index.html`
- Testes confirmados no terminal da VM com o serviço Nginx ativo.

## Observações
O servidor respondeu adequadamente na porta 80 e os ficheiros estáticos foram servidos sem erros.
