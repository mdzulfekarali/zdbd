# ZDBD
## Zoonotic Diseases Research Documents in Bangladesh

ZDBD is a searchable bibliometric discovery website for research documents related to zoonotic diseases in Bangladesh. Its dataset is curated from a Scopus export.

**Website:** Enable GitHub Pages in the repository settings to publish this site.

## Add the Scopus Excel dataset

The website expects the workbook at:

`data/zdbd_scopus_records.xlsx`

1. In this repository, create a folder named `data`.
2. Upload your workbook `Zoonotic_BD_Duplication_Removed_Excel_Title+Journal.xlsx` into that folder.
3. Rename the uploaded file to **`zdbd_scopus_records.xlsx`** (or edit `DATA_URL` near the beginning of the JavaScript in `index.html` to match your filename).
4. The first worksheet should contain these column headers:
   - `Title`
   - `Year`
   - `Source`
   - `DOI`
   - `Abstract/Background`
   - `Keywords`
   - `PubMed.ID`
   - `Language`
   - `Document type`

The site reads the first worksheet in the workbook. It processes the spreadsheet in the visitor's browser; the workbook is not uploaded to a third-party data-processing service by the site. The page loads the SheetJS and Chart.js libraries from jsDelivr and fonts from Google Fonts.

## Publish with GitHub Pages

1. Open **Settings → Pages** in this repository.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Select branch **main** and folder **/(root)**, then save.
4. If this repository is private, change it to **Public** first unless your GitHub plan supports Pages for private repositories. Do not publish sensitive or restricted data.

The expected website address is:

`https://mdzulfekarali.github.io/zdbd/`

## Search and dashboard

Visitors can search titles, abstracts, keywords, source/journal and DOI, and filter by year, source, document type and language. Summary metrics and charts are calculated from the workbook records.

## Data scope and responsible use

- ZDBD reflects only the records included in the supplied Scopus export and the search strategy/date used to collect them.
- It should not be described as a complete census of all zoonotic disease research in Bangladesh unless a reproducible search and screening process supports that claim.
- Article metadata is provided for discovery. DOI links direct visitors to external publication pages; the site does not host article full text.
- Respect Scopus/Elsevier terms and publisher copyright. Do not upload copyrighted full-text PDFs without permission or a valid self-archiving basis.
- ZDBD is an independent project and is not affiliated with or endorsed by Elsevier or Scopus.

## Project maintainer

Repository: https://github.com/mdzulfekarali/zdbd
