# Purchase Order General Relation

## Required References

| Purchase Order General Field | Required Template | Reference Field    |
| ---------------------------- | ----------------- | ------------------ |
| `supplierCode`               | `supplierMaster`  | `supplierCode`     |
| `itemCode`                   | `itemMaster`      | `itemCode`         |
| `vendorUnitCode`             | `unitMaster`      | `internalUnitCode` |

## Submit Order

```text
1. supplierMaster
2. itemMaster
3. unitMaster
4. purchaseOrderGeneral
```

## Notes

- `supplierCode` must exist in `supplierMaster.supplierCode`.
- `itemCode` must exist in `itemMaster.itemCode`.
- `vendorUnitCode` must refer to `unitMaster.internalUnitCode`.
- If one of the reference values does not exist, Purchase Order General may not be processed completely.
