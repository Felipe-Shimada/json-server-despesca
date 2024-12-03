json-server --watch db.json --port 4000

Endereço base do servidor:
http://localhost:4000

Endpoint para os dados da despesca:
http://localhost:4000/despesca

GET: Obter dados (ex.: todos os dados ou um item específico).

Todos os dados:
GET http://localhost:4000/despesca
Item específico:
GET http://localhost:4000/despesca/1

POST http://localhost:4000/despesca
Content-Type: application/json
Body: {
  "data": "2024-12-06",
  "peso": 1400
}

PUT http://localhost:4000/despesca/1
Content-Type: application/json
Body: {
  "id": 1,
  "data": "2024-12-03",
  "peso": 1250
}

DELETE http://localhost:4000/despesca/1
