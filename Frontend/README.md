# Frontend Technical Specifiation

- Create a static website that acts as my resume in HTML

## Resume Format Considerations

Living in the UK we want to keep our resume to a PDF format when being sent to recruiters / applications. We do not want to include overly person info, for eg. DOB, photo, full address. This should also be a maximum of 2 pages in length.

We want to ensure our format is ATG freindly to align with company AI checks.

We want to include the following information within our resume in this order:
- Name & Contact Details
- Linkedin Profile
- Short Summary
- Skills
- Experiance
- Certifactions

### ATG Freindly Template Example

![Template](./Docs/ATG-Template.jpg)

## Resume Format Generation

I have an existing resume using the template above, which is two pages in length, and follows the mentioned considerations. 

 Below are two screenshots one of each page of what my resume looks like, the below has personal info redacted at the top right on the first page.

![](./Docs/CV%20Page%201.jpg)
![](./Docs/CV%20Page%202.jpg)

I do not have much experience with HTML and will be using ChatGPT 5.1 to assist with this process, I will then manually adjust as required.

### Prompt to ChatGPT 5.1

'''text

I'm doing the cloud resume challenge, as part of this I need to create my existing CV into a HTML format.

I have attached my CV as a PDF that I would like you to convert into HTML, as part of this do not use a CSS framework and use the least amount of CSS tags.
'''

This is the [genereated output](./Docs/Nov-23-2025-resume-generation-minimal.html) which we will refactoring

This is what the generated HTML looks like:

![](./Docs/Nov-23-2025-resume-generation-minimal.jpg)

## HTML Adjustments

The output of the generated HTML is fairly inline wtih our examples, all information has been kept and has mostly followed the format.

- Our provided CV did include my mobile number and address, we have edited the headers on lines 56 and 58 to state "redacted" for privacy purposes, this has been edited in the generated HTML.
- We wanted our page to be using HTML5 and we can see the output has selected "!DOCTYPE html" which is required for HTML this also prevent the viewing browser from switcihng to "quirks mode" when attempting to render.
- As our page will only be using english we can see that it has selected UTF-8 which will serve this purpose.