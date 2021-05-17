---
layout: post
title: "Clean Data - Easy Additions and Sharability"
excerpt: "Automating COVID Data Management"
categories: tech
tags: [tech, google sheets]
comments: true
share: true
modified: 2021-05-16T00:00:00+05:30
author: Y Ramesh Rao
toc: true
toc_label: "Nifty Automation Hack"
image:
    path: https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/federico-respini-sYffw0LNr7s-unsplash.jpg
    caption: "Photo credit [Unsplash](https://unsplash.com/photos/sYffw0LNr7s)"
---
One thing that we desperately need when dealing with COVID-19 infection is constant monitoring of 3 vitals i.e.

* Blood Oxygen
* Pulse
* Temperature

Not only monitoring but this data is also needed to be shared by you with your close relatives and doctors.

Below simple steps would come in handy, and I hope it eases a few data gathering and sharing problems that you experience with infection.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/WhatDoesItDo.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/WhatDoesItDo.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

# Steps to achieve the below result

{% include responsive-embed url="https://www.youtube.com/embed/835guSxd0jo?controls=0&amp;" %}

## Step — 1 Google Sheets familiarity

First thing first, head over to [sheets.google.com](https://sheets.google.com); you can dive in right away by creating a new sheet there using the button like shown here.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-1-NewSheet.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-1-NewSheet.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Newly created sheet should like this.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-2-NewlyCreatedSheet.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-2-NewlyCreatedSheet.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Please head over the title section in your new sheet to change it to something more relevant to the task at hand.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-3-ChangingTheSheetTitle.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-3-ChangingTheSheetTitle.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}


The sheet is where we would see our data collected, but we would create a simple google form to ease our data entry part as well; for doing so, follow along like shown.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-4-FormCreationTools.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-4-FormCreationTools.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Once the form gets generated your existing sheet should get transformed into something that looks like this

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-5-PostFormIsCreated.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-5-PostFormIsCreated.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Now we can check out the form we created from a few additional options available to us now.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-6-EditingForm.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-6-EditingForm.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Your basic form should look somewhat similar to the below sample form.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-7-FormInterface.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step1-7-FormInterface.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

🚀 Great Start, almost with those steps outs; trust me, only a few more left to get ourselves in ease of bringing joy to data collection here.

## Step — 2 Google Forms familiarity

We need to do not much on the Google Forms interface but instead jump directly to Script Editor here.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-1-FormToScriptEditor.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-1-FormToScriptEditor.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Your Apps Script editor should have opened for you, and the interface should look like

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-2-AppScriptEditor.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-2-AppScriptEditor.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

Again please rename your script project to a more relevant name

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-3-ProjectNameChange.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-3-ProjectNameChange.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
Enter your project name in dialog opened.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-4-ProjectNameDialog.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-4-ProjectNameDialog.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
You should be able to see a renamed project like this.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-5-PostRenamedProject.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step2-5-PostRenamedProject.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
## Step — 3 Time For Some Code

We can add a few lines of code directly from the Gist below to your project and fix us up.

<script src="https://gist.github.com/yrameshra0/2db00feed90790301c57676ae17ac710.js"></script>

Copy the Gist above in Apps Script Project and hit save.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-1-GistScriptCopied.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-1-GistScriptCopied.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
On saving the script, the Apps Script Editor allows us to run and debug our code script.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-2-ScriptSavedOptionsAvail.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-2-ScriptSavedOptionsAvail.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
On running the script, you should see a dialog asking you to review permissions required for running our script and please complete the following to continue the script's run

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-3-ScriptRunningAndPermissions.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-3-ScriptRunningAndPermissions.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
The first thing would be Sign-In with Google screen asking you to select your google account.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-4-SignInWithGoogle.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-4-SignInWithGoogle.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
Next, it can show you a warning about the app hasn't been verified, and here you need to open the advanced options. 

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-5-AppSecAuthorization.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-5-AppSecAuthorization.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
Post Advanced Clicked it should allow you to proceed to the next step.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-6-AppSecAuthorizationFinal.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-6-AppSecAuthorizationFinal.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
At the last step, before we get redirected back to Apps Script Code Editor, we are allowed to check the permissions needed to run the script.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-7-FinalPermissionsReview.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-7-FinalPermissionsReview.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
Finally, after completing all the above authorizations and permissions review, you should see logs of your script execution. 🥳

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-8-FinalScriptExecution.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step3-8-FinalScriptExecution.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}
## Step — 4 Understanding Code Script

Before diving deeper into code, let's first see how exactly the current script is looking in the actual form rendered from it.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step4-0-FormRender.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step4-0-FormRender.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

**Q1.** How can you add/delete family members?

**Ans.** Using <code>allMembers</code>, that's the array that controls the drop-down items

**Q2.** How can you add/delete form input sections?

**Ans.** Items of the form <code>addTextItem()</code>, you can add or delete the existing ones based on you requirements

**Q3.** Checking out the form rendered?

**Ans.** On <code>Run</code>, a published URL is generated in the execution log; that's the URL we can use to see the final rendered form.

**Q4.** Post Form Submissions Trigger?

**Ans.** When the form is finally submitted <code>postFormSubmission()</code>, is called, and here we are sending email's to our relatives or doctors, or you can configure any other needful actions here.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step4-1-AllCodeExplained.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step4-1-AllCodeExplained.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

## Step — 5 Post Form Submission Actions

As we called out, we are interested in sending out notifications to our near and dear ones once we have submitted the form. That's the final configuration we are trying to set up here.

Firstly, you need to reach to triggers section of the Apps Script Editor Interface.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-1-TriggerSection.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-1-TriggerSection.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

You can start creating your trigger by using the *Add Trigger* Option

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-2-TriggerCreation.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-2-TriggerCreation.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

The dialog would list your code script functions to get your choice to use once the trigger event gets fired.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-3-ChoosingTriggerFunction.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-3-ChoosingTriggerFunction.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

After that, we need to select and tell that trigger function needs calling post form gets submitted.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-4-SavingTriggerFunction.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-4-SavingTriggerFunction.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

That's it, and you should have added a new trigger that's ready to do its job post you save and close.

<figure class="align-center">
  <a href="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-5-SavedTriggerListed.png" class="image-popup">
    <img src="https://s3.ap-south-1.amazonaws.com/bangalorebytes.in/cleandata/Step5-5-SavedTriggerListed.png" alt="">
  </a>  
  <figcaption></figcaption>
</figure>{: .notice}

## That's All To It

But if you have followed along, you pretty much should be able to use our setup, as shown at the start of the blog. 

_**Share and like in kind.**_
