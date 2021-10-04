
This file folder is used to store files related to the continuing development of USLCI features and curation workflow. 


# 2021_Q3_v1 Fall Release, Erratas Correction Script

A bug has caused some elementary flows to display with 'default providers', that is, processes designated as the provider of the elementary flow input or output. The default providers field is intended for technospheric, i.e., intermediate flows only. To correct this in your local database version in openLCA, you may use the following script:

```sql
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39306;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39825;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39799;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39752;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39792;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39861;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39724;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39812;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39884;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39786;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39832;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39836;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39776;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39801;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 39818;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 44015;
UPDATE tbl_exchanges set F_DEFAULT_PROVIDER = 0 where ID = 59835;
```

