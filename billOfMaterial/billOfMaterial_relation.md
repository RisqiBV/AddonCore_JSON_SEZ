# Bill Of Material Relation

## Required References

| Bill Of Material Field | Required Template | Reference Field    |
| ---------------------- | ----------------- | ------------------ |
| `orderNO`              | `salesOrder`      | `orderNO`          |
| `materialCode`         | `itemMaster`      | `itemCode`         |
| `unitCode`             | `unitMaster`      | `internalUnitCode` |

## Submit Order

```text
1. salesOrder
2. itemMaster
3. unitMaster
4. billOfMaterial
```

## Notes

- `orderNO` must exist in `salesOrder.orderNO`.
- `materialCode` must refer to `itemMaster.itemCode`.
- `unitCode` must refer to `unitMaster.internalUnitCode`.
- If one of the reference values does not exist, Bill Of Material may not be processed completely.
