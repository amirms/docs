---
title: "Setup Mendix UI Framework with just CSS"
category: "howto50"
space: "Mendix 5 How-to's"
---
# Setup Mendix UI Framework

<table><thead><tr><th class="confluenceTh">Mendix Version</th><th class="confluenceTh">Create Date</th><th colspan="1" class="confluenceTh">Modified Date</th></tr></thead><tbody><tr><td class="confluenceTd">5</td><td class="confluenceTd">Aug 20, 2015 16:41</td><td colspan="1" class="confluenceTd">Sep 02, 2015 11:26</td></tr></tbody></table>

In this how-to we will go through how to setup the [Mendix UI Framework](https://ux.mendix.com/) and do our first styling changes by just using CSS.

**After completing this how-to you will know:**

*   How to create a new App
*   How to create your own theme with just CSS
*   How to make your first styling changes

## 1. Preparation

Before you can start with this how-to, make sure you have completed the following prerequisites.

*   Download the latest [Mendix Business Modeler](https://appstore.mendix.com)
*   Download a text editor [Sublime Text](http://www.sublimetext.com/)

## 2\. Create a new App in the Mendix Business Modeler

In this chapter we will create a new app and select a theme from the New App selector.

1.  Open the **Mendix Business Modeler**.
2.  Create a **New App** from the **My Apps** screen in the Mendix Business Modeler.

     ![](attachments/14091841/14385528.png)
3.  Select a theme for your app.

    ![](attachments/14091841/14385527.png)
4.  You can now deploy your app (F5)

    ![](attachments/14091841/14385530.png) 

## 3\. Open your project in the text editor

1.  Open your **App Project Folder** in your text editor by choice.
2.  Navigate to the folder **theme** and you will find the css files in the folder **styles\css**.

    ![](attachments/14091841/14385529.png) 
3.  There are two subfolders in our **styles\css** folder. 
    1.  **Lib**, this folder contains our library file that contains all the default styling from the Mendix UI Framework. It's best practise to not alter this file
    2.  **Custom, **the custom file contains a preset of CSS elements and a copy of the library file but empty. Here we want to make our custom changes
4.  Let's open up the **custom.css** file. We always want to work from this file so we can always look back at the library.css file to see how the original theme used to be.  
5.  Let's change the color of our topbar. Find the CSS element .**region-topbar **as you can see in the screenshot below.

    ![](attachments/14091841/14385531.png) 
6.  Let's do a simple change by making the topbar red. Insert the following line as in the example below:

    background-color: #FF0000; 

    ![](attachments/14091841/14385532.png) 
7.  Let's redeploy our application and look at the result!

    ![](attachments/14091841/14385533.png) 
8.  Congratulations, you made your first theme change.

## 4\. Related content

*   [Scout and Windows 10 Workaround](/howto50/Scout+and+Windows+10+Workaround)
*   [Scout and Windows 10 Workaround](/howto6/Scout+and+Windows+10+Workaround)
*   [Filtering Data on an Overview Page](/howto50/Filtering+Data+on+an+Overview+Page)
*   [Layouts and Snippets](/howto50/Layouts+and+Snippets)
*   [Layouts and Snippets](/howto6/Layouts+and+Snippets)
*   [Filtering Data on an Overview Page](/howto6/Filtering+Data+on+an+Overview+Page)
*   [Setup Mendix UI Framework with just CSS](/howto50/Setup+Mendix+UI+Framework+with+just+CSS)
*   [Setting Up the Navigation Structure](/howto50/Setting+Up+the+Navigation+Structure)
*   [Creating your first two Overview and Detail pages](/howto50/Creating+your+first+two+Overview+and+Detail+pages)
*   [Setup Mendix UI Framework](/howto50/Setup+Mendix+UI+Framework)
