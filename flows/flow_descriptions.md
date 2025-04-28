# Flow Descriptions for Caption Generation System

This document outlines the steps involved in the caption generation system using Power Automate flows. The system is designed to automate the process of generating captions from articles, checking compliance, and updating a SharePoint list with the results.

## 1. **Triggers for Caption Creator**

- **Trigger:** A new article file (.docx) is uploaded to the designated SharePoint folder.
- **Process:** The article content is extracted from the .docx file.
- **AI Agent:** The content is sent to the Caption Creator AI agent, which generates captions based on the article.
- **List Update:** A new item is created in the SharePoint list, setting the title to the article's name and the body as "NA" temporarily.

## 2. **Connect to Compliance Checker**

- **Process:** The Caption Creator's generated caption is sent to the Compliance Checker for review.
- **AI Agent:** The Compliance Checker ensures the generated caption adheres to compliance guidelines and makes adjustments if needed.
- **List Update:** Once compliance is checked, the revised caption is passed back to the system.

## 3. **Compliance Checker Send Content**

- **Process:** The Compliance Checker sends the reviewed content via an HTTP post request.
- **Flow Trigger:** This triggers the fourth flow to update the item in the list with the revised caption.

## 4. **Final Update to List Item**

- **Process:** The system identifies items in the list where the body is still set as "NA."
- **AI Agent:** Once the caption has been revised and approved, it is updated in the item body.
- **Outlook Notification:** An Outlook notification is sent to inform relevant stakeholders that the caption has been updated and is now compliant.
