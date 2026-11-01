# Kenya Land Parcels & Nairobi Block Lookup MCP

[Kiswahili](#kiswahili)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Nairobi land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- ~247k Nairobi City parcels, numbered by the post-2021 registration blocks (`Nairobi Block 181/2504`)
- Parcel lookup by block parcel number, pre-conversion Land Reference number (`LR 209/6668`), a whole block (paged), or coordinates
- Folio Register number, stated area, block (estate) name and sub-county
- Satellite and street map images of a parcel and its neighbours, labelled by block parcel number

Nairobi only. This is a community copy of the city cadastre, not an official bulk release: treat it as indicative. No owner or title information.

## Connect

```
https://bumiatlas.com/mcp/kenya
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/kenya](https://bumiatlas.com/mcp-docs/kenya).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `KE_parcel_search` | Find parcels by block parcel number, LR number, a whole block (paged), or `latitude, longitude`; each result is the whole record, the boundary as GeoJSON on request |
| `KE_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its block parcel number |

## Example prompts

- *"Which parcel is at -1.21703, 36.89944?"*
- *"Look up Nairobi Block 181/1870 and show it on satellite imagery."*
- *"What block parcel number does LR 57/1583 have now?"*
- *"List the parcels in Block 181."*

## Data source

Nairobi cadastre, community copy at github.com/leoouma/nairobi-cadastre (MIT); not an official Ministry of Lands release. A copy of public data for research, not a legal land record.

## Kiswahili

Unganisha msaidizi wako wa AI (Claude, ChatGPT au Cursor) na [BumiAtlas](https://bumiatlas.com) kupitia Model Context Protocol (MCP) kutafiti viwanja vya Nairobi.

- Takriban viwanja 247,000 vya Jiji la Nairobi
- Tafuta kwa namba ya block (`Nairobi Block 181/2504`), namba ya LR au kwa viwianishi (latitudo, longitudo)
- Picha za setilaiti na ramani za kiwanja na viwanja jirani

Hakuna majina ya wamiliki.

**Kuunganisha:** ongeza `https://bumiatlas.com/mcp/kenya` kama custom connector kwenye MCP client yako na uingie kwa Google. Majina ya zana ni ya Kiingereza, lakini msaidizi anaweza kujibu kwa Kiswahili.
