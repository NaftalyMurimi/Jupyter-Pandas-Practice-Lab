# Self-check numbers (open AFTER you finish each day)

## Day 3 - production raw file
- Raw rows: 825  (800 original + 25 exact duplicate rows) -> after drop_duplicates you should have 800
- Production-line spellings in raw data: ['LINE A ', 'LINE B ', 'LINE C ', 'LINE D ', 'LINE E ', 'Line A', 'Line B', 'Line C', 'Line D', 'Line E', 'Line-A', 'Line-B', 'Line-C', 'Line-D', 'Line-E', 'line a', 'line b', 'line c', 'line d', 'line e'] -> must become 5 clean values
- Placeholder text 'N/A' in units_produced: 6 rows; sensor-error temperature 999.0: 4 rows
- Dates: 12 rows are in dd/mm/yyyy format, the rest yyyy-mm-dd
- Lines with clearly highest defect rate: Line C and Line E. Night shift is worse than other shifts.

## Day 5 - bugs in broken notebook
1. read_excel('orders.xlsx') -> wrong filename (file is day5_orders.xlsx) -> FileNotFoundError
2. Sheet has 3 junk rows above header -> columns show as Unnamed; use header=3 (or skiprows=3)
3. Column is 'Order Date ' with trailing space -> KeyError; clean with df.columns = df.columns.str.strip()
4. unit_price is text like '$45.20' -> TypeError / wrong maths; strip '$' and convert to float
5. 'Region' vs 'region' -> KeyError (column names are case-sensitive)
6. numpy never imported + 'monthly' used before it is defined -> NameError (execution order)
7. '/output/' folder does not exist -> OSError; use a relative path like 'output/clean_orders.csv' and os.makedirs

## Day 6 - ML dataset
- 1,200 rows, ~8% defective batches (imbalanced -> accuracy alone is misleading)
- Missing values: 30 in humidity_pct, 25 in supplier_quality_score

## Day 7 - deliveries
- Raw rows: 718 (700 + 18 duplicates); 5 negative quantity_ordered values (-500); supplier names inconsistent (case/trailing spaces)
- PolyMetal and TechSource are the slowest suppliers; PolyMetal has the highest rejection rate.
