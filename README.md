# dm-interviews-26jun23

## ----- (~ 1hr 30 mins) ----- 
1. A working API application (JAVA/SpringBoot, NodeJS or any other) that can do basic CRUD
2. Additionally the CRUD shall have capability of single & mass updates (i.e. single create/ mass create, single read/ mass read, single update/ mass update, single delete/ mass delete)
3. Connect to a local SQLite DB (strictly SQLite only)
4. DB model (to be generated via versioned migration scripts) - you may use Flyway or Liquibase:

### --- Production Order Master ---
OrderID: ID (PK) <br>
Order Description: CHAR255 <br>
ProductID: String <br>
Product Description: CHAR255 <br>

5. Push in the following data via migration scripts:
PRD001;'Order for computer table/type01';CT01;'Computer table type 01 <br>
PRD002;'Order for computer table/type02';CT02;'Computer table type 02 <br>
PRD003;'Order for computer table/type03';CT03;'Computer table type 03 <br>
PRD004;'Order for computer table/type04';CT04;'Computer table type 04 <br>
PRD005;'Order for computer table/type05';CT05;'Computer table type 05 <br>
PRD006;'Order for computer table/type06';CT06;'Computer table type 06 <br>
PRD007;'Order for computer table/type07';CT07;'Computer table type 07 <br>
PRD008;'Order for computer table/type08';CT08;'Computer table type 08 <br>
PRD009;'Order for computer table/type09';CT09;'Computer table type 09 <br>
PRD010;'Order for computer table/type10';CT10;'Computer table type 10 <br>

6. Introduce a new column 'Plant' as additional not-null PK via versioned migration scripts

### --- Production Order Master ---
OrderID: ID (PK) <br>
Plant: String (PK) <br>
Order Description: CHAR255 <br>
ProductID: String <br>
Product Description: CHAR255 <br>

7. Take care of the Data migration. New data to look like this.
PRD001;PLNT01;'Order for computer table/type01';CT01;'Computer table type 01 <br>
PRD002;PLNT01;'Order for computer table/type02';CT02;'Computer table type 02 <br>
PRD003;PLNT01;'Order for computer table/type03';CT03;'Computer table type 03 <br>
PRD004;PLNT01;'Order for computer table/type04';CT04;'Computer table type 04 <br>
PRD005;PLNT01;'Order for computer table/type05';CT05;'Computer table type 05 <br>
PRD006;PLNT01;'Order for computer table/type06';CT06;'Computer table type 06 <br>
PRD007;PLNT01;'Order for computer table/type07';CT07;'Computer table type 07 <br>
PRD008;PLNT01;'Order for computer table/type08';CT08;'Computer table type 08 <br>
PRD009;PLNT01;'Order for computer table/type09';CT09;'Computer table type 09 <br>
PRD010;PLNT01;'Order for computer table/type10';CT10;'Computer table type 10 <br>
PRD001;PLNT02;'Order for computer table/type01';CT01;'Computer table type 01 <br>
PRD002;PLNT02;'Order for computer table/type02';CT02;'Computer table type 02 <br>
PRD003;PLNT02;'Order for computer table/type03';CT03;'Computer table type 03 <br>
PRD004;PLNT02;'Order for computer table/type04';CT04;'Computer table type 04 <br>
PRD005;PLNT02;'Order for computer table/type05';CT05;'Computer table type 05 <br>
PRD006;PLNT02;'Order for computer table/type06';CT06;'Computer table type 06 <br>
PRD007;PLNT02;'Order for computer table/type07';CT07;'Computer table type 07 <br>
PRD008;PLNT02;'Order for computer table/type08';CT08;'Computer table type 08 <br>
PRD009;PLNT02;'Order for computer table/type09';CT09;'Computer table type 09 <br>
PRD010;PLNT02;'Order for computer table/type10';CT10;'Computer table type 10 <br>

8. Create Postman collection for the CRUD/ mass-update
9. Code must have proper structure
10. Create your branch and upload code (along with postman scripts) to the public repo -> https://github.com/sandsri/dm-interviews-26jun23 to a folder with your full name in camel case
11. After this, we should be able to download, build and run this locally. Please maintain instructions of the same in a README.md file
