# Exercise 3 - DDIC Objects

## Exercise 3.0 - Initialization

Create package ZADT_USAGE_EX3-#### (replace #### by an alphanumeric characters to have a unique ID of package)

1. Right Click on the project

New->ABAP Package

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/89529391-12b0-4298-a827-1e38a72e953d)

2. Fill the data like in the screenshot below with the informations:
- Name: ZADT_USAGE_EX3-#### (replace #### by an alphanumeric characters to have a unique ID of package)
- Description: EXO 3 ADT DDIC exercise
- Add to favorite packages: ticked
- Package Type: Development

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/25d6b03e-2c50-4197-9bba-6a160bc73a5a)

Click on Next>

3. Fill the data like in the screenshot below with the informations:
- Software Component: ZLOCAL

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/3e4f3efd-6d8b-4afa-878d-d0ad5ac1486a)

Click on Next>

4. Create a new TR like in the screenshot below with the informations:
- Request Description: EXO 3 ADT DDIC exercise

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/4904af0f-f39c-48b7-bd2a-25fffe8e6f4d)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/f3435cce-e340-475c-a8db-0457612985d5)

## Exercise 3.1 - Create Domain

Steps to create a domain

1.Right click on the Package ZADT_USAGE_EX3-#### 

New->Other ABAP Repository Object

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/708b81dd-3ba3-4a1e-8f8f-decbb75a3056)

Filter on Domain

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9fc26b2e-fa02-4353-b1f3-ec4778129bf0)

Click on Next> after select the object Domain

2.Fill basic information for the new domain

Fill the popup with the informations below:

- Name: ZADT_3_DOMAIN#### (replace #### by the unique ID of package)
- Description: ADT Domain Demonstration

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/f5c30e26-8477-422f-87b7-09942ecf96fd)

Click on Next>

3. Choose the TR

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/780978af-8dc0-4fff-98b6-427d22283288)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/3c826956-db29-4c7e-9977-efdd2ce4eb35)

4. Fill the technical definition of the new domain

Mandatory
Data Type (Use Ctrl + Space to display all the predefined type usable): Example use the Char Data Type
>Depending of the "Data Type" choosed, you wil have others mandatory field to fill.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/a0039460-b9a9-431e-8620-b2e9d660b500)

5. Save and activate the new Domain

## Exercise 3.2 - Create data element

Steps to create a data element

1.Right click on the Package ZADT_USAGE_EX3-#### 

New->Other ABAP Repository Object

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/708b81dd-3ba3-4a1e-8f8f-decbb75a3056)

Filter on Data Element

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9b64251c-2929-460a-931e-cb73f244fe81)

Click on Next> after select the object Data Element

2.Fill basic information for the new Data Element

Fill the popup with the informations below:

- Name: ZADT_3_ELT#### (replace #### by the unique ID of package)
- Description: ADT Data Element Demonstration

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/23735555-0ac1-45cb-a225-c63534cb3fb0)

Click on Next>

3. Choose the TR

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/a36b606f-4677-4494-bbc4-cd6e608c10ed)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/c6c3c887-021a-4f25-9b0c-812943b79d22)

4. Fill the technical definition of the new data element

A new data element can be based on predefined type or a domain or reference, in the scope of this we will base the new data element on the predefined type category.

Data Type Information:
Data Type: CHAR
Length: 1

Field Labels:
Short: Demo
Medium: Data Elt Demo
Long: Data Element Demo
Heading:Data Element Demonstration

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/3fd9f53c-3869-4794-9df6-e8cf94a5698c)

5. Save and activate the new Data Element

## Exercise 3.3 - Create a structure

Steps to create a structure

1.Right click on the Package ZADT_USAGE_EX3-#### 

New->Other ABAP Repository Object

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/708b81dd-3ba3-4a1e-8f8f-decbb75a3056)

Filter on Structure

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/dd85f88c-3466-41dc-a449-4abe4be0eb9f)

Click on Next> after select the object Structure

2.Fill basic information for the new Structure

Fill the popup with the informations below:

- Name: ZADT_3_STR#### (replace #### by the unique ID of package)
- Description: ADT Structure Demonstration

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/1b833e61-dd90-4341-9337-89a4a642b1a6)

Click on Next>

3. Choose the TR

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/ed2254cc-ba33-4c55-94de-3d0fa1b7c034)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/ad7e47ad-2263-4c51-b08b-e0cec9d74a2c)

4. Define the fields which define the structure

>Use the Ctrl + Space to add some anotation
>For field based on predefined type use "abap.", use Ctrl + Space

>For field based on data element start the name of the data element and use Ctrl + Space to view all the available data element

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/6a50b9c5-69f7-461b-8a05-e2aa82e9dead)

>You can change the enhancement category through the annotation @AbapCatalog.enhancement.category and use the Ctrl + Space to choose between the available options

5. Save and activate the new Structure

## Exercise 3.4 - Create a DB table

Steps to create a DB Table

1.Right click on the Package ZADT_USAGE_EX3-#### 

New->Other ABAP Repository Object

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/708b81dd-3ba3-4a1e-8f8f-decbb75a3056)

Filter on Table

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/1b3c399d-19cd-474d-a838-1e539591ce73)


Click on Next> after select the object Database Table

2.Fill basic information for the new Database Table

Fill the popup with the informations below:

- Name: ZADT_3_DB#### (replace #### by the unique ID of package)
- Description: ADT DB Table Demonstration

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9da0e8fe-364f-48c3-810d-98a346ba53fd)

Click on Next>

3. Choose the TR

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/3f157a37-fd22-4888-9160-7469132b5e95)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/563310b4-2c81-4f6b-b0f0-a3dfe05a686c)


4. Define the fields which define the db table

>Use the Ctrl + Space to add some anotation
>For field based on predefined type use "abap.", use Ctrl + Space

>For field based on data element start the name of the data element and use Ctrl + Space to view all the available data element

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/6675adce-3a7c-47b6-a7f3-35fd39a05290)

>You can change the enhancement category through the annotation @AbapCatalog.enhancement.category and use the Ctrl + Space to choose between the available options

>use the keywords include to append an include in the db table definition

5. Save and activate the new DB Table
  
6. Update technical settings

Right Click in the DB Table editor view and choose Open Ohters->Technical Settings

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/1d5914d4-4049-446c-9a6b-0e52b88fc1d6)

Update the technical settings (you can use Ctrl + Space on some field to help you to fill them).

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/3fabd400-5d40-4f3a-b756-93c7368fbd07)

Save and activate
