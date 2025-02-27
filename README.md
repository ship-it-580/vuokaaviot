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
```mermaid
graph TD;
  subgraph Lampun vaihto
    A([Lamppu ei toimi]) --> B{Lamppu kytketty?} -- Kyllä --> C{Polttimo palanut?} -- Ei --> D(Osta uusi lamppu) --> G([Lopetus]);
  end
  B -- Ei --> E(Kytke lamppu);
  E --> H([Lopetus])
  C -- Kyllä --> F(Vaihda polttimo);
  F --> I([Lopetus])
```

## Lomapäivä
```mermaid
graph TD;
  subgraph Lomapäivä
    A([Aloita]) --> B[Katso ulos ikkunasta] --> C{Sataako} --> |Ei| D[Mene rannalle] --> E([Lopeta]);
  end
  C --> |kyllä| F[Pysy kotona]
  F --> G([Lopeta])
```

## Herätys aamulla
```mermaid
flowchart TD
  subgraph Herätys aamulla
    A((Alku)) --> B(Herätyskello soi) --> C{Oletko valmis nousemaan?} --> |Kyllä| D(Nouse ylös sängystä) --> E((Loppu))
  end
  G --> B
  F --> G[Lepää]
  C --> |Ei| F([Käytä Snooze -toimintoa])
  
```

