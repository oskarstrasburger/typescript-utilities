# typescript-utilities

Make selected properties nullable:
```ts
type PartialNullable<M, T extends keyof M> = {
  [K in keyof M]: K extends T ? M[K] : M[K] | null;
};
```
