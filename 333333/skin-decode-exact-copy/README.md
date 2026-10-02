# Skin Decode — exact copy with supplied product photos

This build keeps the existing Skin Decode pages, styling, navigation, account flows, Skin Scan, ingredients, and SQLite database. The Brands catalog has been limited to the 20 Skin Decode products for which supplied pack artwork is available.

## Product photos
- 20 supplied Skin Decode pack images are used.
- Each image is prepared as a 4096x4096 (4K square) WebP with light sharpening/upscaling.
- No Korean/Indian product is shown without a supplied photo.

## Run
Requires Node.js 22+.

```powershell
npm install
npm start
```

Open http://localhost:3000

## Database
Uses Node 22+ built-in `node:sqlite`. On startup, the server synchronizes the `products` table with `products.json`, so the catalog stays at the 20 photo-backed products while user/account data remains in SQLite.
