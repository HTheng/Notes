

#SQL


exec sp_helprotect @name='tempTblConfigData'  <br/>
查询所有表名</br>
select * from sysobjects where type='U' order by name</br>


--复制结构+数据</br>
select * into [newtable] from [oldtable]

--只复制结构</br>
select * into [newtable] from [oldtable]
 where 1=0

--复制到临时表</br> 
select * into #temptablename from 数据库名.dbo.原表名 where 1=0 

--COALESCE(,) 和 select top 1 1  的使用 </br>
SELECT CAST(COALESCE((SELECT TOP 1  1 FROM OPD.dbo.ELLLot WHERE Business_Date = '2017-02-03'), 0) AS VARCHAR) AS Result


[Google](https://www.google.com)
