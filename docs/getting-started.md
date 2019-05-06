* [Začíname s TypeScriptom](#getting-started-with-typescript)
* [Verzia TypeScriptu](#typescript-version)

# Začíname s TypeScriptom

TypeScript sa kompiluje do JavaScriptu. JavaScript je to, čo sa v skutočnosti vykonáva (buď v prehliadači alebo na strane servera). Budeš potrtebovať:

* kompiler TypeScriptu (na [githube](https://github.com/Microsoft/TypeScript/) a na [NPM](https://www.npmjs.com/package/typescript))
* editor TypeScriptu  (môžeš použiť poznámkový blok, odporúčam však [vscode 🌹](https://code.visualstudio.com/) s [rozšírením](https://marketplace.visualstudio.com/items?itemName=basarat.god). [Podpora pre iné IDE]( https://github.com/Microsoft/TypeScript/wiki/TypeScript-Editor-Support))


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

## Zdrojový kód knihy
Github repozitár https://github.com/basarat/typescript-book/tree/master/code 
