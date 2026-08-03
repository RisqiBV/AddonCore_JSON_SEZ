# Good Received Material Without PO Relation

## Required References

| Good Received Material Without PO Field | Required Template | Reference Field    |
| --------------------------------------- | ----------------- | ------------------ |
| `itemCode`                              | `itemMaster`      | `itemCode`         |
| `unitCode`                              | `unitMaster`      | `internalUnitCode` |

## Submit Order

```text
1. itemMaster
2. unitMaster
3. goodReceivedMaterialWithoutPo
```

## Notes

- `itemCode` must exist in `itemMaster.itemCode`.
- `unitCode` must refer to `unitMaster.internalUnitCode`.
- Good Received Material Without PO does not require a Purchase Order reference.
- Good Received Material Without PO does not require a Sales Order reference.
- If `itemCode` or `unitCode` does not exist in the corresponding master data, the Good Received Material Without PO transaction cannot be processed completely.
