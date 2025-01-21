# Converting columns to row in postgresql

select 

col1

, col2

, col3

, col_name

, value1

, value2

from table_name

, LATERAL (values

('ABC', abc1, abc2)

, ('BCD', bcd1, bcd2)

) AS vals(col_name, value1, value2)
;
