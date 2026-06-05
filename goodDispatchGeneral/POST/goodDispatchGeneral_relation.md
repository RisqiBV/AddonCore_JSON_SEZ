# Good Dispatch General Relation

## Required References

| Good Dispatch General Field | Required Template | Reference Field    |
| --------------------------- | ----------------- | ------------------ |
| `itemCode`                  | `itemMaster`      | `itemCode`         |
| `unitCode`                  | `unitMaster`      | `internalUnitCode` |

## Submit Order

```text
1. itemMaster
2. unitMaster
3. goodDispatchGeneral
```

## Notes

- `itemCode` must exist in `itemMaster.itemCode`.
- `unitCode` must refer to `unitMaster.internalUnitCode`.
- If one of the reference values does not exist, Good Dispatch General may not be processed completely.