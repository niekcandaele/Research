# MySQL performance on enum columns with or without index

In this notebook I check what the performance difference is on MySQL 5.7 for enum columns with and without an index.


In the `db.log` file you will find logs of MySQL with execution time and index used. To keep this file small, I deleted all `INSERT INTO` statements from it.

`sed -i '/INSERT INTO/d' ./db.log`