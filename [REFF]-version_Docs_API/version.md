# Core-A API — Version History

Release history for Core-A API JSON schemas, payloads, responses, and integration templates.

> 🟢 **Current Version: 1.3.0**  
> **Release Date: October 27, 2026**  
> Added the Return Finish Goods template.

## Version Status

- 🟢 **Active** — The current documentation version used as the integration reference.
- ⚪ **Inactive** — A previous documentation version retained for historical reference.

## Release Overview

| Version   | Release Date | Summary                                                           | Status      |
| :-------- | :----------- | :---------------------------------------------------------------- | :---------- |
| **1.3.0** | 2026-10-27   | Added the Return Finish Goods template                            | 🟢 Active   |
| **1.2.2** | 2026-05-20   | Added Batch to Batch templates                                    | ⚪ Inactive |
| **1.2.1** | 2026-05-20   | Added transaction cancellation contracts                          | ⚪ Inactive |
| **1.2.0** | 2026-05-10   | Added response definitions for JSON schemas                       | ⚪ Inactive |
| **1.1.0** | 2026-04-28   | Reorganized contracts by module and HTTP method                   | ⚪ Inactive |
| **1.0.3** | 2025-04-08   | Added `LineItemNo` to five modules                                | ⚪ Inactive |
| **1.0.2** | 2025-03-03   | Updated Sales Order descriptions and required Finish Goods fields | ⚪ Inactive |
| **1.0.1** | 2025-12-17   | Added `poCust` to selected payloads                               | ⚪ Inactive |
| **1.0.0** | 2025-09-29   | Initial documentation release                                     | ⚪ Inactive |

## Release Details

### 🟢 1.3.0 — October 27, 2026

**Added**

- Return Finish Goods template.

---

<details>
<summary><strong>1.2.2 — May 20, 2026 · Batch to Batch Templates</strong></summary>

### Added

- Batch to Batch templates.

</details>

<details>
<summary><strong>1.2.1 — May 20, 2026 · Transaction Cancellation</strong></summary>

### Added

Transaction cancellation contracts for:

- GoodReceivedMaterial
- GoodDispatchMaterial
- GoodDispatchGeneral
- GoodReceivedFinishGood
- GoodDispatchFinishGood
- routingProduction
- GoodReceivedScrap

</details>

<details>
<summary><strong>1.2.0 — May 10, 2026 · Response Schemas</strong></summary>

### Added

- Response definitions for JSON schemas.

</details>

<details>
<summary><strong>1.1.0 — April 28, 2026 · Contract Structure</strong></summary>

### Changed

- Reorganized JSON contracts into module-based and HTTP method-based folders.

### Added

- Folder structure for `PUT` and `DELETE` contracts.

### Compatibility

- Existing `POST` payload contracts were preserved.

</details>

<details>
<summary><strong>1.0.3 — April 8, 2025 · LineItemNo Field</strong></summary>

### Added

The `LineItemNo` field in:

- BOM
- PurchaseOrderMaterial
- PurchaseOrderGeneral
- GoodReceivedMaterial
- GoodReceivedGeneral

</details>

<details>
<summary><strong>1.0.2 — March 3, 2025 · Sales Order & Finish Goods</strong></summary>

### Changed

- Updated descriptions in `SalesOrder.JSON`.
- Set `colorFinishGood` and `sizeFinishGoodCode` as required fields in `goodDispatchFinishgood` and `Sales`.

</details>

<details>
<summary><strong>1.0.1 — December 17, 2025 · poCust Field</strong></summary>

### Added

The `poCust` field in the following payloads:

- `routingProduction.json`
- `goodReceivedFinishgood.json`

</details>

<details>
<summary><strong>1.0.0 — September 29, 2025 · Initial Release</strong></summary>

### Added

- Initial Core-A API integration documentation.

</details>
