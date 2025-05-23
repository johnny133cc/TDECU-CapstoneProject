# Copilot Prompts for Caption Generation and Compliance Checking

This document provides detailed prompts for interacting with the Caption Creator (AI Agent 1) and the Compliance Checker (AI Agent 2) in the TDECU Caption Generation System.

## **1. Caption Creator (AI Agent 1)**

### Objective:
The Caption Creator AI is responsible for generating concise, engaging captions based on the input content. It takes the content of a post and generates a caption that is professional, relevant, and tailored to TDECU's audience.

### Sample Prompt:
To prompt the Caption Creator, input the following command:

"Give me a caption to post based on the following content:"


After this prompt, provide the article content you wish to create a caption for. For example:

**Input Example:**
Give me a caption to post based on the following content: Enhancing the Member Experience - Piloting QR Codes in our Member Centers. Beginning Tuesday, April 1, four Member Centers began using QR codes to enhance the Member experience. Members and potential new Members can use the codes to start and complete their application while waiting for the Member Specialist. Through their phones, they can also:

- Select products
- Complete the Know Your Customer (KYC) process
- Upload their ID The Member Specialist will review the application before it is finalized to ensure the Member has chosen the best products. This pilot is a step toward streamlining processes, increasing automation, and driving Membership Growth. Feedback from our members has been positive, and we hope to expand this initiative to more centers.


**Sample Output:**

🚀 Exciting News! Starting April 1, four of our Member Centers are piloting QR codes to enhance your experience. 📱 Use your phone to start and complete applications, select products, and more while you wait. Shoutout to our amazing team and pilot centers for making this possible! #TDECU #Innovation #MemberExperience


### Instructions for the Caption Creator:
- The caption should be **concise** and **within 250 characters**.
- Ensure the caption is **engaging** and **relevant** to the content.
- Maintain a **professional tone** with a hint of **casual communication** appropriate for social media.
- Use **emojis** where appropriate to increase engagement.
- Avoid using **offensive** or **inappropriate language**.
- Always ensure the final caption **aligns with TDECU's values** and tone.

---

## **2. Compliance Checker (AI Agent 2)**

### Objective:
The Compliance Checker AI is responsible for evaluating the caption generated by the Caption Creator and ensuring that it adheres to TDECU's compliance guidelines. This includes reviewing for sensitive financial data, proprietary information, and offensive language.

### Sample Prompt:
To prompt the Compliance Checker, input the following command:

"Check compliance requirements for this caption -"

After this prompt, provide the caption text you wish to check for compliance. For example:

**Input Example:**

Check compliance requirements for this caption - 🚀 Exciting News! Starting April 1, four of our Member Centers are piloting QR codes to enhance your experience. 📱 Use your phone to start and complete applications, select products, and more while you wait. Shoutout to our amazing team and pilot centers for making this possible! #TDECU #Innovation #MemberExperience


**Sample Output:**

🚀 Exciting News! Starting April 1, four of TDECU's Member Centers are piloting QR codes to enhance the experience. 📱 Use a phone to start and complete applications, select products, and more while waiting. Shoutout to TDECU's amazing team and pilot centers for making this possible! #TDECU #Innovation #MemberExperience


### Instructions for the Compliance Checker:
- **Sensitive Content Evaluation:**
  - Scan for sensitive financial data such as monetary amounts, percentages, and ratios.
  - Check for proprietary product or internal names (other than "TDECU").
  - Ensure there is no offensive language or inappropriate content.
  
- **Compliance Adjustment:**
  - If sensitive financial or proprietary content is detected, **replace** it with generic language (e.g., “a significant amount,” “several sessions,” or “our financial services partner”).
  - **Retain mentions of "TDECU"** and **non-financial numbers** (e.g., "10 volunteers," "200 participants").
  - Reword the caption to be in **third-person** (e.g., “TDECU hosted an event” instead of “We hosted an event”).
  
- **Output:**
  - Return only the revised **caption text**, with no additional commentary.
  - Ensure compliance and maintain the original sentiment of the caption.
  
---

### Summary of AI Agent Prompts

- **Caption Creator Prompt:** Generate a concise, engaging caption based on provided content.
- **Compliance Checker Prompt:** Ensure the generated caption meets TDECU's compliance guidelines.

By following these prompts, the AI agents work seamlessly to generate and review captions, ensuring they are both engaging and compliant with TDECU’s standards.


