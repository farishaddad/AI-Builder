# Lab 1 - Form Processing
In this lab we will build, train, and publish, a form processing AI model that will be able to extract key-value pairs and table data. We will then create a simple form processing application that will leverage this AI model and render the processed results.

<p align="center">
  <img src="../images/img-lab-fp-44.png" alt="Form Processing App" width="500px">
</p> 

## Prerequisites
1. Meet the standard set of prerequisites required for all labs as outlined in the main [README](../README.md).
2. Download the [Form Processing Sample Data](../../../raw/master/data/ai-builder-lab-formprocessing.zip).
3. Extract the contents of the zip file on your local machine.

## Table of Contents
   [Step 1 - Sign in to PowerApps](#step-1---sign-in-to-powerapps)  
   [Step 2 - Select an Environment](#step-2---select-an-environment)  
   [Step 3 - Build, Train, and Publish an AI Model](#step-3---build-train-and-publish-an-ai-model)  
   [Step 4 - Create a Canvas app](#step-4---create-a-canvas-app)  

## Step 1 - Sign in to PowerApps
1. Navigate to [https://powerapps.microsoft.com/](https://powerapps.microsoft.com/) and click **Sign in**  
[![alt text](../images/img-lab-fp-01.png "Alt")](../../../raw/master/images/img-lab-fp-01.png)  

2. Enter your Microsoft account (email address) and click **Next**  
[![alt text](../images/img-lab-fp-02.png "Alt")](../../../raw/master/images/img-lab-fp-02.png)  

3. Enter your password and click **Sign in**  
[![alt text](../images/img-lab-fp-03.png "Alt")](../../../raw/master/images/img-lab-fp-03.png)  

4. When prompted to "Stay signed in", click **Yes**  
[![alt text](../images/img-lab-fp-04.png "Alt")](../../../raw/master/images/img-lab-fp-04.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 2 - Select an Environment
Upon signing in, the default environment will be selected. Switch to an environment that has AI Builder enabled by opening the Environment drop-down menu at the top of the page. In this example, we would like to switch to the **Lab** environment.

Note: A prerequisite to this lab is that an environment is created in one of the supported AI Builder regions (United States or Europe).  
[![alt text](../images/img-lab-fp-05.png "Alt")](../../../raw/master/images/img-lab-fp-05.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 3 - Build, Train, and Publish an AI Model
1. On the left side panel, expand **AI Builder**, click **Build**, and click **Form Processing**  
[![alt text](../images/img-lab-fp-06.png "Alt")](../../../raw/master/images/img-lab-fp-06.png)  

2. Provide your model a **name** (e.g. Form Processing Model) and click **Create**  
[![alt text](../images/img-lab-fp-07.png "Alt")](../../../raw/master/images/img-lab-fp-07.png)  

3. Click **Add documents**  
[![alt text](../images/img-lab-fp-08.png "Alt")](../../../raw/master/images/img-lab-fp-08.png)  

4. Navigate to the extracted contents of the provided [sample data](../../../raw/master/data/ai-builder-lab-formprocessing.zip) and select the five forms under the **training** folder. Click **Open**.  
[![alt text](../images/img-lab-fp-09.png "Alt")](../../../raw/master/images/img-lab-fp-09.png)  

5. Click **Upload 5 documents**  
[![alt text](../images/img-lab-fp-10.png "Alt")](../../../raw/master/images/img-lab-fp-10.png)  

6. Click **Close**  
[![alt text](../images/img-lab-fp-11.png "Alt")](../../../raw/master/images/img-lab-fp-11.png)  

7. Click **Analyze**  
[![alt text](../images/img-lab-fp-12.png "Alt")](../../../raw/master/images/img-lab-fp-12.png)  

8. Wait until AI Builder has finished analyzing the documents, this may take several minutes.  
[![alt text](../images/img-lab-fp-13.png "Alt")](../../../raw/master/images/img-lab-fp-13.png)  

9. Click the tile to open the form fields selector.  
[![alt text](../images/img-lab-fp-14.png "Alt")](../../../raw/master/images/img-lab-fp-14.png)  

10. Select all the fields on the form.  
[![alt text](../images/img-lab-fp-15.png "Alt")](../../../raw/master/images/img-lab-fp-15.png)  

11. Change a subset of the selected fields to have friendly names by hovering over an item in the side panel on the right, click the pencil icon to enter edit mode, overwrite the text (e.g. AD to Address), then click the tick icon to confirm. Repeat this for Name, Address, Phone, Invoice Number, and Invoice Date. Then click **Done** in the top right hand corner.  
[![alt text](../images/img-lab-fp-16.png "Alt")](../../../raw/master/images/img-lab-fp-16.png)  

12. Click **Next**  
[![alt text](../images/img-lab-fp-17.png "Alt")](../../../raw/master/images/img-lab-fp-17.png)  

13. Click **Train**  
[![alt text](../images/img-lab-fp-18.png "Alt")](../../../raw/master/images/img-lab-fp-18.png)  

14. Click **Go to Details page**  
[![alt text](../images/img-lab-fp-19.png "Alt")](../../../raw/master/images/img-lab-fp-19.png)  

15. Click **Publish**  
[![alt text](../images/img-lab-fp-20.png "Alt")](../../../raw/master/images/img-lab-fp-20.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 4 - Create a Canvas app
1. Click **Create app**  
[![alt text](../images/img-lab-fp-21.png "Alt")](../../../raw/master/images/img-lab-fp-21.png)  

2. Click **Canvass app from blank**  
[![alt text](../images/img-lab-fp-22.png "Alt")](../../../raw/master/images/img-lab-fp-22.png)  

3. Provide the app a **name** (e.g. Form Processing App)  
[![alt text](../images/img-lab-fp-23.png "Alt")](../../../raw/master/images/img-lab-fp-23.png)  

4. If prompted with a "Welcome to PowerApps Studio" dialog box, check **Don't show me this again** and click **Skip**.  
[![alt text](../images/img-lab-fp-24.png "Alt")](../../../raw/master/images/img-lab-fp-24.png)  

5. Click **Insert** in the ribbon located on the top-left side of the page, expand **AI Builder (preview)** drop-down menu, click **Form processor**.  
[![alt text](../images/img-lab-fp-25.png "Alt")](../../../raw/master/images/img-lab-fp-25.png)  

6. Select your Form Processing Model.  
Note: If you are in a shared environment, there may be a number of models in this list built by different users. Use the search bar to locate your model.  
[![alt text](../images/img-lab-fp-26.png "Alt")](../../../raw/master/images/img-lab-fp-26.png)  

7. Drag the Form Processor component to the bottom left hand side and resize the object so that it stretches from top to bottom and about half of the width of the application.  
[![alt text](../images/img-lab-fp-27.png "Alt")](../../../raw/master/images/img-lab-fp-27.png)  

8. Click the **play** icon located on the top right hand side of the page.  
[![alt text](../images/img-lab-fp-28.png "Alt")](../../../raw/master/images/img-lab-fp-28.png)  

9. Click **Analyze**  
[![alt text](../images/img-lab-fp-29.png "Alt")](../../../raw/master/images/img-lab-fp-29.png)  

10. Navigate to the extracted contents of the provided [sample data](../../../raw/master/data/ai-builder-lab-formprocessing.zip) and select the test form under the **test** folder. Click **Open**.  
[![alt text](../images/img-lab-fp-30.png "Alt")](../../../raw/master/images/img-lab-fp-30.png)  

11. You should see all the field values have been identified. Click the **close** icon on the top-right corner of the page to return back to PowerApps Studio.  
[![alt text](../images/img-lab-fp-31.png "Alt")](../../../raw/master/images/img-lab-fp-31.png)  

12. If prompted with a "Did you know?" dialog box, check **Don't show me this again** and click **Ok**.  
[![alt text](../images/img-lab-fp-32.png "Alt")](../../../raw/master/images/img-lab-fp-32.png)  

13. Within the **Insert** ribbon, click **Label**. Drag the label to the right hand side of the Form Processor.  
[![alt text](../images/img-lab-fp-33.png "Alt")](../../../raw/master/images/img-lab-fp-33.png)  

14. Select the label by clicking on the object to bring it into focus, then update the **Text** property with the following formula: ``FormProcessor1.FormContent.Fields.Name``  
[![alt text](../images/img-lab-fp-34.png "Alt")](../../../raw/master/images/img-lab-fp-34.png)  

15. Change the formatting of the label by navigating to the **Home** ribbon, resizing the font to **24**, and making the item **Bold**.  
[![alt text](../images/img-lab-fp-35.png "Alt")](../../../raw/master/images/img-lab-fp-35.png)  

16. Navigate to the **Insert** ribbon and click **Data Table**.  
[![alt text](../images/img-lab-fp-36.png "Alt")](../../../raw/master/images/img-lab-fp-36.png)  

17. Close the Data panel.  
[![alt text](../images/img-lab-fp-37.png "Alt")](../../../raw/master/images/img-lab-fp-37.png)  

18. Drag the Data Table to the lower right hand corner of the app and resize accordingly.  
[![alt text](../images/img-lab-fp-38.png "Alt")](../../../raw/master/images/img-lab-fp-38.png)  

19. Select the Data Table by clicking on the object to bring it into focus, then update the **Items** property with the following formula: ``FormProcessor1.FormContent.Tables.table_0``  
[![alt text](../images/img-lab-fp-39.png "Alt")](../../../raw/master/images/img-lab-fp-39.png)  

20. Click **Choose the fields you want to add from the customization pane**  
[![alt text](../images/img-lab-fp-40.png "Alt")](../../../raw/master/images/img-lab-fp-40.png)  

21. Select the fields in this specific order: Item, Quantity, Unit Price, Amount. Click the **close** icon.  
[![alt text](../images/img-lab-fp-41.png "Alt")](../../../raw/master/images/img-lab-fp-41.png)  

22. While holding down the **Shift** key, click the following three columns in the Data Table: Quantity, Unit Price, and Amount. Release the **Shift** key. On the right panel, toggle **Can grow** to Off, change the **Width** to 100.  
[![alt text](../images/img-lab-fp-42.png "Alt")](../../../raw/master/images/img-lab-fp-42.png)  

23. Now that you understand the fundamentals of being able to map form field values to labels, repeat this process until your app looks like the below.  
[![alt text](../images/img-lab-fp-43.png "Alt")](../../../raw/master/images/img-lab-fp-43.png)  

24. Once complete, return to the preview mode by clicking the play button and analyzing another form from the training data set.  
[![alt text](../images/img-lab-fp-44.png "Alt")](../../../raw/master/images/img-lab-fp-44.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>
