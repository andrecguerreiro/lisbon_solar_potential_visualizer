# Roof 3D Map publish package

This folder is a GitHub Pages-friendly version of `roof_3d_map.html`.

Files:

- `index.html` ? the lightweight map application shell.
- `payload.json.gz` ? the compressed map dataset loaded by the page.

## Preview locally

Run this from this folder:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000/`.

Do not open `index.html` directly from Explorer, because browser security usually blocks `fetch()` from `file://` URLs.

## Publish on GitHub Pages

1. Put these two files in a small public GitHub repository.
2. In GitHub, go to **Settings ? Pages**.
3. Deploy from the repository branch/folder containing `index.html`.
4. Open the Pages URL GitHub gives you.

If you later regenerate the map, replace both files together.
