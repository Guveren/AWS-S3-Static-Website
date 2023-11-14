# AWS-S3-Static-Website

Here I got to create a static website and host it using AWS S3 buckets

create an S3 bucket 
- in creating this S3 bucket you need to uncheck the "All public object access" check box and consent to it by checking the acknowldgement box
- now under the buckets tab you can see the list of buckets you currently have
- Select your newly created bucket and then go under the properties tab
- scroll all the way down to static website hosting and edit
- Check the enable  check box for Static website hosting and for Host type, "Host a static website"
- for the Index document you can type in the name of your HTML file and save the changes.
Create the bucket policy
- Under permissions, we want to edit the bucket policy
- Click on the "Policy generator" so we can enable access in the s3 bucket.
    * The select type of policy should be "s3 bucket policy"
    * Principal " * "
    * Actions " GetObject "
    * ARN " [ARN/*] " the forward slash and * indicates allowing access to all
    * Add the statement and then generate the policy
- Copy out the generated policy and paste in the bucket policy text box
Upload your static website to your S3 Bucket
Navigate to the properties tab and click on the static website link to view your hosted website :)
