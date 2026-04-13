# BirdStation Network — Live Map

Interactive map of all [BirdStation](https://github.com/ernens/birdash) bird detection stations.

**[View the live map](https://ernens.github.io/birdash-network/)**

## What is this?

BirdStation installations can opt-in to share their detection statistics with the community network. This map shows all registered stations with:

- Station location and online/offline status
- Total detections and species count
- Hardware info (Pi model, BirdNET version)
- Top 5 species from the latest daily report

## How to join

1. Install [BirdStation](https://github.com/ernens/birdash) on your Raspberry Pi
2. Go to **Settings > Station** and click **Join the network**
3. Your station appears on the map within minutes

No personal data is transmitted. Only station name, GPS coordinates, hardware info, and daily detection summaries (species names + counts) are shared.

## Technical details

- Data stored in [Supabase](https://supabase.com) (PostgreSQL)
- Map rendered with [Leaflet](https://leafletjs.com) + [CARTO](https://carto.com) dark basemap
- Zero backend — static HTML querying the Supabase REST API directly
- Hosted on GitHub Pages

## License

[MIT](https://github.com/ernens/birdash/blob/main/LICENSE)
