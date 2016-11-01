SELECT col3, col4, count(DISTINCT(uniq)) AS cnt
FROM
(
SELECT col1 || '__' || col2 AS uniq, col3, col4
FROM databas.table
WHERE col5 = 'cond0'
AND col3 IN ('cond1', 'cond2')
AND col6 BETWEEN cond3 AND cond4
)
AS foo
GROUP BY col3, col4
ORDER BY col3 ASC, cnt DESC
;
