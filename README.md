# Blackjack React App using Typescript
Blackjack card game created for our math class using Typscript and React.

### Preveiw
![alt text](src/components/styles/picture/preview.png "Preview")

## Installation

- git clone this project
- npm install
- npm start

# Informations

You will have to make some changes inside the node_modules when you download the project 
- Change this export type ArrayKeys<T> = keyof { [P in keyof T as T[P] extends any[] ? P : never]: P }; to this 
  export type ArrayKeys<T> = {
  [P in keyof T]: T[P] extends any[] ? P : never;
  }[keyof T];

- Change this import type {CompareKeys} from 'pretty-format'; to import { CompareKeys } from 'pretty-format';

- Change this import type {SnapshotFormat} from '@jest/schemas'; to import { SnapshotFormat } from '@jest/schemas';

