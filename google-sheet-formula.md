### Import data from another Google Sheet, and show only selected columns
 The `Col1, .., ColN` are the column index, must be written in this static name `Col1`
```C#
=QUERY(
  IMPORTRANGE("https://docs.google.com/spreadsheets/d/URL_TO_GOOGLE_SHEET", "Sheet1!A1:D"),
  "SELECT Col1, Col3, Col4 where Col2 is NULL",
  1
)
```
