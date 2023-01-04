# automation-scto-zapier

## Overview

- triggering event: Submission of a form in SurveyCTO.
- resulting action: A Zap in Zapier.

## Components

- this GitHub repository

## Replicating the system

1. Set up cloud publishing in SurveyCTO.
   1. Log into SurveyCTO.
   2. Click on "4. Export".
   3. Ensure that "Advanced: publishing form and dataset data to the cloud" is set to ON.
   4. For the desired form, click on Configure.
   5. Click "+ Add Zapier connection".
   6. Name the connection based on the form id and/or subset of fields.
   7. Select which fields to publish.
   8. Select whether to include hyperlink to submission details, whether to include text summary, and whether to publish existing data.
   9. Click "Save and continue".
   10. In the window that pops up, click "Copy to clipboard".

2. Create a new Zap in Zapier.
   1. In a new tab, log into Zapier.
   2. Click on "+ Create Zap".
   3. In the search box for App event, enter "SurveyCTO" and then click on SurveyCTO.
   4. Select the Event "New Form Submission" and click Continue.
   5. Select the SurveyCTO account corresponding to the relevant SurveyCTO form.
      1. If necessary, click "Connect a new account", paste the API key you just copied, then click "Yes, Continue".
   6. Click Continue.
   7. Select the Connection Name corresponding to the Zapier connection you created, then click Continue.
   8. Click "Test trigger", which should result in a green checkbox and a message that "We found a submission!".

## Modifying a replicated system

- To change what information is sent to the Zap, edit the connection in SurveyCTO.
- To complete the Zap, set up one or more actions and then publish the Zap.

## External documentation

- https://docs.surveycto.com/05-exporting-and-publishing-data/03-publishing-data-to-the-cloud/04.forms-to-zapier.html
