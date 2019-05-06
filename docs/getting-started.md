* [Začíname s TypeScriptom](#getting-started-with-typescript)
* [Verzia TypeScriptu](#typescript-version)

# Začíname s TypeScriptom

TypeScript sa kompiluje do JavaScriptu. JavaScript je to, čo sa v skutočnosti vykonáva (buď v prehliadači alebo na strane servera). Budeš potrtebovať:

* kompiler TypeScriptu (na [githube](https://github.com/Microsoft/TypeScript/) a na [NPM](https://www.npmjs.com/package/typescript))
* editor TypeScriptu  (môžeš použiť poznámkový blok [vscode 🌹](https://code.visualstudio.com/) s [rozšírením](https://marketplace.visualstudio.com/items?itemName=basarat.god). [Podpora pre iné IDE]( https://github.com/Microsoft/TypeScript/wiki/TypeScript-Editor-Support))


## Verzia TypeScriptu 

Odporúčam používať najnovšiu (nightly) verziu.

Inštalácia cez terminál:

```
npm install -g typescript@next
```

* Ak chceš, aby  vscode používalo túto verziu tak pridaj do  `.vscode/settings.json`nasledujúci obsah:

```json
{
  "typescript.tsdk": "./node_modules/typescript/lib"
}
```

## Getting the Source Code
The source for this book is available in the books github repository https://github.com/basarat/typescript-book/tree/master/code most of the code samples can be copied into vscode and you can play with them as is. For code samples that need additional setup (e.g. npm modules), we will link you to the code sample before presenting the code. e.g.

`this/will/be/the/link/to/the/code.ts`
```ts
// This will be the code under discussion
```

With a dev setup out of the way let's jump into TypeScript syntax.
