[README](../README.md) > [Lab 1 - Form Processing](./lab-form-processing.md)

# Lab 1 - Form Processing
In this lab we will build, train, and publish, a form processing AI model that will be able to extract key-value pairs and table data. We will then create a simple form processing application that will leverage this AI model and render the processed results.

<p align="center">
  <img src="../images/img-lab-fp-44.png" alt="Form Processing App" width="500px">
</p> 

## Prerequisites
Meet the standard set of prerequisites required for all labs as outlined in the main [README](../README.md).

## Table of Contents
   [Step 1 - Download the Sample Data](#step-1---download-the-sample-data)  
   [Step 2 - Sign in to PowerApps](#step-2---sign-in-to-powerapps)  
   [Step 3 - Select an Environment](#step-3---select-an-environment)  
   [Step 4 - Build, Train, and Publish an AI Model](#step-4---build-train-and-publish-an-ai-model)  
   [Step 5 - Create a Canvas app](#step-5---create-a-canvas-app)  
   [Step 6 - Save to the Cloud](#step-6---save-to-the-cloud)  

## Step 1 - Download the Sample Data
1. Download the sample data: [ai-builder-lab-formprocessing.zip](../../../raw/master/data/ai-builder-lab-formprocessing.zip).  
2. Once the download is complete, locate the zip file.  
Note: The downloaded file will appear at the bottom of your browser window, click the appropriate menu item to open the containing folder.  

    **Internet Explorer**  
    [![alt text](../images/img-lab-fp-46.png "Alt")](../../../raw/master/images/img-lab-fp-46.png)  

    **Google Chrome**  
    [![alt text](../images/img-lab-fp-47.png "Alt")](../../../raw/master/images/img-lab-fp-47.png)  

    **Microsoft Edge**  
    [![alt text](../images/img-lab-fp-45.png "Alt")](../../../raw/master/images/img-lab-fp-45.png)  

3. Right-click the zip file and click **Extract All...**  
    [![alt text](../images/img-lab-fp-48.png "Alt")](../../../raw/master/images/img-lab-fp-48.png)  

4. Click **Extract**  
    [![alt text](../images/img-lab-fp-49.png "Alt")](../../../raw/master/images/img-lab-fp-49.png)  

5. Navigate back to the Downloads folder by clicking **Downloads** in the navigation bar.  
    [![alt text](../images/img-lab-fp-51.png "Alt")](../../../raw/master/images/img-lab-fp-51.png)

6. Select the zip file **ai-builder-lab-formprocessing.zip** and click **Delete** as we only need the extracted contents to remain.  
    [![alt text](../images/img-lab-fp-50.png "Alt")](../../../raw/master/images/img-lab-fp-50.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 2 - Sign in to PowerApps
1. Open a new browser window. 

    **Tip #1**: If you have enough screen real estate, have these two windows side-by-side.
    * Window 1 - This page with the lab instructions
    * Window 2 - PowerApps
    
    Alternatively, you will need to switch between the two windows as you follow the instructions.

    **Tip #2**: If you are signing in using a new account, use Incognito or InPrivate mode to ensure a clean sign in process.  

    **Google Chrome**  
    [![alt text](../images/img-lab-fp-53.png "Alt")](../../../raw/master/images/img-lab-fp-53.png)  

    **Microsoft Edge**  
    [![alt text](../images/img-lab-fp-52.png "Alt")](../../../raw/master/images/img-lab-fp-52.png)  


2. Navigate to [https://powerapps.microsoft.com/](https://powerapps.microsoft.com/) and click **Sign in**  
[![alt text](../images/img-lab-fp-01.png "Alt")](../../../raw/master/images/img-lab-fp-01.png)  

3. Enter your Microsoft account (email address) and click **Next**  
[![alt text](../images/img-lab-fp-02.png "Alt")](../../../raw/master/images/img-lab-fp-02.png)  

4. Enter your password and click **Sign in**  
[![alt text](../images/img-lab-fp-03.png "Alt")](../../../raw/master/images/img-lab-fp-03.png)  

5. When prompted to "Stay signed in", click **Yes**  
[![alt text](../images/img-lab-fp-04.png "Alt")](../../../raw/master/images/img-lab-fp-04.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 3 - Select an Environment
Upon signing in, the default environment will be selected. Switch to an environment that has AI Builder enabled by opening the Environment drop-down menu at the top of the page. In this example, we would like to switch to the **Lab** environment.

Note: A prerequisite to this lab is that an environment is created in one of the supported AI Builder regions (United States or Europe).  
[![alt text](../images/img-lab-fp-05.png "Alt")](../../../raw/master/images/img-lab-fp-05.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 4 - Build, Train, and Publish an AI Model
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

10. Select all the fields on the form by clicking on them.  
[![alt text](../images/img-lab-fp-15.png "Alt")](../../../raw/master/images/img-lab-fp-15.png)  

11. Hover over the **TO** field and click the **Pencil** icon to enter edit mode.  
    [![alt text](../images/img-lab-fp-54.png "Alt")](../../../raw/master/images/img-lab-fp-54.png)

12. Rename the field to **Name** and click the **Tick** icon to confirm the change.    
    [![alt text](../images/img-lab-fp-55.png "Alt")](../../../raw/master/images/img-lab-fp-55.png)

13. Repeat this step until the following fields have all been renamed.
    * TO > Name
    * AD > Address
    * PH > Phone
    * INVOICE > Invoice Number
    * Date > Invoice Date

    Note: Ensure to check that all the changes have been confirmed by clicking the tick icon after renaming the field and that all the fields are selected with the purple tick on the left hand side of each field.

    [![alt text](../images/img-lab-fp-56.png "Alt")](../../../raw/master/images/img-lab-fp-56.png)

14. Click **Next**  
[![alt text](../images/img-lab-fp-17.png "Alt")](../../../raw/master/images/img-lab-fp-17.png)  

15. Click **Train**  
[![alt text](../images/img-lab-fp-18.png "Alt")](../../../raw/master/images/img-lab-fp-18.png)  

16. Wait until you see a dialog box that states "Training complete", then click **Go to Details page**  
[![alt text](../images/img-lab-fp-19.png "Alt")](../../../raw/master/images/img-lab-fp-19.png)  

17. Click **Publish**  
[![alt text](../images/img-lab-fp-20.png "Alt")](../../../raw/master/images/img-lab-fp-20.png)  

<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>

## Step 5 - Create a Canvas app
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

## Step 6 - Save to the Cloud
1. Click **File**  
[![alt text](../images/img-lab-fp-57.png "Alt")](../../../raw/master/images/img-lab-fp-57.png)  

2. Click **Save** > Click **The cloud** > Click  **Save**
[![alt text](../images/img-lab-fp-58.png "Alt")](../../../raw/master/images/img-lab-fp-58.png) 

3. By saving your app to the cloud, you can access it using PowerApps on iOS. Watch the video below to see how you can:
   * Download PowerApps from the App Store
   * Sign in using your Microsoft account
   * Open your published Form Processing app
   * Analyze a form directly from the iOS device

[![alt text](../images/img-lab-fp-59.png "Form Processing with PowerApps on the iPad")](https://vimeo.com/350481725) 


<div align="right"><a href="#lab-1---form-processing">↥ back to top</a></div>
