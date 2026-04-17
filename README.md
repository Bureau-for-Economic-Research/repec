# RePEC Archive – Impumelelo Economic Growth Lab

**Handle:** `RePEc:cxs`
**Series:** Research Notes
**Institution:** Bureau for Economic Research, Impumelelo Economic Growth Lab
**GitHub Pages URL:** `https://Bureau-for-Economic-Research.github.io/repec/`

---

## Folder Structure

```
repec/
├── index.html                        ← Human-readable homepage
├── README.md                         ← This file
└── RePEc/
    └── cxs/
        ├── cxsarch.rdf                  ← Archive-level metadata
        ├── cxsseri.rdf                  ← Series-level metadata
        └── wpaper/
            └── wpaper.rdf            ← All paper metadata (21 papers)
```

---

## Registering with RePEC

Email the following URL to RePEC to complete registration:
`https://Bureau-for-Economic-Research.github.io/repec/RePEc/cxs/`

Before sending, update the placeholder email in:
- `RePEc/cxs/arch.rdf` — line: `Maintainer-Email:`
- `RePEc/cxs/seri.rdf` — line: `Maintainer-Email:`

---

## Adding New Papers

To add a new paper, edit `RePEc/cxs/wpaper/wpaper.rdf` and append:

```
Template-Type: ReDIF-Paper 1.0
Handle: RePEc:cxs:wpaper:22
Title: Your Paper Title Here
Author-Name: First Author
Author-Name: Second Author
Abstract: Your abstract here.
Year: 2026
File-URL: https://www.ber.ac.za/Documents/ViewMode/your-document-id
File-Format: Application/pdf
Keywords: keyword1, keyword2, South Africa
Classification-JEL: O55
```

Also add the paper to `index.html` under the appropriate year heading.

---

## Useful RePEC Links

- ReDIF format guide: https://repec.org/docs/redif.html
- Check your archive after registration: https://ideas.repec.org/s/cxs/wpaper.html
- RePEC checker: https://econpapers.repec.org/check/
