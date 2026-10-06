# Equipment record cleaning report

## Summary

- Input rows: 10
- Output records retained: 9
- Rows removed: 1 (source row 6 was an empty object)
- Duplicate `item_id` rows retained: `EQ01` (source rows 1 and 4) and `EQ02` (source rows 2 and 5)

## Data handling

- Leading/trailing whitespace was trimmed from text fields. Original input remains unchanged in `practice/03-equipment/equipment.json`.
- Quantities were preserved as supplied; no missing or negative quantity was replaced or altered.
- Source row numbers and validation flags are included in `cleaned-equipment.json`.
- Source row 7 has an empty quantity and is flagged `quantity_missing`.
- Source row 8 has quantity `-1` and is flagged `quantity_negative`.

## Verification

- Parsed the output JSON and confirmed 9 records and `removed_count` 1.
- Confirmed the duplicate IDs and their source rows are both present.
- Confirmed rows 7 and 8 retain their original quantity values and carry the corresponding flags.
