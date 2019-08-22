# typescript-utilities

Make selected properties nullable:
```
type PartialNullable<M, T extends keyof M> = {
  [K in keyof M]: K extends T ? M[K] : M[K] | null;
};
```
