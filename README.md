# RePEC Archive – Impumelelo Economic Growth Lab

**Handle:** `RePEc:IMPBER`  
**Series:** Research Notes  
**Institution:** Bureau for Economic Research, Impumelelo Economic Growth Lab  
**GitHub Pages URL:** `https://RoyHavemann.github.io/repec-archive-imp/`

---

## Folder Structure

```
repec-archive-imp/
├── index.html                        ← Human-readable homepage
├── README.md                         ← This file
└── RePEc/
    └── IMPBER/
        ├── arch.rdf                  ← Archive-level metadata
        ├── seri.rdf                  ← Series-level metadata
        └── wpaper/
            └── wpaper.rdf            ← All paper metadata (21 papers)
```

---

## Step 1: Create the GitHub Repository

1. Go to [github.com](https://github.com) and log in as **RoyHavemann**
2. Click **New repository**
3. Name it: `repec-archive-imp`
4. Set it to **Public**
5. Click **Create repository**

---

## Step 2: Upload the Files

### Option A – Upload via GitHub web interface (easiest)
1. In your new repo, click **Add file → Upload files**
2. Drag the entire contents of the unzipped folder into the upload area
3. Add commit message: `Initial RePEC archive setup`
4. Click **Commit changes**

### Option B – Use Git on your computer
```bash
git clone https://github.com/RoyHavemann/repec-archive-imp.git
# Copy all files into the cloned folder
git add .
git commit -m "Initial RePEC archive setup"
git push
```

---

## Step 3: Enable GitHub Pages

1. In your repo, go to **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Select branch: **main**, folder: **/ (root)**
4. Click **Save**
5. Wait 1–2 minutes, then visit: `https://RoyHavemann.github.io/repec-archive-imp/`

---

## Step 4: Update Your Email

Before registering, update the placeholder email in these two files:
- `RePEc/IMPBER/arch.rdf` — line: `Maintainer-Email:`
- `RePEc/IMPBER/seri.rdf` — line: `Maintainer-Email:`

---

## Step 5: Register with RePEC

1. Go to [repec.org/archives.html](https://repec.org/archives.html)
2. Click **Register a new archive**
3. Fill in:
   - **Archive handle:** `IMPBER`
   - **Archive URL:** `https://RoyHavemann.github.io/repec-archive-imp/RePEc/IMPBER/`
   - **Maintainer name:** Roy Havemann
   - **Maintainer email:** *(your real email)*
4. Submit and wait for confirmation (usually 1–3 business days)

---

## Adding New Papers

To add a new paper, open `RePEc/IMPBER/wpaper/wpaper.rdf` and append a new block:

```
Template-Type: ReDIF-Paper 1.0
Handle: RePEc:IMPBER:wpaper:22
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

- RePEC registration: https://repec.org/archives.html
- ReDIF format guide: https://repec.org/docs/redif.html
- Check your archive after registration: https://ideas.repec.org/s/IMPBER/wpaper.html
