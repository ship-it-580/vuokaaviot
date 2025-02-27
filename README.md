# vuokaaviot


## Tanssiseuran etsintä
```mermaid
graph TD;
  A([Haluat tanssiseuraa]) --> B{Pyydät henkilöä tanssimaan};
  B -- Kyllä --> C[Tanssia ja kivaa];
  C --> E[Kotia kohti jnejne];
  B -- Ei --> D[Pyyhi kyyneleet ja yritä uudestaan];
  D --> B;
  
  
```

## Lampun vaihto
```mermaid
graph TD;
  A([Lamppu ei toimi]) --> B{Lamppu kytketty?}
  B -- Kyllä --> C{Polttimo palanut?}
  C -- Ei --> D(Osta uusi lamppu)
  B -- Ei --> E(Kytke lamppu)
  C -- Kyllä --> F(Vaihda polttimo)
```
