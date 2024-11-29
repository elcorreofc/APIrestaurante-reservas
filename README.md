API de Reservas de Mesa
Este projeto implementa uma API RESTful simples para gerenciar reservas de mesa. A API permite agendar, listar, atualizar e excluir reservas de mesa em um restaurante, usando Node.js com o Express.

Funcionalidades
POST /agendar: Cria uma nova reserva de mesa.
GET /reservas: Retorna todas as reservas.
GET /reservas/:id: Retorna uma reserva específica, com base no ID.
PUT /reservas/:id: Atualiza uma reserva existente.
DELETE /reservas/:id: Deleta uma reserva.
Pré-requisitos
Antes de rodar o projeto, você precisará ter o Node.js e o npm instalados em sua máquina.

Como instalar o Node.js e o npm
Acesse o site oficial do Node.js.

Baixe e instale a versão LTS (Long Term Support), que é recomendada.

Após a instalação, você pode verificar se o Node.js e o npm foram instalados corretamente, executando os seguintes comandos no terminal:

bash
Copiar código
node -v
npm -v
Como rodar o projeto
1. Clonar o repositório
Clone este repositório para sua máquina local:

bash
Copiar código
git clone https://github.com/seu-usuario/reservas-api.git
cd reservas-api
2. Instalar dependências
No diretório do projeto, execute o comando abaixo para instalar as dependências do projeto:

bash
Copiar código
npm install
3. Rodar o servidor
Para iniciar o servidor da API, execute:

bash
Copiar código
npm start
O servidor será iniciado em http://localhost:3000.

4. Testar a API
Agora você pode testar as rotas da API usando ferramentas como o Postman ou o curl.

Exemplos de uso:
Criar uma reserva (POST /agendar):

URL: http://localhost:3000/agendar Body (JSON):

json
Copiar código
{
  "nome": "João Silva",
  "data": "2024-12-01",
  "horario": "19:00"
}
Listar todas as reservas (GET /reservas):

URL: http://localhost:3000/reservas

Obter uma reserva específica (GET /reservas/:id):

URL: http://localhost:3000/reservas/1

Atualizar uma reserva (PUT /reservas/:id):

URL: http://localhost:3000/reservas/1 Body (JSON):

json
Copiar código
{
  "nome": "João Silva",
  "data": "2024-12-02",
  "horario": "20:00"
}
Excluir uma reserva (DELETE /reservas/:id):

URL: http://localhost:3000/reservas/1

Estrutura do Projeto
bash
Copiar código
/reservas-api
  /node_modules        # Dependências instaladas
  /public              # Arquivos estáticos (se houver)
  /src                 # Código fonte da API
  server.js            # Arquivo principal que inicia o servidor
  package.json         # Dependências e scripts do projeto
  README.md            # Este arquivo
Contribuindo
Se você gostaria de contribuir para este projeto, fique à vontade para fazer um fork do repositório e enviar pull requests.

Faça um fork deste repositório.
Crie uma nova branch (git checkout -b minha-nova-funcionalidade).
Faça as mudanças necessárias e envie os commits (git commit -am 'Adiciona nova funcionalidade').
Envie a branch para o seu repositório (git push origin minha-nova-funcionalidade).
Abra um pull request neste repositório.
Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais informações.

Este README.md cobre os aspectos principais do projeto, como instalação, execução e exemplos de uso da API, além de fornecer instruções para contribuir com o código.



