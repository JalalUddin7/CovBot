# CovBot - Covid-19 Response Chatbot

Many employees have questions regarding COVID-19 and their company’s response to it. This provides the opportunity for employers to create an FAQ document and get that information out to their employees instantly over a chatbot on their website – reducing traffic on landlines and emails. 

Credit: Based on Joe Plumb’s suggestion.

## Demo

The link to the demo website: https://covid-19-faqbot.azurewebsites.net/

**Question:** 

“What are the symptoms?”

**Response:** 

“We are still learning more about the symptoms that this virus causes in infected people as the outbreak progresses. Symptoms associated with coronaviruses can vary:

- Common coronaviruses can cause symptoms similar to a common cold, such as fever, cough, sore throat, and feeling unwell.”

## Steps to reproduce:

1. Go to QnAMaker.ai

   a.    Create Knowledge Base (KB) (upload word document or point to URL)

   b.    Publish KB 

   c.    Click “Create Bot” Button that appears after publishing the KB

   

2. Go to Azure Portal

   a.    Click on “Channels” in the Web App Bot resource that was just created

   b.    Obtain secret key. Obtain the iframe embed code. Paste in secret where it says “YOUR_SECRET_HERE”

   

3. Go to Visual Studio Code

   a.    Paste the iframe embed code with the newly added secret into your HTML

   b.    Deploy to Web App (if existing) or Create New Web App to upload website to Azure

## Resources

The knowledge base is currently based on: https://coronavirus.dc.gov/page/covid-19-faqs

The website template is from http://www.templatewire.com/interact-free-one-page-bootstrap-template - free templates for personal and commercial use. I have simply cut it down and adapted it for the chatbot use case.

The QnAMaker steps are based on this link:https://docs.microsoft.com/en-us/azure/cognitive-services/QnAMaker/Quickstarts/create-publish-knowledge-base
