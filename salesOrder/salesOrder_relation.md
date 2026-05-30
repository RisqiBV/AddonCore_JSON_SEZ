# Sales Order Relation

## Required References

| Sales Order Field    | Required Template | Reference Field    |
| -------------------- | ----------------- | ------------------ |
| `brandCode`          | `brandMaster`     | `brandCode`        |
| `internalUnitCode`   | `unitMaster`      | `internalUnitCode` |
| `sizeFinishGoodCode` | `sizeMaster`      | `sizeCode`         |

## Submit Order

```text
1. brandMaster
2. unitMaster
3. sizeMaster
4. salesOrder
```
