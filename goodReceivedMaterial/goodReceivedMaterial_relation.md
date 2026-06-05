# Good Received Material Relation

## Required References

| Good Received Material Field | Required Template       | Reference Field    |
| ---------------------------- | ----------------------- | ------------------ |
| `poNo`                       | `purchaseOrderMaterial` | `poNo`             |
| `orderNo`                    | `salesOrder`            | `orderNo`          |
| `lineItemNo`                 | `purchaseOrderMaterial` | `lineItemNo`       |
| `vendorUnitCode`             | `unitMaster`            | `internalUnitCode` |
| `internalUnitCode`           | `unitMaster`            | `internalUnitCode` |

## Submit Order

```text
1. supplierMaster
2. itemMaster
3. unitMaster
4. salesOrder
5. purchaseOrderMaterial
6. goodReceivedMaterial
```

## Notes

- `poNo` must exist in `purchaseOrderMaterial.poNo`.
- `orderNo` must exist in `salesOrder.orderNo`.
- `lineItemNo` must exist in `purchaseOrderMaterial.lineItemNo`.
- `vendorUnitCode` must refer to `unitMaster.internalUnitCode`.
- `internalUnitCode` must refer to `unitMaster.internalUnitCode`.
- If one of the reference values does not exist, Good Received Material may not be processed completely.
