# Chrome Dev Tools

## Antall bilder på forsiden:
Fant 4 bilder ved å skrive inn "document.images.length" i konsollvinduet.
Fant 17 bilder i Application>Frames>top>Images.

Totalt er det 17 bilder, hvorav 4 ligger som img-tagger på siden, mens de 13 andre bildene er lagt inn via CSS.

## Lastetid med og uten cache:
Gikk til "Network", refreshet siden noen ganger og fant ut at lastetiden var ca. 300-500 ms med cache, og 500-700 ms uten cache.

## Audit:
Trykket på "Lighthouse" og deretter på "Generate report" for desktop med alle kategoriene avkrysset.

Resultatene:
Performance: 91
Accessibility: 84
Best Practices: 92
SEO: 90
Progressive Web App: Fast and reliable: 1/3, Installable: 1/3, PWA Optimized: 4/8

## Antall eksterne requests:
Gikk til "Network". Så på requests nederst på siden.
Siden hadde 43 requests.

## Content-type i response header:
Gikk til "Network", og trykket på "tjenester/" i tabellen.
Content-type: text/html;charset=utf-8

## Cache-control i request header:
Gikk til "network", og trykket på "tjenester/" i tabellen.
Cache-control: max-age=0

## Protokoll:
Gikk til "Network", høyreklikket på tabellheaderen og trykket på "Protocol" for å vise protokollen som en kolonne i tabellen.
Protokollen som siden bruker er h2 (HTTP/2).