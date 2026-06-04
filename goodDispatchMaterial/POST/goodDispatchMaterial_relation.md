# Good Dispatch Material Relation

## Required References

| Good Dispatch Material Field | Required Template      | Reference Field    |
| ---------------------------- | ---------------------- | ------------------ |
| `orderNo`                    | `salesOrder`           | `orderNo`          |
| `itemCode`                   | `itemMaster`           | `itemCode`         |
| `unitCode`                   | `unitMaster`           | `internalUnitCode` |
| `batchNo`                    | `goodReceivedMaterial` | `batchNo`          |

## Submit Order

```text
1. itemMaster
2. unitMaster
3. salesOrder
4. goodReceivedMaterial
5. goodDispatchMaterial
```

## Notes

- `orderNo` must exist in `salesOrder.orderNo`.
- `itemCode` must exist in `itemMaster.itemCode`.
- `unitCode` must refer to `unitMaster.internalUnitCode`.
- `batchNo` must exist in `goodReceivedMaterial.batchNo`.
- If one of the reference values does not exist, Good Dispatch Material may not be processed completely.
