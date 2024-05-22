# Exercise 1 - Refactoring features

## Exercise 1.0 - Initialization

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


## Exercise 1.1 - Create class from scratch

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

## Exercise 1.2 - Create class from usage - Variable declaration

1. Declare new varaible of an unknown class

In the method if_oo_adt_classrun~main create a new variable lv_o_dependency_class type ref to zcl_exo1_d_class_#### (#### corresponding to the unique id of your package)

```
data lv_o_dependency_class type ref to zcl_exo1_d_class_####.

```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9072965c-a160-4873-a1f2-f1c380754131)


2. Use Quick Fix to create the class (Global)

Right click on the error in the code and click on Quick Fix or use the shortcut Ctrl + 1 to lauch the Quick Fix

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/d16e938b-2ae9-448d-b271-7da26929b7c0)

In the Quick fix proposal choose "create global class ZCL_EXO1_D_CLASS_####" (you can choose Local if you don't want to create a global class but a local one which should be visible only for the main class)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9ad19758-eaf3-46a6-aa58-7f945951f012)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/6bd43e02-9f24-423f-9d7b-7bd3731c69d9)

3. Fill Class Characteristics

Fill the description of the newly created class : "Exo 1 First dependent class"

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/7f06624f-e0df-4af8-bc83-0e69b9523c0d)

Click on Next>

Choose the same TR used previously.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/bf0508f8-13df-492b-b22e-b61f60811b2a)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/3ddbc060-127b-4385-a723-eb1bdcf4903d)

Activate all your classes
 
## Exercise 1.3 - Create class from usage - class-methods calling

We will create a class with a factory method from the usage in the call method.

1. Delete the class previously created

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/485cb447-9177-4bb2-b6f1-7c4a88050e92)

2. Delete the variable previously created in method if_oo_adt_classrun~main

```
data lv_o_dependency_class type ref to zcl_exo1_d_class_####.

```
With plugin ABAP Cleaner you can go to :
Right click on your code Source code->Clean Up With Interactive ABAP Cleaner...

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/85643821-5457-48b3-84ed-514fc23e9ddb)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9200668a-1dbc-47ca-b864-8a7be7bb5bef)


3. Add a call of a factory method of an unknown class

```
data(lv_o_delegate) = zcl_exo1_d_####=>create_with_ref_console( i_out = out ).

```
(#### corresponding to the unique id of your package)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/50309c65-6d33-4d07-8704-1d5c1ff90ca2)

4. Use Qucik fix to generate the class and the method definition

Click on the class name and use the shortcut Ctrl + 1 to launch the Quick Fix and create a global class

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/fef0c4d8-2d1a-4760-9803-33054d814dc7)

Fill the description: delegate class

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/16a05554-3987-418f-b35d-3b916fdb901a)

Click on Next>

Use the same TR and click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/47e76f39-848e-427f-b634-96f3eca602de)

5. Create the method definition with quick fix.
Go back to the edit page of the class ZCL_ADT_EXO1_####
Click on the method name create_with_ref_console and use the shortcut Ctrl + 1 to launch the Quick Fix

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9e8fa71e-5d62-4077-ad97-d4e3712aad30)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9ecf7197-c5af-4c9f-8248-cb768af0089f)

Change the type of the parameter r_result from any to type ref to zcl_exo1_d_####

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/0baa9cd7-1048-49eb-b8ae-dd445f978a2a)

Click on finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/45cd5992-a54f-443a-95a7-f768f2275ba2)


## Exercise 1.4 - Create a factory method

1. Remove definition and implementation of class method create_with_ref_console
In class zcl_exo1_d_#### remove the definition and the implementation of the method create_with_ref_console

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/eb845b85-61d3-492f-b4df-591d11e72c7d)

2. Add private attribute gv_out 

Add the private attribute gv_out type ref to IF_OO_ADT_CLASSRUN_OUT

```
data gv_out type ref to if_oo_adt_classrun_out.

```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9936238b-380a-4f0f-adfb-65a1f09dac27)


3. Change the visibility for the creation process from PUBLIC to PRIVATE
From

```
CLASS zcl_exo1_d_0001 DEFINITION
  PUBLIC
  FINAL
  CREATE PUBLIC .
```

To

```
CLASS zcl_exo1_d_0001 DEFINITION
  PUBLIC
  FINAL
  CREATE PRIVATE .
```

With this change the creation of a new instance of this class is only possible inside this class

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/e3283a56-0f5d-440c-adbc-60d2c4a634b3)


4. Generate Factory method (Static method which generate a new instance of the class)

Put your cursor on the name of the class and open the Quick Fix (Shortcut Ctrl + 1 or Right Click => Quick Fix)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/247b4288-4091-4a82-baf5-2f7078d62fca)

Choose "generate factory method create"

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/65b11e6a-1e3d-4e9f-ac9b-42b1f1bd4244)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/5ddabd69-95b2-45f7-8d06-79c858251149)


5. rename the create method to create_with_ref_console

Click on the method name (implementation or definition) and use the Quick Fix or even the shortcut Ctrl + 2 + r to rename the method.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/2ae5d484-46eb-4838-8c7e-a1f0aae04552)

6. Activate all your class

## Exercise 1.5 - Create method from usage

Go to the class zcl_adt_exo1_####

1. add the code below after the call of the factory method

```
lv_o_delegate->process( ).
```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/80ec70d6-7afa-4822-b6ef-e36e0b2aded0)


2. Use Quick fix (Ctrl + 1) to generate the definition of the new method and its empty implementation in class zcl_exo1_d_0001

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/261cdb09-e372-4d7f-a84d-fa98444ba2d5)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9542217b-bae2-47de-841b-cae2daf8794e)

Click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/58e389e8-21f4-4999-b30b-e1dd31a9256d)


3. Implement the new method process

Cut/Paste the code below from the method if_oo_adt_classrun~main of the class zcl_adt_exo1_#### to the method process of the class zcl_exo1_d_####

```
 out->write( data = |Hello World| ).
```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/913953fd-12ef-42c2-8c37-f6a980499d72)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/e204f0c9-e5c5-485f-8936-904f13ba8d9c)


4. Rename the variable out to gv_out to correspond to the private attribut.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/899df3bd-c58a-4f99-be7d-5afe0ef881bd)


5. Activate all your classes
6. Execute the class zcl_adt_exo1_#### as an ABAP Application (Console)

You should have the same result than the one got in Exercice 1.1.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/2e434d05-b5bf-4f6c-8cb8-697f5aa8a230)


## Exercise 1.6 - Create method from expression

Go to class zcl_exo1_d_####

1. Add a condition statement before to call the method write of the attribue gv_out in method process

```
if gv_out is bound.
  gv_out->write( data = |Hello World| ).
endif.
```

2. Select the condition 'gv_out is bound' and use quick fix to generate new method

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/980b5a50-49c8-4750-bc18-478ecbbecdd4)

Name the new method "is_console_initialized"

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/f97ed047-a9ac-4869-b447-545592fbb5b9)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/fd8ea957-d557-41cc-95cd-49c68f124ec7)

3. Activate the class

## Exercise 1.6 - Create method from statements

Go to class zcl_exo1_d_####

1. select all the statements in the method process and use Quick fix to generate a new private method internal_processing

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/b23e75fe-443c-4537-ba93-89e6c8e972be)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/2d317c72-7206-45b7-aae7-fdb5ad20f3dd)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/80250d90-609d-4026-9075-3ee2809734f4)

2. Activate your class


## Exercise 1.7 - Create interface from usage

Go to class zcl_exo1_d_#### 

1. Create an ABAP Interface from the usage in class zcl_exo1_d_####

In Public section add the code below to declare the new interface zif_exo1_delegate_#### where #### corresponds to your unique id

```
INTERFACES ZIF_EXO1_DELEGATE_####.
```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/b3afbf77-f87a-44b2-92f7-ba74c91f09ec)


2. Use Quick fix (Ctrl + 1) to create the global interface

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/5bb08d41-e6d4-4d3b-b869-fd5f69b5a932)

Fill the description: delegation processing

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/8cf5c3ec-a80e-40f4-9308-9ed6e6eeda1b)

Click on Next>

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/063240d5-40a7-434f-bc31-689cdf55ec16)

Select your TR and click on Finish

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/2e3ebf1f-c36c-414e-b912-fd52f0a407b2)


3. Activate the newly interface.

## Exercise 1.8 - Pull Up method to Interface

Go to class zcl_exo1_d_#### 

1. Change the definition of the method create_with_ref_console to return an interface type instance in place of the class instance type 

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/fda8ffca-d342-4156-9761-9db765747e01)

Some error appeared in the implementation of the method create_with_ref_console

2. Change the implementation of the method create_with_ref_console

Insert the below code in place of the actual implementation

```
    DATA(lv_instance) = NEW zcl_exo1_d_0001( ).
    lv_instance->gv_out = i_out.
    r_result = lv_instance.
```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/42f84e57-d0cf-4f59-830c-5b8837586244)

3. Pull-Up the method process to the interface ZIF_EXO1_DELEGATE_####

Click on the method name process in the declaration and use the Quick fix to pull up the method in the interface.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/f66e9b4d-0c80-4003-bb23-484d57cf03ed)

 Change in class zcl_exo1_d_0001 declaration
 
 ![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/7daf2a80-3353-4383-8242-30c83a08f68f)

Change in interface definition.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/b157cbae-30ec-44a9-83ab-e638a0945c50)

Save and activate the interface and the class.

4. Execute the class zcl_adt_exo1_#### as an ABAP Application (Console)

You should have the same result than the one got in Exercice 1.1.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/2e434d05-b5bf-4f6c-8cb8-697f5aa8a230)

## Exercise 1.9 - Create a constructor

Go to Class zcl_exo1_d_#### 

1. Generate Constructor using Quick Fix (Ctrl + 1)

Put your cursor on the class name and open the Quick fix (Ctrl + 1).

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/237dc64f-01eb-4aff-a242-7ae3f05c3231)

Based on the attribute in your class in the popup you choose the attributes which would be part of the construtor implementation.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/e51487ef-8e73-47d4-976c-8829d8aa433d)

Click on finish.

Constructor method definition generated

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/50c9e90c-3087-44ed-9b53-4a41701cf535)

Constructor method implementation generated

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/613753cc-f431-4265-8b53-930a0e1be750)


An error occured in method create_with_ref_console due to the constructor expects an importing parameter.

2. Change the implementation of the factory method create_with_ref_console

Replace the actual code by the code below

```
    DATA(lv_instance) = NEW zcl_exo1_d_0001( i_out ).
    r_result = lv_instance.
```

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/99e67f51-072b-46e8-b9d9-041e88820d77)


3. Activate your class

## Exercise 1.10 - Generate constants from literal

Go to class zcl_exo1_d_#### 

1. Add a literal in the method internal_processing

Replace the implementation of the method internal_processing by the code below:

```
IF is_console_initialized( ) = abap_true.
      gv_out->write( data = |Hello World| ).
      DO 3 TIMES.
        gv_out->write(  data = |iteration: { sy-index }| ).
      ENDDO.
    ENDIF.
```

2. Activate your class
3. Execute the Class zcl_adt_exo1_#### and check the result in Console

Execute the class zcl_adt_exo1_#### as an ABAP Application(Console)

You should have the result below:

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/8a53dfd0-33ab-4a3b-812e-e4ea0059025c)


4. Back to the class zcl_exo1_d_#### and use Quick fix to transform literal in local constants

In method internal_processing implementation select the number 3 in the statement "DO 3 TIMES" and use the quick fix (Ctrl + 1) to transform this literal in a local constants "c_nb_iteration

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/d4ce3bec-958d-425a-bec7-bb26c5eb064d)

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/278dc03b-554b-46d1-9363-7bb937460214)

5. Activate your class
6. Execute the Class zcl_adt_exo1_#### and check the result in Console

Execute the class zcl_adt_exo1_#### as an ABAP Application(Console)

You should have the result below:

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/8a53dfd0-33ab-4a3b-812e-e4ea0059025c)

## Exercise 1.11 - Converting local to class member

Go to class zcl_exo1_d_#### 

1. In method internal_processing implementaton put your cursor on the constant c_nb_iteration and use Quick fix to change from local to class member

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/4e0cfdf9-a650-4638-8703-141c2ebc2989)


2. Change in the class

In method internal_processing implementaton

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/c26b38d6-7f32-4bcb-8af6-1afb3200fdce)

In class Definition

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/9c97c9c1-cfda-400a-99f4-ba14c266747f)

3. Activate your class.

## Exercise 1.12 - Change visibility

Go to class zcl_exo1_d_#### 

1. change the visibility of the method internal_processing from private to protected.

Put your cursor on the name of the method internal_processing and use the Quick Fix (ctrl + 1) to move the method declaration from the private section to the protected section.

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/a2a3d096-708b-4af4-ba19-3527a33e9d10)

Change in the Class Definition

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/1680cb43-1881-4f6b-9b50-b286ba871131)

2. Activate your class.
3. Execute the Class zcl_adt_exo1_#### and check the result in Console

Execute the class zcl_adt_exo1_#### as an ABAP Application(Console)

You should have the result below:

![image](https://github.com/davidmacn/ADT-Usage-Exercises/assets/118279247/8a53dfd0-33ab-4a3b-812e-e4ea0059025c)

