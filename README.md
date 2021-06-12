# Sequelize E-comerce
![last-commit](https://img.shields.io/github/last-commit/AugustoLL/ecomerce-sequelize)
![contributors](https://img.shields.io/github/contributors/AugustoLL/ecomerce-sequelize)
![node-version](https://img.shields.io/badge/Node->=12.0.0-brightgreen)
![npm-version](https://img.shields.io/badge/npm->=6.14.0-brightgreen)
![sequelize-version](https://img.shields.io/badge/sequelize-%3E%3D6.6.2-blue)
![dotenv-version](https://img.shields.io/badge/dotenv-%3E%3D10.0.0-blue)
![mysql2-version](https://img.shields.io/badge/mysql2-%3E%3D2.2.5-red)

## Project setup
```
npm install
```
## Sequelize Commands
The following command should be utilized after using any of the commands shown in the next section:
```
npx sequelize db:migrate
```
### List of commands
```
sequelize model:generate --name Brand --attributes name:string
```
```
sequelize model:generate --name Payment --attributes type:string
```
```
sequelize model:generate --name Category --attributes name:string
```
```
sequelize model:generate --name Gender --attributes type:string
```
```
sequelize model:generate --name Size --attributes name:string
```
```
sequelize model:generate --name Role --attributes description:string
```
```
sequelize model:generate --name State --attributes description:string
```
```
sequelize model:generate --name Address --attributes street:string,number:integer
```
```
sequelize model:generate --name User --attributes first_name:string,last_name:string,username:string,email:string,password:string,address_id:integer
```
```
sequelize model:generate --name UserHasRole --attributes users_id:integer,roles_id:integer
```
```
sequelize model:generate --name Product --attributes name:string,price:decimal,stock:integer,stock_min:integer,stock_max:integer,brands_id:integer
```
```
sequelize model:generate --name Image --attributes name:string,url:string,description:string
```
```
sequelize model:generate --name Shipping --attributes street:string,number:integer,delivered_date:date
```
```
sequelize model:generate --name Order --attributes number:integer,date:date,total:decimal,users_addresses:integer
```
```
sequelize model:generate --name OrderDetails --attributes quantity:decimal,subtotal:decimal
```
## Project Status
The project is still under development.