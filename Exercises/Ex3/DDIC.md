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

## Exercise 3.4 - Create a DB table
