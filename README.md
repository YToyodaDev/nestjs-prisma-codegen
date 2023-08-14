# nestjs-prisma-codegen

```
npx nestjs-prisma-codegen ResourceName
```

# nestjs-prisma-codegen 🚀🦖

This package takes your resource name and generates all the tedious NestJS types that you'd otherwise write by hand.

# Usage 🧙‍♂️💼

No complicated spells or potions here. In your src/ directory, Just run the script with the required model name.

```
npx nestjs-prisma-codegen User
```

You will get these files generated.

```
├── common
│   ├── dtos
│   │   └── common.input.ts
├── models
│   └── users
│       ├── dtos
│       │   ├── create-user.input.ts
│       │   ├── find.args.ts
│       │   ├── order-by.args.ts
│       │   ├── update-user.input.ts
│       │   └── where.args.ts
│       ├── entity
│       │   └── user.entity.ts
│       ├── users.module.ts
│       ├── users.resolver.ts
│       └── users.service.ts
```

Then you can implement the input types with the help of typescript. Also the custom RestrictProperties type will always keep the nest types in sync with the prisma schema.
