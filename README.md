# Sequelize E-comerce
![last-commit](https://img.shields.io/github/last-commit/AugustoLL/ecomerce-sequelize)
![contributors](https://img.shields.io/github/contributors/AugustoLL/ecomerce-sequelize)
![node-version](https://img.shields.io/badge/Node->=12.0.0-brightgreen)
![npm-version](https://img.shields.io/badge/npm->=6.14.0-brightgreen)

## Project setup
```
npm install
```
## Comandos de Sequalize
Luego de cada comando que se menciona a continuación se debe ejecutar el siguiente comando:
```
npx sequelize db:migrate
```
### Lista de comandos
```
npx sequelize model:generate --name Brand --attributes name:string
```
```
npx sequelize model:generate --name Category --attributes name:string
```
```
npx sequelize model:generate --name Gender --attributes type:string
```
```
npx sequelize model:generate --name Size --attributes name:string
```
```
npx sequelize model:generate --name Image --attributes name:string, url:string, description:string
```
```
npx sequelize model:generate --name State --attributes description:string
```
```
npx sequelize model:generate --name Address --attributes street:string,number:integer
```
```
npx sequelize model:generate --name Role --attributes description:string
```
```
npx sequelize model:generate --name User --attributes first_name:string,last_name:string, username:string, email:string, password:string, address_id:integer
```
```
npx sequelize model:generate --name Payment --attributes type:string
```
```
npx sequelize model:generate --name Product --attributes name:string, price:decimal, stock:integer, stock_min:integer, stock_max:integer, brands_id:integer
```
```
npx sequelize model:generate --name OrderDetails --attributes quantity:decimal,subtotal:decimal
```
```
npx sequelize model:generate --name Order --attributes number:integer, date:date, total:decimal, payments_id:integer, users_addresses:integer, states_id:integer
```
```
npx sequelize model:generate --name UserHasRole --attributes users_id:integer,roles_id:integer
```

## Project Status
The project is still under development.