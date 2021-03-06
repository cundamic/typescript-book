# JavaScript

Existuje a bude existovať veľa súperiacich kompilerov z nejakej syntaxe do  _JavaScriptu ._ TypeScript sa od nich líši tým, že  _JavaScript je TypeScript_. 

![JavaScript je TypeScript](https://raw.githubusercontent.com/basarat/typescript-book/master/images/venn.png)

Znamená to, že sa budeš musieť naučiť _JavaScript_. TypeScript Ti vlastne poskytuje  dokumentáciu.

* Samotná nová syntax nepomáha s chybami  \(pozerám na Teba CoffeeScript\).
* Vytvorenie nového jazyka \(pozerám na Teba Dart\).

## Making JavaScript Better

TypeScript Ťa ochráni pred tým, čo v JavaScripte nefunguje:

```typescript
[] + []; // JavaScript Ti dá "" (čo je nezmysel), v TypeScripte je to chyba

// 
// aj iné nezmysly v JavaScripte nedávajú chybu počas behu, čím sa sťažuje hľadanie chýb
// TypeScript však vyvolá chybu už počas kompilácie 
//
{} + []; // JS : 0, TS chyba
[] + {}; // JS : "[object Object]", TS chyba
{} + {}; // JS : NaN alebo [object Object][object Object] v závislosti od prehliadača, TS chyba
"ahoj" - 1; // JS : NaN, TS chyba

function add(a,b) {
  return
    a + b; // JS : undefined, TS chyba 'unreachable code detected'
}
```



[Vysvetlenie](https://stackoverflow.com/questions/9032856/what-is-the-explanation-for-these-bizarre-javascript-behaviours-mentioned-in-the) 

TypeScript je [ linting](https://it-slovnik.cz/pojem/linting) pre JavaScript, ktorý vykonáva svoju prácu lepšie, pretože má informáciu o type. 

## 

