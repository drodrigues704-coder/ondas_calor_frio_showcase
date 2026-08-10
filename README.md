# Ondas de Calor e Frio — WebApp (Showcase)

WebApp WebGIS para visualização de indicadores climáticos relacionados
com **ondas de calor** e **ondas de frio** em Portugal Continental,
entre 2001 e 2025, a partir dos dados de reanálise **CERRA**
(Copernicus).

> Este repositório é uma apresentação pública do projeto — não contém
> o código-fonte, que é mantido num repositório privado.

## Capturas de ecrã

**Ondas de calor — número de eventos, região Norte**
![Ondas de calor, região Norte](images/heat-norte.png)

**Ondas de frio — duração máxima, Grande Lisboa**
![Ondas de frio, Grande Lisboa](images/cold-lisboa.png)

**Ondas de calor — intensidade total, Alentejo**
![Ondas de calor, Alentejo](images/heat-alentejo.png)

## O que é

Permite selecionar uma região (NUTS II), uma metodologia de deteção,
um evento, uma variável e um ano, e visualizar o resultado no mapa
como isobandas coloridas, com legenda dinâmica, séries temporais
(regional e por ponto clicado) e download do GeoTIFF correspondente.

## Funcionalidades

- **Duas metodologias de deteção**, selecionáveis em tempo real:
  - **OMM** — limiares fixos, segundo a Organização Meteorológica Mundial.
  - **Percentis** — limiares por percentil (P90 calor / P10 frio) da
    climatologia local de cada célula.
- **Seleção por região (NUTS II)**.
- **Cinco variáveis por evento**: número de eventos, dias em evento,
  duração máxima, intensidade máxima e intensidade total.
- **Renderização por isobandas** — áreas vetoriais suaves entre
  isolinhas, com legenda em gradiente contínuo.
- **Séries temporais** — evolução regional e no ponto clicado no mapa.
- **Basemaps alternativos** (escuro / claro / rua / híbrido).
- **Download do GeoTIFF** atualmente representado.

## Stack tecnológico

| Camada | Tecnologia |
|---|---|
| Backend | Python · FastAPI · rasterio · GDAL · geopandas |
| Frontend | JavaScript · Leaflet · Turf.js · Chart.js |
| Dados | Cloud Optimized GeoTIFF (COG), reanálise CERRA |

## Autor

Daniel Rodrigues

---

Interessado em ver uma demonstração? Contacta-me.
