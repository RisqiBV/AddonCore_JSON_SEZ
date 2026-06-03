# Good Received General Relation

## Required References

| Good Received General Field | Required Template      | Reference Field    |
| --------------------------- | ---------------------- | ------------------ |
| `poNo`                      | `purchaseOrderGeneral` | `poNo`             |
| `itemCode`                  | `itemMaster`           | `itemCode`         |
| `vendorUnitCode`            | `unitMaster`           | `internalUnitCode` |
| `internalUnitCode`          | `unitMaster`           | `internalUnitCode` |
| `lineItemNoPo`              | `purchaseOrderGeneral` | `lineItemNo`       |

## Submit Order

```text
1. supplierMaster
2. itemMaster
3. unitMaster
4. purchaseOrderGeneral
5. goodReceivedGeneral
```

## Notes

- `poNo` must exist in `purchaseOrderGeneral.poNo`.
- `itemCode` must exist in `itemMaster.itemCode`.
- `vendorUnitCode` must refer to `unitMaster.internalUnitCode`.
- `internalUnitCode` must refer to `unitMaster.internalUnitCode`.
- `lineItemNoPo` must refer to `purchaseOrderGeneral.lineItemNo`.
- If one of the reference values does not exist, Good Received General may not be processed completely.
