

SQL


exec sp_helprotect @name='tempTblConfigData'  <br/>
查询所有表名
select * from sysobjects where type='U' order by name
