# nestjs-firebase

![Actions Status](https://github.com/g59/nestjs-plugins/workflows/Node%20CI/badge.svg)
[![npm version](https://badge.fury.io/js/nestjs-firebase.svg)](https://badge.fury.io/js/nestjs-firebase)


# This will not be maintained

This is a fork of https://github.com/g59/nestjs-plugins/tree/main/packages/nestjs-firebase which does not yet support nestjs version 9.


## Install

For nestjs version 9:

```
npm install @nicholas.braun/nestjs-firebase
```

For nestjs version 8:

```
npm install nestjs-firebase
```

## Usage

```typescript
@Module({
  imports: [
    FirebaseModule.forRoot({
      googleApplicationCredential: "path/to/credential file.json",
    }),
  ],
})
export class AppModule {}

// using in service class
export class Service {
  constructor(
    @InjectFirebaseAdmin() private readonly firebase: FirebaseAdmin,
  ) {}
}
```

## Contributing

PRs accepted.

## License

[MIT](https://github.com/g59/nestjs-plugins/blob/main/LICENSE) © g59
