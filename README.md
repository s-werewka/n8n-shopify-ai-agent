# n8n-shopify-ai-agent
# 🛒 Shopify AI Customer Support & Routing Workflow (n8n + OpenAI + Gmail)

Automated customer support ticketing and routing system built in **n8n**. The workflow integrates **Gmail** and **Shopify** APIs, leveraging **OpenAI** for semantic email classification, automated intent detection, and structured routing with human-in-the-loop oversight.

---

## 🚀 Key Features

1. **Semantic Email Classification:** Automatically processes incoming support emails via Gmail API and classifies intents (e.g., Order Status, Returns & Refunds, General Product Inquiries, Order Modifications) using OpenAI API.
2. **Shopify API Integration:** Automatically fetches order details, tracking status, and fulfillment data directly from Shopify to draft context-aware responses.
3. **Smart Routing & Prioritization:** Tags, categorizes, and routes tickets based on urgency, customer history, and issue type.
4. **Human-In-The-Loop Escalation:** Complex or high-risk requests (e.g., refund approvals, VIP escalations) are flagged and forwarded to human support reps for manual review before sending.
5. **Automated Response Generation:** Crafts personalized, professional email replies using dynamic context retrieved from Shopify.

---

## 🛠️ Tech Stack & Nodes

- **Workflow Engine:** n8n
- **AI & NLP:** OpenAI API (Intent Classification & Dynamic Draft Generation)
- **E-Commerce Integration:** Shopify REST / Admin API
- **Communication:** Gmail API
- **Logic & Formatting:** Switch Nodes, JavaScript Code Nodes, IF Conditionals

---

## 📥 Quick Setup Guide

1. Clone or download this repository.
2. Import the `workflow.json` file into your **n8n** instance.
3. Configure required credentials:
   - **OpenAI API Key**
   - **Shopify Admin API Token & Store Domain**
   - **Gmail OAuth2 Credentials**
4. Adjust the prompt and escalation thresholds in the OpenAI / Switch nodes to match your store policies.
5. Activate the workflow!

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).
