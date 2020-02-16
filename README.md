# mp_web_to_email_form
Web to Email Form Plugin for MP's Website to Help Case Workers by Tagging Emails

## Useful Websites
 * https://docs.google.com/document/d/1HNZC0GznBqoiRD7PQYQFwr-6EZbI2_hkgfv8nK80zlE/edit#heading=h.63gk82yb67mq
 * https://www.tapvote.org/
 * https://youcanbook.me/
 * https://calendar.parliament.uk/
 * https://publications.parliament.uk/pa/cm/cmfutoral/futoral.htm
 * https://builtformp.com/
 * https://www.parliament.uk/business/publications/business-papers/commons/question-book/
 * https://catchapp.mobi/
 * https://www.selbyandainsty.com/
 * https://docs.publishing.service.gov.uk/apps/mapit.html
 * https://www.mysociety.org/category/community/mapit/
 * https://www.theyworkforyou.com/
 * http://www.w4mp.org/
 * https://www.mpsontwitter.co.uk/list/party


## What is a Website Plugin
Self contained code to add extra functionality to a website such as a WordPress' plugin architecture allows users to extend the features and functionality of a website or blog.

If you are hammer all problems look like a nail so if you use AWS serverless microservices then a web plugins look like a web form posting to an API backed via a queue and lambda.

## Separate repos for each lambda service
 * 

## Web forms Websites
 * https://www.quackit.com/html/codes/html_form_to_email.cfm
 * https://www.crazyegg.com/blog/put-forms-on-your-website/
 * https://learning.linkedin.com/blog/tech-tips/send-email-from-a-web-form-with-php
 * https://github.com/dwyl/learn-to-send-email-via-google-script-html-no-server
 * https://github.com/GiacomoLaw/web-form
 * http://javascript-coder.com/javascript-form/javascript-email-form.phtml
 * https://gist.github.com/conceptree/7785672
 * https://github.com/agarrharr/awesome-static-website-services
 * https://formspree.io/
 * https://gist.github.com/escopecz/136f62b66d526bc32006f0d2358a8e15
 * https://medium.com/@asjas/using-formspree-io-on-your-github-pages-a60c290d1ee
 * https://stackoverflow.com/questions/24348223/send-email-from-static-page-hosted-on-github-pages
 * https://www.wpbeaverbuilder.com/creating-wordpress-plugin-easier-think/
 * https://codex.wordpress.org/Writing_a_Plugin
 * https://www.smashingmagazine.com/2011/09/how-to-create-a-wordpress-plugin/
 * https://www.youtube.com/watch?v=34HJlgkxieg
 * https://codeburst.io/how-to-write-a-wordpress-plugin-in-5-minutes-5f8de34f3cd3
 * https://www.wpbeginner.com/wp-tutorials/how-to-create-a-wordpress-plugin/

## AWS Lambda Email
 * https://aws.amazon.com/premiumsupport/knowledge-center/lambda-send-email-ses/
 * https://docs.aws.amazon.com/ses/latest/DeveloperGuide/receiving-email-action-lambda.html
 * https://www.scrivito.com/using-an-aws-lambda-function-to-send-an-email-after-form-submission-f0e6697e59a381ba
 * https://dev.to/centrics/send-e-mails-through-aws-ses-and-lambda-17f2
 * https://www.smashingmagazine.com/2018/11/sending-emails-asynchronously-through-aws-ses/
 * https://medium.com/@xoor/sending-emails-with-attachments-with-aws-lambda-and-node-js-e6a78500227c
 * https://zapier.com/learn/email-marketing/best-transactional-email-sending-services/
 * https://read.iopipe.com/how-to-use-aws-lambda-to-send-high-volume-emails-at-scale-10efe65b2f32
 * https://read.iopipe.com/6-lessons-learned-sending-mass-emails-with-aws-lambda-3c5e56e19571
 * https://intellipaat.com/community/13263/sending-email-via-aws-ses-within-aws-lambda-function
 * https://blogit.create.pt/guilhermeperuzzi/2019/10/21/send-email-in-aws-using-sqs-sns-and-lambda-function/

## Microservice Architecture

```
website https://website.com
|
|
v
Webform with POST data to AWS Lambda frontend
|
|
v
Trigger AWS lambda with API fronend
|
|
v
Subscribe to processing email topic
|
|
v
Linked to email processing queue
|
|
v
Email processing Lambda (Cagney)
|
|
v
Subcribed to emailing topic
|
|
v
Linked to email sending queue (Lacey)
|
|
v
emailing Lambda 
```
