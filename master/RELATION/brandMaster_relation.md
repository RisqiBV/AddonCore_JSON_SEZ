# Brand Master Relation

## Required References

| Brand Master Field | Required Template | Reference Field |
| ------------------ | ----------------- | --------------- |
| `customerCode`     | `customerMaster`  | `customerCode`  |

## Submit Order

```text
1. customerMaster
2. brandMaster
```

## Notes

- `customerCode` must exist in `customerMaster.customerCode`.
- If `customerCode` does not exist, Brand Master may not be processed completely.
