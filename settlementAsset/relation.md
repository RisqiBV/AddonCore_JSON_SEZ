# Settlement Asset Relation

## Required References

| Settlement Asset Field | Required Template     | Reference Field    |
| ---------------------- | --------------------- | ------------------ |
| `unitCode`             | `unitMaster`          | `internalUnitCode` |
| `grpoRef`              | `goodReceivedGeneral` | `transactionNo`    |
| `lineItemNoGR`         | `goodReceivedGeneral` | `lineItemNo`       |

## Submit Order

```text
1. unitMaster
2. goodReceivedGeneral
3. settlementAsset
```

## Validation Flow

```text
1. Read locationId from the API token.
2. Validate unitCode against coreA_Unit.internalUnitCode using the same locationId.
3. Validate grpoRef against coreA_GoodReceivedGeneral.transactionNo using the same locationId.
4. If the transactionNo does not exist, reject grpoRef.
5. If the transactionNo exists, validate lineItemNoGR within the referenced transactionNo.
6. If the transactionNo + lineItemNoGR combination does not exist, reject lineItemNoGR.
7. If all references are valid, continue the Settlement Asset saving process.
```

## Notes

- `unitCode` must exist in `unitMaster.internalUnitCode`
- `grpoRef` must exist in `goodReceivedGeneral.transactionNo`
- `lineItemNoGR` must exist under the Good Received General transaction specified by `grpoRef`.
- The `grpoRef` and `lineItemNoGR` validation must use the combination of `transactionNo` and `lineItemNo`.
- A valid `lineItemNoGR` from another Good Received General transaction cannot be used.
- If `unitCode`, `grpoRef`, or `lineItemNoGR` is invalid, the Settlement Asset transaction will be rejected and will not be saved.
- The Settlement Asset saving process is executed only after all reference validations are successfully completed.
