# Purchase Order Material Relation

## Required References

| Purchase Order Material Field | Required Template | Reference Field    |
| ----------------------------- | ----------------- | ------------------ |
| `supplierCode`                | `supplierMaster`  | `supplierCode`     |
| `orderNo`                     | `salesOrder`      | `orderNo`          |
| `itemCode`                    | `itemMaster`      | `itemCode`         |
| `vendorUnitCode`              | `unitMaster`      | `internalUnitCode` |

## Submit Order

```text
1. supplierMaster
2. itemMaster
3. unitMaster
4. salesOrder
5. purchaseOrderMaterial
```
