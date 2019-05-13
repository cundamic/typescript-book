# Rovnosť

Treba  mať na pamäti rozdiel medzi `==` a `===`.  JavaScript sa snaží pomáhať programátorovi tak, že `==` používa pretypovanie  \(type  [coercion](https://beta.chesstempo.com/chess-tactics/)\) , napríklad zmení reťazec na číslo \(ak sa to dá\) a tak ho môžeš porovnať s číslom:

```javascript
console.log(5 == "5"); // true   , TS chyba
console.log(5 === "5"); // false , TS chyba
```

Toto pretypovanie nie je vždy ideálne. Napríklad pri porovaní  `""` a `"0"`  dostaneme `false,`pretože  sa reťazce nerovnajú. V druhom prípade  `0`a prázdny reťazec   \(`""`\)  sú považované za nepravdivé \(falsy, t.j. správajú sa ako`false`\) a  preto sú pri`==` rovnaké  a výsledkom je `true`  . Ak použijeme `===`  tak dostaneme `false`.

```javascript
console.log("" == "0"); // false
console.log(0 == ""); // true

console.log("" === "0"); // false
console.log(0 === ""); // false
```

> `string == number` and `string === number` sú v TypeScripte kompilačné chyby.

Podobne ako `==` vs. `===` sa správa aj `!=` vs. `!==`

Tip: Vždy používaj `===` a `!==`  s výnimkou pre  null kontrolu.

## Štrukturálna rovnosť

Na zistenie štrukturálnej rovnosti dvoch objektov nám nestačí `==`/`===`

```javascript
console.log({a:123} == {a:123}); // False
console.log({a:123} === {a:123}); // False
```

Pomôže nám  npm balíček [deep-equal](https://www.npmjs.com/package/deep-equal).

```javascript
import * as deepEqual from "deep-equal";

console.log(deepEqual({a:123},{a:123})); // True
```

Hľadanie daného  `id` :

```typescript
type IdDisplay = {
  id: string,
  display: string
}
const list: IdDisplay[] = [
  {
    id: 'foo',
    display: 'Foo Select'
  },
  {
    id: 'bar',
    display: 'Bar Select'
  },
]

const fooIndex = list.map(i => i.id).indexOf('foo');
console.log(fooIndex); // 0
```

