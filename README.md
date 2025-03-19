<h1>Orchestrating Serverless Functions with Step Functions</h1>

<h2>Lab overview and objectives</h2>
In this lab, I will use AWS Step Functions to coordinate the actions necessary to generate and deliver a report upon request. The report will contain data from a database.
After completing this lab, you should be able to:
<ol>
<li>  Create an asynchronous state machine by using Step Functions</li>
<li>  Configure an Amazon Simple Notification Service (Amazon SNS) topic to deliver email alerts</li>
<li>  Configure AWS Lambda functions to be invoked from a Step Functions state machine</li>
<li>  Use a parallel state flow object in the design of a Step Functions state machine</li>
<li>  Invoke a state machine to start when a REST API endpoint is invoked </li>
<li>  Generate a presigned URL for an object stored in an Amazon Simple Storage Service (Amazon S3) bucket</li>
</ol>

<h2>Business Scenario</h2>
Thanks to Sofía, the coffee suppliers inventory now automatically updates on the café website. But the work is not finished! Frank asks if it would be possible to log in to the website to request a report with the latest inventory information.
Yesterday, Mateo, who is an AWS consultant and Sofía's friend, came into the café for a macchiato, his favorite espresso drink. While he was enjoying his beverage, Sofía told him about how she needs to build a reporting mechanism for Frank. After discussing the high-level business requirements, Mateo suggested that she use AWS Step Functions to coordinate the steps to generate the report. He described how Step Functions can help a developer to automate business processes by creating workflows, and providing parallelization and service integrations, among other features.
In this lab, Sofía will build the functionality to create and deliver the report. Then, in the next lab, she will improve the design further and implement authentication on the website to limit who can request and access reports.


The following diagram shows the architecture of the previous labs that I created in the previous labs. At the START of the lab, the infrastructure was recreated.

<img width="551" alt="image" src="https://github.com/user-attachments/assets/e517ca6f-2014-471a-abc2-c29d9fde0a53" />
