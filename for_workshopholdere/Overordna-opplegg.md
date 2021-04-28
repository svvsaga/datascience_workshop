## TODO

- Vi må avklare hvilke agendapunkter som kan være buffere som vi kan sløyfe dersom vi går over tida, uten at dette ødelegger for neste sesjon.
- Vi burde ta høyde for at noen kan "hoppe inn igjen" i workshop dersom de må være borte en time
  - F.eks. kan vi ha dataene man skal jobbe med i en gitt sesjon tilgjengelig utenfor deres personlige prosjekter

## Andre oppgaver i forkant
- Sende ut agenda (senest ila. fredag)
- Sende ut liste med ting som deltakerne må ordne på forhånd (senest ila. onsdag)

## Overordnet workshop-opplegg

- 10:00 - 10:30 Presentasjon om Saga, GCP, de mest brukte tjenestene, typiske kostnadsdrivere m.m.
- 10:30 - 11:15 Sesjon 1: "Extract and Load" med GCS, BigQuery
    - Grunnleggende innføring i hvordan få data inn i GCS og BigQuery
    - Hvordan hente data fra API til BigQuery gjennom Notebook: Trafikkregistreringspunkter fra trafikkdata
    - Hvordan gå inn i Data Catalog
    - Ekstra: Det samme som over, men via Cloud Function (kan sløyfes dersom vi går over tiden)
- 11:15 - 12:00 Lunsj
- 12:00 - 12:50 Sesjon 2: Transform: Intro til DBT og FME (og Apache Beam/Dataflow)
  -  Må finne ut om FME kan lese fra GCS
  -  Transformasjoner: Legge til "ingest time" fra filnavn og transformere "from" og "to" til gyldig iso8601 timestamp
  - Ekstra: Vi bruker Apache Beam/Dataflow til å fordøye og importere større mengder data (kan sløyfes dersom vi går over tiden)
  - Alternativ ekstra: Vi viser Apache Beam/Dataflow
- 12:50 - 13:00 Pause
- 13:00 - 13:50 Sesjon 3: Utforsking og analyse med BigQuery
- 14:50 - 15:00 Pause
- 15:00 - 15:40 Sesjon 4: Visualisering - DataStudio og GeoViz
- 15:40 - 16:00 Tilbakemelding og neste steg
  - Hvordan var workshoppen?
  - Klarte vi å dekke læringsmålene?
  - Hvilke andre temaer kunne folk tenke seg en innføring i?
  - Hvordan kan Saga støtte dere i videre analysearbeid?
  - Tror deltakerne at dette kan endre måten de jobber på?

## Læringsmål
- Laste opp egne datasett til GCS og BigQuery
- Kunne hente data gjennom API og Data Catalog
- Gjøre enkle transformasjoner med FME på data som ligger i GCS og BigQuery
- Hvordan bruke BigQuery som et analyseverktøy
- Forstå BigQuery sine styrker og begrensinger
- Bruke Data Studio og GeoViz til utforskende analyse og enkel visualisering


## Hvordan er hver sesjon strukturert?

1. Dersom nødvendig, en felles presentasjon/intro (5-10 min) til temaet hvor vi sier noe om:
    - Hva vi skal gjøre
    - Hvorfor vi skal gjøre det
    - Ting man må vite

2. Interaktiv sesjon hvor vi deler opp i 4 grupper som sitter i hvert sitt breakout-rom. Der kan deltagerne spørre hverandre om hjelp, dele skjerm osv. Vi fordeler oss utover i de 4 breaout-rommene som fasilitatorer.
3. En kort recap i fellesskap (5 min) på slutten av hver del.

## Feedback fra Lars

- Presentasjon: 1 time kanskje litt mykje, dei har sikkert meir lyst å kode meir
  - Lars foreslår: Halvtime til tre kvarter
- Sesjon:
  - Peder og Lars: Dataflow litt for tungvekt?
- Om tilbakemelding på slutten av dagen:
  - 10 minutt for lite
  - Ha nokon spørsmål klar
- Apache Beam/Dataflow vs FME vs andre ingest-måtar?
- Bør skrive ned læringsmål 

- Ein fin ekstra: Vise bigquery inn i pandas?
- Må ikkje være for SQL-vanskeleg. Dei fleste har nok 


- Om breakout rooms:
  - Er ikkje sikkert at SVV sin Teams støttar breakout rooms
