# Lab 1 - Form Processing
In this lab we will build, train, and publish, a form processing AI model that will be able to extract key-value pairs and table data. We will then create a simple form processing application that will leverage this AI model and render the processed results.

## Prerequisites
1. Meet the standard set of prerequisites required for all labs as outlined in the main [README](../README.md)
2. Download the [Form Processing Sample Data](../data/ai-builder-lab-formprocessing.zip)
3. Extract the contents of the zip file on your local machine

## Step 1 - Sign in to PowerApps
1. Navigate to [https://powerapps.microsoft.com/](https://powerapps.microsoft.com/) and click **Sign in**  
![alt text](../images/img-lab-fp-01.png "Alt")  

2. Enter your Microsoft account (Email address) and click **Next**  
![alt text](../images/img-lab-fp-02.png "Alt")  

3. Enter your password and click **Sign in**  
![alt text](../images/img-lab-fp-03.png "Alt")  

4. When prompted to Stay sign in, click **Yes**  
![alt text](../images/img-lab-fp-04.png "Alt")  

## Step 2 - Select an Environment
Once signed in, the default environment will likely be selected. Switch to an environment that has AI Builder enabled by opening the Environment drop-down menu at the top of the page. In this example, we would like to switch to the **Lab** environment.

Note: A prerequisite to this lab is that an environment is created in one of the supported AI Builder regions (United States or Europe).  
![alt text](../images/img-lab-fp-05.png "Alt")  

## Step 3 - Build an AI Model
1. On the left side panel, expand **AI Builder**, click **Build**, and click **Form Processing**  
![alt text](../images/img-lab-fp-06.png "Alt")  

2. Provide your model a **name** (e.g. Form Processing Model) and click **Create**  
![alt text](../images/img-lab-fp-07.png "Alt")  

3. Click **Add documents**  
![alt text](../images/img-lab-fp-08.png "Alt")  

4. Navigate to the extracted contents of the provided [sample data](../data/ai-builder-lab-formprocessing.zip) and select the five forms under the **training** folder. Click **Open**.
![alt text](../images/img-lab-fp-09.png "Alt")  
![alt text](../images/img-lab-fp-10.png "Alt")  
![alt text](../images/img-lab-fp-11.png "Alt")  
![alt text](../images/img-lab-fp-12.png "Alt")  
![alt text](../images/img-lab-fp-13.png "Alt")  
![alt text](../images/img-lab-fp-14.png "Alt")  
![alt text](../images/img-lab-fp-15.png "Alt")  
![alt text](../images/img-lab-fp-16.png "Alt")  
![alt text](../images/img-lab-fp-17.png "Alt")  
![alt text](../images/img-lab-fp-18.png "Alt")  
![alt text](../images/img-lab-fp-19.png "Alt")  
![alt text](../images/img-lab-fp-20.png "Alt")  
![alt text](../images/img-lab-fp-21.png "Alt")  
![alt text](../images/img-lab-fp-22.png "Alt")  
![alt text](../images/img-lab-fp-23.png "Alt")  
![alt text](../images/img-lab-fp-24.png "Alt")  
![alt text](../images/img-lab-fp-25.png "Alt")  
![alt text](../images/img-lab-fp-26.png "Alt")  
![alt text](../images/img-lab-fp-27.png "Alt")  
![alt text](../images/img-lab-fp-28.png "Alt")  
![alt text](../images/img-lab-fp-29.png "Alt")  
![alt text](../images/img-lab-fp-30.png "Alt")  
![alt text](../images/img-lab-fp-31.png "Alt")  
![alt text](../images/img-lab-fp-32.png "Alt")  
![alt text](../images/img-lab-fp-33.png "Alt")  
![alt text](../images/img-lab-fp-34.png "Alt")  
![alt text](../images/img-lab-fp-35.png "Alt")  
![alt text](../images/img-lab-fp-36.png "Alt")  
![alt text](../images/img-lab-fp-37.png "Alt")  
![alt text](../images/img-lab-fp-38.png "Alt")  
![alt text](../images/img-lab-fp-39.png "Alt")  
![alt text](../images/img-lab-fp-40.png "Alt")  
![alt text](../images/img-lab-fp-41.png "Alt")  
![alt text](../images/img-lab-fp-42.png "Alt")  
![alt text](../images/img-lab-fp-43.png "Alt")  
![alt text](../images/img-lab-fp-44.png "Alt")  