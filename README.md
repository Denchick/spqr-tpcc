# SPQR TPC-C test

TPCC-like workload for sysbench 1.0.x. Make sure you are using sysbench 1.0.14 or better!. I am using this repository to test [SPQR](github.com/pg-sharding/spqr).

## Example

`
sysbench ./tpcc.lua --pgsql-user=denchick --pgsql-password=P@ssw0rd --pgsql-db=denchick --time=3600 --threads=1 --report-interval=1 --tables=1 --scalefrom=1 --scaleto=2 --use_fk=0 --trx_level=RC --db-driver=pgsql --pgsql-port=6432 --pgsql-host=sas-eobe4680fa6vxg4a.db.yandex.net --skipddl=0 prepare
`

There is also run and cleanup commands, for more info see code and original [sysbench repository](github.com/akopytov/sysbench)
