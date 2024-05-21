# Exercice 1 - Refarctoring features

## Exercice 1.0 - Initiliazation

Create package ZADT_USAGE_EX1-#### (replace #### by an alphanumeric characters to have a unique ID of package)

1. Right Click on the project

New->ABAP Package

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/89529391-12b0-4298-a827-1e38a72e953d)

2. Fill the data like in the screenshot below with the informations:
- Name: ZADT_USAGE_EX1-#### (replace #### by an alphanumeric characters to have a unique ID of package)
- Description: EXO 1 ADT usage exercise
- Add to favorite packages: ticked
- Package Type: Development

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/4499234d-d1f1-4b33-b4c4-20e118b575ba)

Click on Next>

3. Fill the data like in the screenshot below with the informations:
- Software Component: ZLOCAL

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/4e50f2e0-dcc8-46d1-b610-8fde2a61d0c5)

Click on Next>

4. Create a new TR like in the screenshot below with the informations:
- Request Description: EXO 1 ADT usage exercise

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/80ee7cdc-d3e4-447e-ae23-0fa2442d67a2)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/2660ab72-54c3-48f4-be1d-96830421f325)


## Exercice 1.1 - Create class from scratch

In the package ZADT_USAGE_EX1-#### create a class ZCL_ADT_EXO1_#### (Use same id than the one used for the package)

1. Right click on the package ZADT_USAGE_EX1-####

New->ABAP Class

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/50611f7f-3d81-4204-9e4e-d4307fdcc373)

2. Fill the screen like in the screenshot below with the informations:
- Name: ZCL_ADT_EXO1_#### (Use same id than the one used for the package)
- Description: Exo1 Class
- Interfaces: IF_OO_ADT_CLASSRUN (Interface used to execute application in console)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/83704d9e-eb4b-42a0-bade-bd66d55dc526)

Click on Next>

3. Use the same TR than the one used for the Package

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/c051bfb3-4c92-4639-954c-3db444cb23c3)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/c40ce6af-a421-42a5-bbe4-13046c633164)

4. Implement an "Hello World" text to be display in the console

Fill the implementation of the method if_oo_adt_classrun~main

```
out->write( data = |Hello World| ).
```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/8888e3ae-b9bc-421d-85d3-150c129a4f54)

Activate your class (Shortcut Ctrl+F3)

5. Execute you class as a console application Shortcut F9 or right click on your code Run As->1 ABAP Application(Console)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/bf592159-bbec-4327-b5d2-c912098d37fc)

6. Result in Console

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/ce31f874-2a11-4376-bb5d-5b3abf14f4c3)

## Exercice 1.2 - Create class from usage

## Exercice 1.3 - Create method from usage

## Exercice 1.4 - Create method from expression

## Exercice 1.5 - Create method from statements

## Exercice 1.6 - Create interface from usage

## Exercice 1.7 - Pull Up method to Interface



