create table store_revenue (id int not null primary key, date datetime,
  brand_id int, store_location varchar(250), revenue float);
insert into store_revenue values (1, 2016-01-01, 1, "United States-CA", 100);
insert into store_revenue values (2, 2016-01-01, 1, "United States-TX", 420);
insert into store_revenue values (3, 2016-01-01, 1, "United States-NY", 142);
insert into store_revenue values (4, 2016-01-02, 1, "United States-CA", 231);
insert into store_revenue values (5, 2016-01-02, 1, "United States-TX", 2342);
insert into store_revenue values (6, 2016-01-02, 1, "United States-NY", 232);
insert into store_revenue values (7, 2016-01-03, 1, "United States-CA", 100);
insert into store_revenue values (8, 2016-01-03, 1, "United States-TX", 420);
insert into store_revenue values (9, 2016-01-03, 1, "United States-NY", 3245);
insert into store_revenue values (10, 2016-01-04, 1, "United States-CA", 34);
insert into store_revenue values (11, 2016-01-04, 1, "United States-TX", 3);
insert into store_revenue values (12, 2016-01-04, 1, "United States-NY", 54);
insert into store_revenue values (13, 2016-01-05, 1, "United States-CA", 45);
insert into store_revenue values (14, 2016-01-05, 1, "United States-TX", 423);
insert into store_revenue values (15, 2016-01-05, 1, "United States-NY", 234);
insert into store_revenue values (16, 2016-01-01, 2, "United States-CA", 234);
insert into store_revenue values (17, 2016-01-01, 2, "United States-TX", 234);
insert into store_revenue values (18, 2016-01-01, 2, "United States-NY", 142);
insert into store_revenue values (19, 2016-01-02, 2, "United States-CA", 234);
insert into store_revenue values (20, 2016-01-02, 2, "United States-TX", 3423);
insert into store_revenue values (21, 2016-01-02, 2, "United States-NY", 2342);
insert into store_revenue values (22, 2016-01-03, 2, "United States-CA", 234234);
insert into store_revenue values (23, 2016-01-06, 3, "United States-TX", 3);
insert into store_revenue values (24, 2016-01-03, 2, "United States-TX", 3);
insert into store_revenue values (25, 2016-01-03, 2, "United States-NY", 234);
insert into store_revenue values (26, 2016-01-04, 2, "United States-CA", 2);
insert into store_revenue values (27, 2016-01-04, 2, "United States-TX", 2354);
insert into store_revenue values (28, 2016-01-04, 2, "United States-NY", 45235);
insert into store_revenue values (29, 2016-01-05,2, "United States-CA", 23);
insert into store_revenue values (30, 2016-01-05, 2, "United States-TX", 4);
insert into store_revenue values (31, 2016-01-05, 2, "United States-NY", 124);

create table marketing_data ( id int not null primary key, date datetime, geo varchar(2), impressions float, clicks float );
insert into marketing_data values (1, 2016-01-01, "TX", 2532, 45);
insert into marketing_data values (2, 2016-01-01, "CA", 3425, 63);
insert into marketing_data values (3, 2016-01-01, "NY", 3532, 25);
insert into marketing_data values (4, 2016-01-01, "MN", 1342, 784);
insert into marketing_data values (5, 2016-01-02, "TX", 3643, 23);
insert into marketing_data values (6, 2016-01-02, "CA", 1354, 53);
insert into marketing_data values (7, 2016-01-02,"NY", 4643, 85);
insert into marketing_data values (8, 2016-01-02, "MN", 2366, 85);
insert into marketing_data values (9, 2016-01-03, "TX", 2353, 57);
insert into marketing_data values (10, 2016-01-03, "CA", 5258, 36);
insert into marketing_data values (11, 2016-01-03, "NY", 4735, 63);
insert into marketing_data values (12, 2016-01-03, "MN", 5783, 87);
insert into marketing_data values (13, 2016-01-04, "TX", 5783, 47);
insert into marketing_data values (14, 2016-01-04, "CA", 7854, 85);
insert into marketing_data values (15, 2016-01-04, "NY", 4754, 36);
insert into marketing_data values (16, 2016-01-04, "MN", 9345, 24);
insert into marketing_data values (17, 2016-01-05, "TX", 2535, 63);
insert into marketing_data values (18, 2016-01-05, "CA", 4678, 73);
insert into marketing_data values (19, 2016-01-05, "NY", 2364, 33);
insert into marketing_data values (20, 2016-01-05, "MN", 3452, 25);

/* Question 3: Merge these two datasets so we
can see impressions, clicks, and revenue together
by date and geo. Please ensure all records from
each table are accounted for.
 */
select
    geo, impressions, clicks
from
    marketing_data
union
select
    store_location, revenue, date
from
    store_revenue;
