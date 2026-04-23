# nest

![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)

Primer acercamiento a **NestJS**. El repo contiene un módulo `tasks` con su controlador, partiendo del template oficial del framework. No tiene servicio ni persistencia: es solo el punto de partida para entender módulos, controladores y el CLI de Nest.

Ejercicio introductorio de aprendizaje.

> **Nota sobre el nombre:** el nombre del repositorio (`nest`) colisiona con el del framework oficial NestJS. Queda pendiente renombrarlo a algo como `nestjs-primeros-pasos`. Internamente el `package.json` se identifica como `nestfirstapp`.

## Stack

- **Framework:** NestJS 10
- **Lenguaje:** TypeScript 5
- **Runtime:** Node.js
- **Tests:** Jest + Supertest (scaffold)
- **Lint/format:** ESLint + Prettier

## Estructura

```
nest/
├── src/
│   ├── main.ts                    # Bootstrap de la app
│   ├── app.module.ts              # Módulo raíz
│   └── tasks/
│       ├── tasks.module.ts        # Módulo de tasks
│       └── tasks.controller.ts    # Controlador (@Controller('tasks'))
├── test/
├── nest-cli.json
├── tsconfig.json
└── package.json
```

## Scripts

```bash
# Instalar dependencias
npm install

# Desarrollo (watch)
npm run start:dev

# Producción
npm run build
npm run start:prod

# Tests
npm run test
npm run test:e2e
```

## Estado actual

- Módulo `tasks` registrado con un controlador vacío (`@Controller('tasks')`).
- Sin servicios, sin DTOs, sin base de datos.
- Pensado como base para iterar y agregar lógica real más adelante.

## Autor

Jean Caicedo — [@JeanCaicedo](https://github.com/JeanCaicedo)
