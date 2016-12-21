

#SQL


exec sp_helprotect @name='tempTblConfigData'  <br/>
查询所有表名
select * from sysobjects where type='U' order by name


--复制结构+数据
select * into [CMD].[dbo].[AppTrackingDataFlow_Backup1221] from [CMD].[dbo].[AppTrackingDataFlow]

--只复制结构 
select * into [CMD].[dbo].[AppTrackingDataFlow_Backup1221] from [CMD].[dbo].[AppTrackingDataFlow]
 where 1=0

--复制到临时表
select * into #temptablename from 数据库名.dbo.原表名 where 1=0 


