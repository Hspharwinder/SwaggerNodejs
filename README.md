# SwaggerNodejs
Swagger for nodejs endpoints

STEPS:
----------------------------------
1. npm i swagger-ui-express <br>
2. file ---> app.js or endpoints.js <br>
	const swaggerUi = require('swagger-ui-express'); <br>
	const swaggerDocument = require('../swagger.json'); <br>
3. file ---> app.js or endpoints.js  <br>
  // user Apis  <br>
  app.get('/user', user.allUsers);   // endpoints/api which you have created <br>
	// swagger <br>
  app.use('/swagger', swaggerUi.serve, swaggerUi.setup(swaggerDocument)); <br>

4. create new file --> swagger.json <br>

5. run in browser  http://localhost:54358/swagger

