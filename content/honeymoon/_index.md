---
draft: false
title: "Il nostro Viaggio di Nozze"
---

## 🌎❤️ Destinazione: Argentina

"Una terra lontana… dove la natura regna sovrana, i paesaggi cambiano ad ogni curva e ogni giorno è una nuova avventura."

<br>


<!-- MapLibre CSS & JS -->
<link href="https://unpkg.com/maplibre-gl@2.4.0/dist/maplibre-gl.css" rel="stylesheet" />
<script src="https://unpkg.com/maplibre-gl@2.4.0/dist/maplibre-gl.js"></script>

<!-- Mappa -->
<div id="map" style="height: 500px; border-radius: 10px; margin-bottom: 2rem;"></div>

<script>
  const map = new maplibregl.Map({
    container: 'map',
    style: 'https://api.maptiler.com/maps/aquarelle/style.json?key=ieAH8MPmB1ALRkjlPFmn',
    center: [-63.6167, -38.4161], // Centro Argentina
    zoom: 1.5
  });

  // Add zoom and rotation controls to the map
  map.addControl(new maplibregl.NavigationControl());

  // Coordinate list with names and anchor targets
  const places = [
    { name: "Patagonia", coords: [-72.9, -49.3], anchor: "#patagonia" },
    { name: "Perito Moreno", coords: [-73.2, -50.5], anchor: "#perito-moreno" },
    { name: "Iguazú", coords: [-54.6, -25.6], anchor: "#iguazu-falls" },
    { name: "Tilcara", coords: [-65.39, -23.57], anchor: "#tilcara" },
    { name: "Salinas Grandes", coords: [-65.1, -23.5], anchor: "#salinas-grandes" },
    { name: "Ruta 68", coords: [-65.97, -26.07], anchor: "#ruta-68" },
    { name: "Cafayate", coords: [-65.97, -26.07], anchor: "#cafayate" },
    { name: "Mendoza", coords: [-68.84, -32.89], anchor: "#mendoza" }
  ];

  map.on('load', function () {
    places.forEach((p, index) => {
      // Create a custom HTML marker
      const el = document.createElement('div');
      el.className = 'marker';
      el.style.width = '20px';
      el.style.height = '20px';
      el.style.backgroundColor = '#c0392b';
      el.style.borderRadius = '50%';
      el.style.cursor = 'pointer';
      el.style.boxShadow = '0 0 5px rgba(0,0,0,0.5)';

      const marker = new maplibregl.Marker(el)
        .setLngLat(p.coords)
        .setPopup(new maplibregl.Popup({ offset: 25 }).setHTML(`<a href="${p.anchor}">${p.name}</a>`))
        .addTo(map);
    });
  });
</script>

<br>

### 💌 Un pensiero per il nostro viaggio  <br><br>

Se desiderate farci un regalo, potete contribuire a realizzare questo viaggio di nozze. Sarà per noi un gesto prezioso, che porteremo nel cuore ad ogni tappa di questa fantastica avventura.  <br><br>

Potete farci un bonifico al seguente IBAN: <br><br>

### **Nicoletta Gentiloni Silveri** --  `IT83H0326803204052180830230`

<br>

Potete indicare la causale:  <br><br>

#### *Viaggio di nozze Andrea & Nicoletta*  <br><br>

## 🧭 Il nostro itinerario

Esploreremo una terra lontana e misteriosa, ma al tempo stesso familiare per l’anima che vive nelle sue piazze e nei suoi volti. <br><br>

Dal ghiaccio millenario della Patagonia alle foreste subtropicali di Iguazú, passando per deserti, canyon colorati e bianchi salares: sarà un viaggio memorabile, a stretto contatto con la natura: **avventuroso e  indimenticabile** 🌿🏞️

## 💞 Seguici in questa avventura

Ogni tappa sarà per noi un momento speciale da ricordare. Non vediamo l’ora di partire, e condividere con voi qualche aggiornamento, lungo la strada! 📸