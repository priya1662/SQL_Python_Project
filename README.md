-- database created
create database startups;

select * from startups.table limit 1000;

-- Drop the remarks column
Alter table startups.table
drop column remarks;
commit;

-- Handling Null values
select count(*) from startups.table
where AmountInUSD is null;

-- Checking for duplicates
Select count(*) from startups.table
group by sno
having sno > 1;

select * from startups.table limit 1000;

