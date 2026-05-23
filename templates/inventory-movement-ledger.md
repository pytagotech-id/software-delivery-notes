# Inventory Movement Ledger

Current stock should be explainable from movement history.

## Movement fields

| Field | Example |
|---|---|
| item_id | SKU-001 |
| location_id | WH-01 |
| movement_type | purchase, sale, transfer, return, adjustment |
| quantity_delta | +10 or -3 |
| reference | PO-1021 |
| reason | initial stock, damaged item, stock opname correction |
| actor | admin@example.com |
| created_at | 2026-05-23T10:00:00Z |

## Rules

- Avoid direct stock editing.
- Use adjustment movements for corrections.
- Keep the reason visible.
- Let current quantity be derived from movement history when possible.
