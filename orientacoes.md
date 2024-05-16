## ORIENTAÇÕES PARA IMPLEMENTAÇÃO DA ARQUITETURA

### Ajustes para que os frontends possam trabalhar com variáveis de ambiente

### Foram criados 3 arquivos .env, cada um para os ambientes development, staging e production, respectivamente. 

![image](https://github.com/CelDarley/arquitetura/assets/99372966/ddd1cb01-d187-4585-9391-dde0860cee18)

### Para conseguirmos trabalhar com os arquivos .env, é preciso também adicionar a biblioteca “dotenv” no package.json”

### padronizar todas as requisições para a API, baseados no objeto api, que está definido em services/api.js

## é preciso definir que “baseURL”, terá o valor da variável de ambiente VUE_APP_ROOT_API, que está definido nos arquivos .env

![image](https://github.com/CelDarley/arquitetura/assets/99372966/82972dac-80ee-492a-90a9-8a941964247f)

### Não é mais necessário passar toda URL no caminho da requisição. Com o “baseURL” definido em api.js, podemos passar como parametro, somente o complemento da url do endpoint do backend. 

Exemplo:

![image](https://github.com/CelDarley/arquitetura/assets/99372966/1f39b7a6-ba22-4ca8-b1c0-81c5a0c54d8a)

### é necessário adicionar um arquivo Dockerfile em todos os projetos. Esse arquivo é para gerar a imagem docker dos projetos.
