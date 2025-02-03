A [[Database]] View is the result of a stored query on the data, which can be queried as if was a database persisteng object. There are two kind of views, [[Materialized views]]. which stores the result of the view in disk, and non-materialized views, which executes its query only when the view is called.

Views can be selected from `information_schema.views` table.

Views can be updated if:
* The view is made up of one table 
* No aggregate or window function are used
#### Code
`CREATE VIEW AS ...`
## Redefining a view
`CREATE OR REPLACE VIEW view_name AS new_query`
A view can be redefined under the following circunstances:
* new_query must generate the same column names, order and data types as the old one.
* Column output may be different
* New columns may be added at the end



