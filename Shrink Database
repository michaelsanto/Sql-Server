USE [DatabaseName];  
GO  
-- Truncate the log by changing the database recovery model to SIMPLE.  
ALTER DATABASE [DatabaseName]  
SET RECOVERY SIMPLE;  
GO  
-- Shrink the truncated log file to 1 MB.  
DBCC SHRINKFILE ([DatabaseName]_Log, 1);  
GO  
-- Reset the database recovery model.  
ALTER DATABASE [DatabaseName]  
SET RECOVERY FULL;  
GO
