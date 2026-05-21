
# Time Intelligence DAX

## Year-to-Date (YTD)

```DAX
YTD Sales =
TOTALYTD(
    SUM(Sales[Amount]),
    Date[Date]
)
