# AddonCore_JSON_SEZ

Addon Finance Indonesia | Data Contracts (JSON) | Special Economic Zone - Core

# JSON Schema — PT Addon Finance Indonesia

This repository provides reference data and schema assets used by PT Addon Finance Indonesia for item master classification and unit-of-measure interoperability.

---

## 1) Category Codes (for `itemMaster.json`)

These category codes standardize how items are grouped across systems. Use them whenever you define an item in `itemMaster.json`.

| CategoryCode | Description           |
| -----------: | --------------------- |
|            1 | Bahan Baku            |
|            2 | Bahan Penolong        |
|            3 | Bahan Habis Pakai     |
|            4 | Barang Dagangan       |
|            5 | Mesin dan Peralatan   |
|            6 | Barang dalam proses   |
|            7 | Barang Jadi           |
|            8 | Barang Reject & Scrap |

**Files**

- CSV: `refs/category-codes.csv`
- JSON: `refs/category-codes.json`

**Intended Use**

- Acts as a controlled vocabulary for item categories.
- Prevents free-text drift and ensures reporting consistency (inventory, costing, customs).

---

## 2) INSW Unit Catalogue

The **INSW (Indonesia National Single Window) Unit Catalogue** enumerates codes and descriptions for units-of-measure commonly referenced in customs and trade processes.  
We publish the catalogue in two formats:

- **CSV (authoritative)**: `refs/list-of-unit-insw.csv`
- **Markdown (human-readable)**: `refs/list-of-unit-insw.md` (full table view)

> The CSV is the single source of truth. The Markdown is generated from it for documentation.

### Quick Preview (first 10 rows)

```csv
Code,Description
6,small spray
8,heat lot
10,group
11,outfit
13,ration
14,shot
15,stick
16,hundred fifteen kg drum
17,hundred lb drum
18,fiftyfive gallon (US) drum
```
