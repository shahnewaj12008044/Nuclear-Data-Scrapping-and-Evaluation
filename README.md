# Nuclear-Data-Scrapping-and-Evaluation

Neutron cross-section work in Google Colab: TALYS 2.2 calculations and
EXFOR / JEFF data retrieval for Fe and Cr isotopes, by Md Shahnewaj Al Hasan
(University of Chittagong, NDA Lab).

## Notebooks

### `notebooks/fe-54/` · `fe-56/` · `fe-57/` · `fe-58/`
TALYS output parsing and excitation-function plots (pandas + Matplotlib):
- `Fe-54-(n,p)-54Mn.ipynb`, `Fe-54-np.ipynb` — 54Fe(n,p)54Mn
- `Fe-56-(n,p).ipynb`, `updated-fe-56-(n,p).ipynb` — 56Fe(n,p)56Mn
- `fe-56-(n,inl).ipynb` — 56Fe(n,n′) inelastic scattering
- `Fe-57-(n,p).ipynb` — 57Fe(n,p)
- `Fe-58-(n,p)-jun-2026.ipynb` and `Fe-58-(n,p)-aug-2026.ipynb` — 58Fe(n,p),
  two versions (June and August 2026)

### `notebooks/scrapers/`
- `exfor-cr-scraper.ipynb` — EXFOR data collector for 50Cr and 53Cr,
  reactions (n,γ), (n,α), (n,p), via `x4i3`; writes one consolidated CSV
  plus a ZIP archive
- `scraping-jeff-data.ipynb` — downloads the JEFF-4.0 neutron data library
  (OECD-NEA) for local use

### `notebooks/untitled/`
- `Untitled2.ipynb` — EXFOR collector variant for 50Cr / 53Cr
- `Untitled0.ipynb`, `Untitled1.ipynb` — empty Colab templates (no code)

## How to run

Open a notebook in Google Colab or Jupyter. The first cell of each notebook
installs its dependencies (`pandas`, `numpy`, `matplotlib`, `openpyxl`, and
`x4i3` for the EXFOR scrapers). TALYS output files and downloaded libraries
are not included — point the notebooks at your local copies.
