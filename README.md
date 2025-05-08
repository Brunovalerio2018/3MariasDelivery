# 3MariasDelivery


O **3MariasDelivery** é um projeto criado com o objetivo de estudar e desenvolver uma aplicação de delivery moderna, com arquitetura baseada em **API RESTful utilizando NestJS** e integração com aplicações **web e mobile**. A ideia central é construir uma base sólida que simula um ambiente real de desenvolvimento backend e frontend, integrando serviços e ferramentas utilizadas no mercado.

Este projeto serve como um laboratório de aprendizado envolvendo:

- Criação de APIs com NestJS (Node.js e TypeScript)
- Documentação de endpoints com Swagger
- Consumo da API usando Axios
- Integração com bancos de dados (PostgreSQL)
- Comunicação com aplicativos mobile e web
- Organização em ambientes de desenvolvimento (como GitHub Codespaces)

## 🔧 O que o projeto envolve

- Backend com **NestJS**, estruturado por módulos, controladores e serviços
- Endpoints REST documentados com **Swagger**
- Frontend React Native (Expo) e/ou ReactJS, consumindo os dados com **Axios**
- A API pode ser iniciada com `npm run start:dev` tanto no ambiente local quanto no Codespaces
- Ideal para quem deseja entender como se estrutura um backend completo e como integrá-lo com o frontend

## 🚀 Comandos úteis para criar um projeto semelhante

### 1. Instalar o NestJS CLI
```bash
npm install -g @nestjs/cli
nest new nome-do-projeto
npm install @nestjs/swagger swagger-ui-express axios


import { NestFactory } from '@nestjs/core';
import { AppModule } from './app.module';
import { SwaggerModule, DocumentBuilder } from '@nestjs/swagger';

async function bootstrap() {
  const app = await NestFactory.create(AppModule);

  const config = new DocumentBuilder()
    .setTitle('API Delivery')
    .setDescription('Documentação dos endpoints da API de delivery')
    .setVersion('1.0')
    .build();

  const document = SwaggerModule.createDocument(app, config);
  SwaggerModule.setup('api', app, document);

  await app.listen(3000);
}
bootstrap();


nest g module pedidos
nest g controller pedidos
nest g service pedidos


O 3MariasDelivery é um projeto ideal para quem está aprendendo
 desenvolvimento backend com NestJS
 e deseja integrar uma API com aplicações mobile e web.
Ele ensina, na prática, como estruturar uma API robusta, como documentá-la com Swagger,
 como consumir dados com Axios e como organizar um ambiente de desenvolvimento eficiente para projetos reais.

Sinta-se livre para explorar, modificar e evoluir este projeto conforme suas necessidades!
