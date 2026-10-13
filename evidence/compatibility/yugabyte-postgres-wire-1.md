<!-- fetched 2026-10-13 from https://docs.yugabyte.com/stable/api/ysql/ by sweep-shape-compat.py; text extracted from the provider's own page -->

YSQL API reference | YugabyteDB Docs 
 Ask AI about " " 
 OR Ask AI 
 Star us on Github 
 Join us on Slack 
 Start Now 
 YugabyteDB Aeon Try our fully-managed cloud DBaaS for free. No credit card required Sign up 
 YugabyteDB Try our open source distributed SQL database on your laptop. Download 
 Products 
 YugabyteDB The open source distributed SQL database 
 YugabyteDB Anywhere Self-managed cloud DBaaS 
 YugabyteDB Aeon Fully-managed cloud DBaaS 
 YugabyteDB Voyager Database migration service 
 Develop 
 Integrations 
 API 
 SQL APIs 
 YSQL 
 YCQL 
 Clients 
 ysqlsh 
 ycqlsh 
 Management APIs 
 YugabyteDB Anywhere API 
 YugabyteDB Aeon API 
 FAQ 
 Releases 
 YugabyteDB 
 YugabyteDB Anywhere 
 YugabyteDB Aeon 
 YugabyteDB Voyager 
 YugabyteDB Clients 
 Tech Advisories 
 Docs Menu
 API 
 YSQL 
 The SQL language 
 SQL statements 
 ABORT 
 ALTER AGGREGATE 
 ALTER DATABASE 
 ALTER DEFAULT PRIVILEGES 
 ALTER DOMAIN 
 ALTER FOREIGN DATA WRAPPER 
 ALTER FOREIGN TABLE 
 ALTER FUNCTION 
 ALTER GROUP 
 ALTER INDEX 
 ALTER MATERIALIZED VIEW 
 ALTER POLICY 
 ALTER PROCEDURE 
 ALTER PUBLICATION 
 ALTER ROLE 
 ALTER ROUTINE 
 ALTER SCHEMA 
 ALTER SEQUENCE 
 ALTER SERVER 
 ALTER TABLE 
 ALTER TABLESPACE 
 ALTER TYPE 
 ALTER USER 
 ANALYZE 
 BEGIN 
 CALL 
 CLOSE 
 COMMENT 
 COMMIT 
 COPY 
 CREATE AGGREGATE 
 CREATE CAST 
 CREATE DATABASE 
 CREATE DOMAIN 
 CREATE EXTENSION 
 CREATE FOREIGN DATA WRAPPER 
 CREATE FOREIGN TABLE 
 CREATE FUNCTION 
 CREATE GROUP 
 CREATE INDEX 
 CREATE MATERIALIZED VIEW 
 CREATE OPERATOR 
 CREATE OPERATOR CLASS 
 CREATE POLICY 
 CREATE PROCEDURE 
 CREATE PUBLICATION 
 CREATE ROLE 
 CREATE RULE 
 CREATE SCHEMA 
 CREATE SEQUENCE 
 CREATE SERVER 
 CREATE TABLE 
 CREATE TABLE AS 
 CREATE TABLESPACE 
 CREATE TRIGGER 
 CREATE TYPE 
 CREATE USER 
 CREATE USER MAPPING 
 CREATE VIEW 
 CREATE_REPLICATION_SLOT 
 DEALLOCATE 
 DECLARE 
 DELETE 
 DO 
 DROP AGGREGATE 
 DROP CAST 
 DROP DATABASE 
 DROP DOMAIN 
 DROP EXTENSION 
 DROP FOREIGN DATA WRAPPER 
 DROP FOREIGN TABLE 
 DROP FUNCTION 
 DROP GROUP 
 DROP INDEX 
 DROP MATERIALIZED VIEW 
 DROP OPERATOR 
 DROP OPERATOR CLASS 
 DROP OWNED 
 DROP POLICY 
 DROP PROCEDURE 
 DROP PUBLICATION 
 DROP ROLE 
 DROP RULE 
 DROP SCHEMA 
 DROP SEQUENCE 
 DROP SERVER 
 DROP TABLE 
 DROP TABLESPACE 
 DROP TRIGGER 
 DROP TYPE 
 DROP USER 
 DROP VIEW 
 DROP_REPLICATION_SLOT 
 END 
 EXECUTE 
 EXPLAIN 
 FETCH 
 GRANT 
 IMPORT FOREIGN SCHEMA 
 INSERT 
 LISTEN, NOTIFY, and UNLISTEN 
 LOCK 
 MOVE 
 PREPARE 
 REASSIGN OWNED 
 REFRESH MATERIALIZED VIEW 
 RELEASE SAVEPOINT 
 RESET 
 REVOKE 
 ROLLBACK 
 ROLLBACK TO SAVEPOINT 
 SAVEPOINT 
 SELECT 
 SET 
 SET CONSTRAINTS 
 SET ROLE 
 SET SESSION AUTHORIZATION 
 SET TRANSACTION 
 SHOW 
 SHOW TRANSACTION 
 START TRANSACTION 
 START_REPLICATION 
 TRUNCATE 
 UPDATE 
 VALUES 
 Temporary schema-objects 
 Temp tables, views, sequences, and indexes 
 Temp schema-objects of all kinds 
 Globality of metadata and privacy of use of temp objects 
 Paradigm for creating temporary objects 
 Table inheritance 
 WITH clause 
 WITH clause—SQL syntax and semantics 
 Recursive CTE 
 Case study: traversing an employee hierarchy
 Traversing general graphs 
 Graph representation 
 Common code 
 Undirected cyclic graph 
 Directed cyclic graph 
 Directed acyclic graph 
 Rooted tree 
 Unique containing paths 
 Stress testing find_paths() 
 Case study: Bacon Numbers from IMDb
 Bacon numbers for synthetic data 
 Bacon numbers for IMDb data 
 Transaction model for top-level SQL statements 
 Names and identifiers 
 Name resolution in top-level SQL 
 Supporting language elements 
 Built-in functions and operators 
 yb_index_check() 
 yb_hash_code() 
 yb_servers() 
 yb_cancel_transaction() 
 gen_random_uuid() 
 Aggregate functions 
 Informal functionality overview 
 Invocation syntax and semantics 
 Grouping sets, rollup, cube 
 Per function signature and purpose 
 avg(), count(), max(), min(), sum() 
 array_agg, jsonb_agg, jsonb_object_agg, string_agg, range_agg 
 bit_and(), bit_or(), bool_and(), bool_or() 
 variance(), var_pop(), var_samp(), stddev(), stddev_pop(), stddev_samp() 
 linear regression 
 covar_pop(), covar_samp(), corr() 
 regr_%() 
 mode(), percentile_disc(), percentile_cont() 
 rank(), dense_rank(), percent_rank(), cume_dist() 
 Case study: percentile_cont() and the "68–95–99.7" rule
 Case study: linear regression on COVID data
 Download the COVIDcast data 
 Ingest the COVIDcast data 
 Inspect the COVIDcast data 
 Copy the .csv files to staging tables 
 Check staged data conforms to the rules 
 Join the staged data into a single table 
 SQL scripts 
 Create cr_staging_tables() 
 Create cr_copy_from_scripts() 
 Create assert_assumptions_ok() 
 Create xform_to_covidcast_fb_survey_results() 
 ingest-the-data.sql 
 Analyze the COVIDcast data 
 symptoms vs mask-wearing by day 
 Data for scatter-plot for 21-Oct-2020 
 Scatter-plot for 21-Oct-2020 
 SQL scripts 
 analysis-queries.sql 
 synthetic-data.sql 
 Geo-partitioning helper functions 
 yb_is_local_table() 
 yb_server_cloud() 
 yb_server_region() 
 yb_server_zone() 
 Sequence functions 
 currval() 
 lastval() 
 nextval() 
 setval() 
 Window functions 
 Informal functionality overview 
 Invocation syntax and semantics 
 Per function signature and purpose 
 row_number(), rank() and dense_rank() 
 percent_rank(), cume_dist() and ntile() 
 first_value(), nth_value(), last_value() 
 lag(), lead() 
 Tables for the code examples 
 table t1 
 table t2 
 table t3 
 table t4 
 Case study: analyzing a normal distribution
 Bucket allocation scheme 
 do_clean_start.sql 
 cr_show_t4.sql 
 cr_dp_views.sql 
 cr_int_views.sql 
 cr_pr_cd_equality_report.sql 
 cr_bucket_using_width_bucket.sql 
 cr_bucket_dedicated_code.sql 
 do_assert_bucket_ok 
 cr_histogram.sql 
 cr_do_ntile.sql 
 cr_do_percent_rank.sql 
 cr_do_cume_dist.sql 
 do_populate_results.sql 
 do_report_results.sql 
 do_compare_dp_results.sql 
 do_demo.sql 
 Reports 
 Histogram report 
 dp-results 
 compare-dp-results 
 int-results 
 Data types 
 Array 
 array[] constructor 
 Literals 
 Text typecasting and literals 
 Array of primitive values 
 Row 
 Array of rows 
 FOREACH loop (PL/pgSQL) 
 array of DOMAINs 
 Functions and operators 
 ANY and ALL 
 Array comparison 
 Array slice operator 
 Array concatenation 
 Array properties 
 array_agg(), unnest(), generate_subscripts() 
 array_fill() 
 array_position(), array_positions() 
 array_remove() 
 array_replace() / set value 
 array_to_string() 
 string_to_array() 
 Binary 
 Boolean 
 Character 
 Date and time 
 Conceptual background 
 Section contents 
 Timezones and UTC offsets 
 Catalog views 
 Extended_timezone_names 
 Unrestricted full projection 
 Real timezones with DST 
 Real timezones no DST 
 Synthetic timezones no DST 
 Offset/timezone-sensitive operations 
 Timestamptz to/from timestamp conversion 
 Pure 'day' interval arithmetic 
 Four ways to specify offset 
 Name-resolution rules 
 1 case-insensitive resolution 
 2 ~names.abbrev never searched 
 3 'set timezone' string not resolved in ~abbrevs.abbrev 
 4 ~abbrevs.abbrev before ~names.name 
 Helper functions 
 Syntax contexts for offset 
 Recommended practice 
 Typecasting between date-time and text-values 
 Semantics of the date-time data types 
 Date data type 
 Time data type 
 Plain timestamp and timestamptz 
 Interval data type 
 Interval representation 
 Ad hoc examples 
 Representation model 
 Interval value limits 
 Declaring intervals 
 Justify() and extract(epoch...) 
 Interval arithmetic 
 Interval-interval comparison 
 Interval-interval addition and subtraction 
 Interval-number multiplication 
 Moment-moment overloads of "-" 
 Moment-interval overloads of "+" and "-" 
 Custom interval domains 
 Interval utility functions 
 Typecasting between date-time data types 
 Operators 
 Test comparison overloads 
 Test addition overloads 
 Test subtraction overloads 
 Test multiplication overloads 
 Test division overloads 
 General-purpose functions 
 Creating date-time values 
 Manipulating date-time values 
 Current date-time moment 
 Delaying execution 
 Miscellaneous 
 Function age() 
 Function extract() | date_part() 
 Implementations that model the overlaps operator 
 Formatting functions 
 Case study: SQL stopwatch
 Download & install the date-time utilities 
 JSON 
 JSON literals 
 Primitive and compound data types 
 Code example conventions 
 Indexes and check constraints 
 Functions & operators 
 ::jsonb, ::json, ::text (typecast) 
 ->, ->>, #>, #>> (JSON subvalues) 
 - and #- (remove) 
 || (concatenation) 
 = (equality) 
 @> and <@ (containment) 
 ? and ?| and ?& (key or value existence) 
 array_to_json() 
 jsonb_agg() 
 jsonb_array_elements() 
 jsonb_array_elements_text() 
 jsonb_array_length() 
 jsonb_build_object() 
 jsonb_build_array() 
 jsonb_each() 
 jsonb_each_text() 
 jsonb_extract_path() 
 jsonb_extract_path_text() and json_extract_path_text() 
 jsonb_object() 
 jsonb_object_agg() 
 jsonb_object_keys() 
 jsonb_populate_record() 
 jsonb_populate_recordset() 
 jsonb_pretty() 
 jsonb_set() and jsonb_insert() 
 jsonb_strip_nulls() 
 jsonb_to_record() 
 jsonb_to_recordset() 
 jsonb_typeof() 
 row_to_json() 
 to_jsonb() 
 Money 
 Numeric 
 Range 
 Serial 
 UUID 
 XML 
 Keywords 
 Reserved names 
 Cursors 
 User-defined subprograms and anonymous blocks 
 «Commit» in user-defined subprograms 
 Subprogram attributes 
 "Depends on extension" semantics
 Alterable subprogram attributes 
 Alterable function-only attributes 
 Immutable function examples 
 "language sql" subprograms
 "language plpgsql" subprograms
 Create-time and execution model 
 "language plpgsql" syntax and semantics
 Declaration section 
 Executable section 
 Basic statements 
 "assert" statement
 "get diagnostics" statement
 "raise" statement
 "return" statement
 Cursor manipulation 
 Doing SQL from PL/pgSQL 
 Compound statements 
 The "if" statement 
 The "case" statement 
 The "loop", "exit", and "continue" statements 
 Infinite and while loops 
 Integer for loop 
 Array foreach loop 
 Query for loop 
 Jumping out of a block statement with "exit"
 Two case studies 
 Exception section 
 Case study: PL/pgSQL procedures-for role provisioning
 Subprogram overloading 
 Variadic and polymorphic subprograms 
 Name resolution in subprograms 
 The "pg_proc" catalog table 
 SQL compatibility 
 PG15 features 
 YCQL 
 ALTER KEYSPACE 
 ALTER ROLE 
 ALTER TABLE 
 CREATE INDEX 
 CREATE KEYSPACE 
 CREATE ROLE 
 CREATE TABLE 
 CREATE TYPE 
 DROP INDEX 
 DROP KEYSPACE 
 DROP ROLE 
 DROP TABLE 
 DROP TYPE 
 GRANT PERMISSION 
 GRANT ROLE 
 REVOKE PERMISSION 
 REVOKE ROLE 
 USE 
 INSERT 
 SELECT 
 EXPLAIN 
 UPDATE 
 DELETE 
 TRANSACTION 
 TRUNCATE 
 Simple expressions 
 Subscripted expressions 
 Function call 
 Operators 
 BLOB 
 BOOLEAN 
 Collection 
 FROZEN 
 INET 
 Integer and counter 
 Non-integer 
 TEXT 
 DATE, TIME, and TIMESTAMP 
 UUID and TIMEUUID 
 JSONB 
 Date and time 
 BATCH 
 ysqlsh 
 Meta-commands 
 pset options 
 Examples 
 ycqlsh 
 YugabyteDB Anywhere API 
 YugabyteDB Aeon API 
 Download 
 Join our community 
 Slack 
 Yugabyte University 
 GitHub 
 Yugabyte Friday Tech Talks 
 Forum 
 Contact Support 
 YugabyteDB 
 API 
 YSQL
 v2026.1 STS Stable release with standard-term support 
 v2026.1 STS Stable release with standard-term support 
 v2025.2 LTS Stable release with long-term support 
 v2025.1 STS Stable release with standard-term support 
 v2024.2 LTS Stable release with long-term support 
 Unsupported versions 
 YSQL API reference
 Copy page as Markdown 
 PostgreSQL-compatible API
 Introduction 
 Yugabyte Structured Query Language (YSQL) is an ANSI SQL, fully-relational API that is best fit for scale-out RDBMS applications that need ultra resilience, massive write scalability, and geographic data distribution. The YugabyteDB SQL processing layer is built by using the PostgreSQL code (version 15) directly. The result of this approach is that YSQL is fully compatible with PostgreSQL by construction .
 YSQL therefore supports all of the traditional relational modeling features, such as referential integrity (implemented using a foreign key constraint from a child table to a primary key to its parent table), joins, partial indexes, triggers, and stored procedures. It extends the familiar transactional notions into the YugabyteDB Distributed SQL Database architecture.
 If you don't find what you're looking for in the YSQL documentation, you might find answers in the relevant PostgreSQL documentation . Successive YugabyteDB releases honor PostgreSQL syntax and semantics, although some features (for example those that are specific to the PostgreSQL monolithic SQL database architecture) might not be supported for distributed SQL. The YSQL documentation specifies the supported syntax and extensions.
 To find the version of the PostgreSQL processing layer used in YugabyteDB, you can use the version() function. The following YSQL query displays only the first part of the returned value:
 select rpad( version (), 18 ) || '...' as v; 
 v
-----------------------
 PostgreSQL 15.2-YB...
 YSQL components 
 The main components of YSQL include:
 Data definition language (DDL)
 Data manipulation language (DML)
 Data control language (DCL)
 Built-in SQL functions
 PL/pgSQL procedural language for stored procedures
 These components depend on underlying features like the data type system (common for both SQL and PL/pgSQL), expressions, database objects with qualified names, and comments. Other components support purposes such as system control, transaction control, and performance tuning.
 The SQL language 
 The section The SQL language describes of all of the YugabyteDB SQL statements. Each statement has its own dedicated page. Each page starts with a formal specification of the syntax: both as a railroad diagram ; and as a grammar using the PostgreSQL convention. Then it explains the semantics and illustrates the explanation with code examples.
 Supporting language elements 
 This section lists the main elements that support the YugabyteDB SQL language subsystem.
 Built-in SQL functions .
 Data types . Most PostgreSQL-compatible data types are supported.
 Keywords .
 Names and Qualifiers. Some names are reserved for the system. List of reserved names .
 Quick Start 
 You can explore the basics of the YSQL API using the Quick Start .
 It always helps to have access to a sandbox YugabyteDB cluster where you can, when you need to, do whatever you want without considering any risk of doing harm. Here are the kinds of things you'll want to do:
 Connect as the postgres role and create and drop other superusers , and regular roles.
 Create and drop databases
 Create and drop extensions
 Create and drop objects of all other kinds
 With these freedoms, you'll be able to set up any regime that you need to help you illustrate, or test, a hypothesis about how things work.
 Moreover, for some experiments, you'll need operating system access so that you can make changes to various configuration files (like the one that determines the default values for session parameters).
 It also helps to have a vanilla PostgreSQL installation on the same server so that you can confirm for yourself that the SQL systems of each (at least for the functionality that application developers use, and in the overwhelming majority of cases) are syntactically and semantically identical.
 To do all this confidently, you need to be sure that nobody else can use your sandbox so that you know that everything that you observe will be explained by what you deliberately did. Occasionally, you'll even want to destroy a cluster at one version and replace it with a cluster at a different version.
 The simplest way to achieve this ideal sandbox regime is to use your own laptop. The Quick Start shows you how to do this.
 Contribute
 Report a doc issue
 Suggest new content
 Edit this page
 View as Markdown
 Contributor guide
 On this page 
 Introduction 
 YSQL components 
 The SQL language 
 Supporting language elements 
 Quick Start 
 © 2026 YugabyteDB, Inc. All Rights Reserved Privacy Policy | 
 Terms of Service
