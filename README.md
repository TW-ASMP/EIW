# Entity Information Workbook

This repository holds the latest version of the Entity Information Workbook template (EIW).


> [!IMPORTANT]  
> This version of the EIW is being piloted exclusively at the HCTP. If you wish to use this version for a project at your facility, you must consult with the plant engineer(s) responsible for capital project delivery at that facility.

To download the file:
1. click on the file name to enter the file page
2. in the file page, find the download button (as seen in the picture below)

---

![Annotation 2024-03-01 103817](https://github.com/TW-ASMP/EIW/assets/116810412/255e107a-1aff-44d0-90a3-1a839ea0e252)

# Usage Instructions

---

This section contains instructions for particular steps in EIW usage that may not be immediately intuitive.  The other steps, perceived by TW to be straightforward are not included.  In other words, this is not a complete or comprehensive instruction set. 

## Consultant and Contractor: Enabling Excel Macro 

The EIW is a VBA macro-enabled spreadsheet; upon opening the EIW, you must enable the Excel macros.  You can find more instructions from Microsoft in the links below.

​	[Enable or disable macros in Microsoft 365 files - Microsoft Support](https://support.microsoft.com/en-us/office/enable-or-disable-macros-in-microsoft-365-files-12b036fd-d140-4e74-b45e-16fed1a7e5c6)

## Consultant: Documenting Asset Changes

Each row on the **Asset** worksheet represents one of the following asset changes.

* a new asset added by the project to perform a new role
* a new asset replacing an existing asset playing an existing role
* an original asset being removed but *not* replaced
* an original asset being moved (either to do something else or into storage)
* no asset changes

We start representing these changes from the  **Original Entity Number in WMS** column, shown below.

### Representing New Asset (and new role) Addition 

First, ensure that the asset you add is not replacing an existing asset (or multiple existing assets).  Then, in the **Change to Physical Asset** column, select "Added as new (to serve a new role)."

###  Representing Asset Replacement 

In the **Change to Physical Asset** column, select "Replaced".  Then, enter the correct value in the **Original Entity Number in WMS** column.

> In most cases, the original value you enter into the **Original Entity Number in WMS** column should be the same as the value you enter into the **Final Entity Number**. There are times, however, when it is valid for the consultant to enter different entity numbers in the two columns.  The difference would indicate to TW that the original entity number was revised to a new entity number in the course of the project. 
>
> Also, it is valid for the consultant to enter multiple entity numbers in the **Original Entity Number in the WMS** column;  this would indicate to TW that a new asset has replaced the function of multiple original assets.

### Representing Old Asset (and Role) Removal

In the **Change to Physical Asset** column, select "Replaced".  Then, all columns, except for **Original Entity Number**, should be left empty.

### Representing the Movement or Reassignment of Old Asset

In the **Change to Physical Asset** column, select "Moved".

If the asset is moved into storage, i.e., it will not play any role after the project, you only need to fill out the **Original Entity Number** and **Entity Location Description** columns.  Alternatively, if the asset is being moved to another role, fill out all columns on the sheet. 

### Representing an Asset not Changed by the Project

In every project, the consultant also needs to represent a class of assets that are not being changed by the project - these are assets on the branch of the asset hierarchy that fall within the scope of the consultant's project.  For example, if the consultant redesigns the HVAC equipment of Building-A, it is responsible for re-specifying Building-A's HVAC system asset hierarchy.  In its specification, the consultant must rebuild the complete hierarchy, including several original air handlers that the project will not change.  This is analogous to the consultant's responsibility to represent the same air handler in the revised drawings.  

## Consultant: Indicating Requirement for Further Asset Specification

TW collects additional technical specifications for approximately a dozen asset classes, including pump, motor, and valve.  While most of this information is entered by the contractor, the consultant must indicate, in each row, where additional specifications must be entered.  The following is an example of a consultant indicating, with the word "yes" under a class name, that further technical specifications on a pump and the motor are required.  

![image-20240415134238477](C:\Users\thuang4\AppData\Roaming\Typora\typora-user-images\image-20240415134238477.png)

At a later date, the consultant and the contractor would click on the "+" symbol (shown at the top of the example image) to expand and reveal the additional information entry columns.  The additional technical information for the pump class is shown in the example below.

![image-20240415134329504](C:\Users\thuang4\AppData\Roaming\Typora\typora-user-images\image-20240415134329504.png)

> In the previous iteration of the EIW, the contractor(s) would fill out all additional specifications.  In this version, the consultant is also responsible for a few columns of information.  In the example above, the consultant must specify the pump's orientation. 

## Contractor: Additional Technical Specification for Instrumentations

Unlike other asset classes, you won't be able to enter any additional technical specifications for instrumentations into the Asset worksheet.  You will need to enter them in the Asset-Instrumentation worksheet.  The reason is that many instrumentations can sense multiple parameters, such as temperature, pressure, or flow, and TW would like to know this full range of sensing functions. 

In the example below, the consultant indicated that THC-EX-FIT-0001 is a piece of instrumentation.  



![image-20240415133130362](C:\Users\thuang4\AppData\Roaming\Typora\typora-user-images\image-20240415133130362.png)

After examining the manual, the contractor for the project noticed that this instrument has flow and temperature-sensing functions.   As such, the contractor fills out two rows in the Asset-Instrumentation worksheet, both under the entity number THC-EX-FIT-0001. 



![image-20240415133041829](C:\Users\thuang4\AppData\Roaming\Typora\typora-user-images\image-20240415133041829.png)















