# Registro de Testes de Software

Os testes de software do sistema Sweetify foram conduzidos com base em um plano pré-definido, visando validar rotas e funcionalidades principais.

## Testes de API
- Ferramentas utilizadas: Postman e Swagger  
- Módulos testados: insumos, receitas, serviços, produtos e encomendas  
- Resultados:
  - Todas as rotas responderam corretamente com os códigos HTTP adequados (200, 201, 204, 400, 404)
  - Requisições retornaram os dados esperados
  - Tratamento adequado de erros e mensagens claras ao usuário

## Análise dos Resultados dos Testes

Os resultados obtidos foram satisfatórios, indicando que a aplicação atende aos requisitos definidos.

### Ações Planejadas para Próximas Iterações

1. Aprimorar mensagens da API, tornando-as mais específicas e informativas  
2. Ampliar e padronizar a documentação no Swagger, incluindo exemplos e respostas esperadas  
3. Implementar novas validações no frontend, garantindo envio de dados completos e válidos  
4. Revisar a interface de usuário, incorporando feedbacks dos testes de usabilidade realizados com o Expo Go

## Conclusão

Os testes realizados confirmaram o bom desempenho e estabilidade do sistema, garantindo que:
- Todos os requisitos funcionais foram validados
- A integração entre camadas estável e consistente
- A aplicação encontra-se pronta para uso em ambiente de produção
