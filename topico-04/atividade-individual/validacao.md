# Validação pós-Alterações de Segurança

## 1. Testes de Acesso ao Serviço Web
Após a ativação do UFW, foram executados testes de conectividade ao servidor Nginx:

- **Teste HTTP Local:** `curl -I http://localhost/topico-03/index.html`
- **Resultado:** `HTTP/1.1 200 OK`

## 2. Conclusão da Validação
- O serviço web Nginx continua **100% funcional** e a responder na porta 80.
- O acesso SSH permanece ativo e protegido.
- As portas não autorizadas foram bloqueadas pela política padrão da firewall.
