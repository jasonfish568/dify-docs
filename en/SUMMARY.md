# Table of contents

## Getting Started

* [Welcome to Dify](README.md)
  * [Features and Specifications](getting-started/readme/features-and-specifications.md)
  * [List of Model Providers](getting-started/readme/model-providers.md)
* [Dify Community](getting-started/install-self-hosted/README.md)
  * [Deploy with Docker Compose](getting-started/install-self-hosted/docker-compose.md)
  * [Start with Local Source Code](getting-started/install-self-hosted/local-source-code.md)
  * [Deploy with aaPanel](getting-started/install-self-hosted/bt-panel.md)
  * [Start Frontend Docker Container Separately](getting-started/install-self-hosted/start-the-frontend-docker-container.md)
  * [Environment Variables Explanation](getting-started/install-self-hosted/environments.md)
  * [FAQs](getting-started/install-self-hosted/faqs.md)
* [Dify Cloud](getting-started/cloud.md)
* [Dify Premium on AWS](getting-started/dify-premium.md)
* [Dify for Education](getting-started/dify-for-education.md)

## Guides

* [Model](guides/model-configuration/README.md)
  * [Add New Provider](guides/model-configuration/new-provider.md)
  * [Predefined Model Integration](guides/model-configuration/predefined-model.md)
  * [Custom Model Integration](guides/model-configuration/customizable-model.md)
  * [Interfaces](guides/model-configuration/interfaces.md)
  * [Schema](guides/model-configuration/schema.md)
  * [Load Balancing](guides/model-configuration/load-balancing.md)
* [Application Orchestration](guides/application-orchestrate/README.md)
  * [Create Application](guides/application-orchestrate/creating-an-application.md)
  * [Chatbot Application](guides/application-orchestrate/chatbot-application.md)
    * [Multiple Model Debugging](guides/application-orchestrate/multiple-llms-debugging.md)
  * [Agent](guides/application-orchestrate/agent.md)
  * [Application Toolkits](guides/application-orchestrate/app-toolkits/README.md)
    * [Moderation Tool](guides/application-orchestrate/app-toolkits/moderation-tool.md)
* [Workflow](guides/workflow/README.md)
  * [Key Concepts](guides/workflow/key-concepts.md)
  * [Variables](guides/workflow/variables.md)
  * [Node Description](guides/workflow/node/README.md)
    * [Start](guides/workflow/node/start.md)
    * [End](guides/workflow/node/end.md)
    * [Answer](guides/workflow/node/answer.md)
    * [LLM](guides/workflow/node/llm.md)
    * [Knowledge Retrieval](guides/workflow/node/knowledge-retrieval.md)
    * [Question Classifier](guides/workflow/node/question-classifier.md)
    * [Conditional Branch IF/ELSE](guides/workflow/node/ifelse.md)
    * [Code Execution](guides/workflow/node/code.md)
    * [Template](guides/workflow/node/template.md)
    * [Doc Extractor](guides/workflow/node/doc-extractor.md)
    * [List Operator](guides/workflow/node/list-operator.md)
    * [Variable Aggregator](guides/workflow/node/variable-aggregator.md)
    * [Variable Assigner](guides/workflow/node/variable-assigner.md)
    * [Iteration](guides/workflow/node/iteration.md)
    * [Parameter Extraction](guides/workflow/node/parameter-extractor.md)
    * [HTTP Request](guides/workflow/node/http-request.md)
    * [Agent](guides/workflow/node/agent.md)
    * [Tools](guides/workflow/node/tools.md)
    * [Loop](guides/workflow/node/loop.md)
  * [Shortcut Key](guides/workflow/shortcut-key.md)
  * [Orchestrate Node](guides/workflow/orchestrate-node.md)
  * [File Upload](guides/workflow/file-upload.md)
  * [Error Handling](guides/workflow/error-handling/README.md)
    * [Predefined Error Handling Logic](guides/workflow/error-handling/predefined-error-handling-logic.md)
    * [Error Type](guides/workflow/error-handling/error-type.md)
  * [Additional Features](guides/workflow/additional-features.md)
  * [Debug and Preview](guides/workflow/debug-and-preview/README.md)
    * [Preview and Run](guides/workflow/debug-and-preview/yu-lan-yu-yun-hang.md)
    * [Step Run](guides/workflow/debug-and-preview/step-run.md)
    * [Conversation/Run Logs](guides/workflow/debug-and-preview/log.md)
    * [Checklist](guides/workflow/debug-and-preview/checklist.md)
    * [Run History](guides/workflow/debug-and-preview/history.md)
  * [Application Publishing](guides/workflow/publish.md)
  * [Structured Outputs](guides/workflow/structured-outputs.md)
  * [Bulletin: Image Upload Replaced by File Upload](guides/workflow/bulletin.md)
* [Knowledge](guides/knowledge-base/README.md)
  * [Create Knowledge](guides/knowledge-base/create-knowledge-and-upload-documents.md)
    * [1. Import Text Data](guides/knowledge-base/create-knowledge-and-upload-documents/import-content-data/README.md)
      * [1.1 Import Data from Notion](guides/knowledge-base/create-knowledge-and-upload-documents/import-content-data/sync-from-notion.md)
      * [1.2 Import Data from Website](guides/knowledge-base/create-knowledge-and-upload-documents/import-content-data/sync-from-website.md)
    * [2. Choose a Chunk Mode](guides/knowledge-base/create-knowledge-and-upload-documents/chunking-and-cleaning-text.md)
    * [3. Select the Indexing Method and Retrieval Setting](guides/knowledge-base/create-knowledge-and-upload-documents/setting-indexing-methods.md)
  * [Manage Knowledge](guides/knowledge-base/knowledge-and-documents-maintenance/README.md)
    * [Maintain Documents](guides/knowledge-base/knowledge-and-documents-maintenance/maintain-knowledge-documents.md)
    * [Maintain Knowledge via API](guides/knowledge-base/knowledge-and-documents-maintenance/maintain-dataset-via-api.md)
  * [Metadata](guides/knowledge-base/metadata.md)
  * [Integrate Knowledge Base within Application](guides/knowledge-base/integrate-knowledge-within-application.md)
  * [Retrieval Test / Citation and Attributions](guides/knowledge-base/retrieval-test-and-citation.md)
  * [Knowledge Request Rate Limit](guides/knowledge-base/knowledge-request-rate-limit.md)
  * [Connect to an External Knowledge Base](guides/knowledge-base/connect-external-knowledge-base.md)
  * [External Knowledge API](guides/knowledge-base/external-knowledge-api-documentation.md)
* [Tools](guides/tools/README.md)
  * [Quick Tool Integration](guides/tools/quick-tool-integration.md)
  * [Advanced Tool Integration](guides/tools/advanced-tool-integration.md)
  * [Tool Configuration](guides/tools/tool-configuration/README.md)
    * [Google](guides/tools/tool-configuration/google.md)
    * [Bing](guides/tools/tool-configuration/bing.md)
    * [SearchApi](guides/tools/tool-configuration/searchapi.md)
    * [StableDiffusion](guides/tools/tool-configuration/stable-diffusion.md)
    * [Dall-e](guides/tools/tool-configuration/dall-e.md)
    * [Perplexity Search](guides/tools/tool-configuration/perplexity.md)
    * [AlphaVantage](guides/tools/tool-configuration/alphavantage.md)
    * [Youtube](guides/tools/tool-configuration/youtube.md)
    * [SearXNG](guides/tools/tool-configuration/searxng.md)
    * [Serper](guides/tools/tool-configuration/serper.md)
    * [SiliconFlow (Flux AI Supported)](guides/tools/tool-configuration/siliconflow.md)
    * [ComfyUI](guides/tools/tool-configuration/comfyui.md)
* [Publishing](guides/application-publishing/README.md)
  * [Publish as a Single-page Web App](guides/application-publishing/launch-your-webapp-quickly/README.md)
    * [Web App Settings](guides/application-publishing/launch-your-webapp-quickly/web-app-settings.md)
    * [Text Generator Application](guides/application-publishing/launch-your-webapp-quickly/text-generator.md)
    * [Conversation Application](guides/application-publishing/launch-your-webapp-quickly/conversation-application.md)
  * [Embedding In Websites](guides/application-publishing/embedding-in-websites.md)
  * [Developing with APIs](guides/application-publishing/developing-with-apis.md)
  * [Re-develop Based on Frontend Templates](guides/application-publishing/based-on-frontend-templates.md)
* [Annotation](guides/annotation/README.md)
  * [Logs and Annotation](guides/annotation/logs.md)
  * [Annotation Reply](guides/annotation/annotation-reply.md)
  * [Maintain Annotation via API](guides/annotation/maintain-annotation-via-api.md)
* [Monitoring](guides/monitoring/README.md)
  * [Data Analysis](guides/monitoring/analysis.md)
  * [Integrate External Ops Tools](guides/monitoring/integrate-external-ops-tools/README.md)
    * [Integrate LangSmith](guides/monitoring/integrate-external-ops-tools/integrate-langsmith.md)
    * [Integrate Langfuse](guides/monitoring/integrate-external-ops-tools/integrate-langfuse.md)
    * [Integrate Opik](guides/monitoring/integrate-external-ops-tools/integrate-opik.md)
* [Extension](guides/extension/README.md)
  * [API-Based Extension](guides/extension/api-based-extension/README.md)
    * [External Data Tool](guides/extension/api-based-extension/external-data-tool.md)
    * [Deploy API Tools with Cloudflare Workers](guides/extension/api-based-extension/cloudflare-workers.md)
    * [Moderation](guides/extension/api-based-extension/moderation.md)
  * [Code-Based Extension](guides/extension/code-based-extension/README.md)
    * [External Data Tool](guides/extension/code-based-extension/external-data-tool.md)
    * [Moderation](guides/extension/code-based-extension/moderation.md)
* [Collaboration](guides/workspace/README.md)
  * [Discover](guides/workspace/app.md)
  * [Invite and Manage Members](guides/workspace/invite-and-manage-members.md)
* [Management](guides/management/README.md)
  * [App Management](guides/management/app-management.md)
  * [Team Members Management](guides/management/team-members-management.md)
  * [Personal Account Management](guides/management/personal-account-management.md)
  * [Subscription Management](guides/management/subscription-management.md)
  * [Version Control](guides/management/version-control.md)

## Workshop

* [Basic](workshop/basic/README.md)
  * [How to Build an AI Image Generation App](workshop/basic/build-ai-image-generation-app.md)
* [Intermediate](workshop/intermediate/README.md)
  * [Build An Article Reader Using File Upload](workshop/intermediate/article-reader.md)
  * [Building a Smart Customer Service Bot Using a Knowledge Base](workshop/intermediate/customer-service-bot.md)
  * [Generating analysis of Twitter account using Chatflow Agent](workshop/intermediate/twitter-chatflow.md)

## Community

* [Seek Support](community/support.md)
* [Become a Contributor](community/contribution.md)
* [Contributing to Dify Documentation](community/docs-contribution.md)

## Plugins

* [Introduction](plugins/introduction.md)
* [Quick Start](plugins/quick-start/README.md)
  * [Install and Use Plugins](plugins/quick-start/install-plugins.md)
  * [Develop Plugins](plugins/quick-start/develop-plugins/README.md)
    * [Initialize Development Tools](plugins/quick-start/develop-plugins/initialize-development-tools.md)
    * [Tool Plugin](plugins/quick-start/develop-plugins/tool-plugin.md)
    * [Model Plugin](plugins/quick-start/develop-plugins/model-plugin/README.md)
      * [Create Model Providers](plugins/quick-start/develop-plugins/model-plugin/create-model-providers.md)
      * [Integrate the Predefined Model](plugins/quick-start/develop-plugins/model-plugin/predefined-model.md)
      * [Integrate the Customizable Model](plugins/quick-start/develop-plugins/model-plugin/customizable-model.md)
    * [Agent Strategy Plugin](plugins/quick-start/develop-plugins/agent-strategy-plugin.md)
    * [Extension Plugin](plugins/quick-start/develop-plugins/extension-plugin.md)
    * [Bundle](plugins/quick-start/develop-plugins/bundle.md)
  * [Debug Plugin](plugins/quick-start/debug-plugin.md)
* [Manage Plugins](plugins/manage-plugins.md)
* [Schema Specification](plugins/schema-definition/README.md)
  * [Manifest](plugins/schema-definition/manifest.md)
  * [Endpoint](plugins/schema-definition/endpoint.md)
  * [Tool](plugins/schema-definition/tool.md)
  * [Agent](plugins/schema-definition/agent.md)
  * [Model](plugins/schema-definition/model/README.md)
    * [Model Designing Rules](plugins/schema-definition/model/model-designing-rules.md)
    * [Model Schema](plugins/schema-definition/model/model-schema.md)
  * [General Specifications](plugins/schema-definition/general-specifications.md)
  * [Persistent Storage](plugins/schema-definition/persistent-storage.md)
  * [Reverse Invocation of the Dify Service](plugins/schema-definition/reverse-invocation-of-the-dify-service/README.md)
    * [App](plugins/schema-definition/reverse-invocation-of-the-dify-service/app.md)
    * [Model](plugins/schema-definition/reverse-invocation-of-the-dify-service/model.md)
    * [Tool](plugins/schema-definition/reverse-invocation-of-the-dify-service/tool.md)
    * [Node](plugins/schema-definition/reverse-invocation-of-the-dify-service/node.md)
* [Best Practice](plugins/best-practice/README.md)
  * [Develop a Slack Bot Plugin](plugins/best-practice/develop-a-slack-bot-plugin.md)
  * [Dify MCP Plugin Guide: Connect Zapier and Automate Email Delivery with Ease](plugins/best-practice/how-to-use-mcp-zapier.md)
* [Publish Plugins](plugins/publish-plugins/README.md)
  * [Publish Plugins Automatically](plugins/publish-plugins/plugin-auto-publish-pr.md)
  * [Publish to Dify Marketplace](plugins/publish-plugins/publish-to-dify-marketplace/README.md)
    * [Plugin Developer Guidelines](plugins/publish-plugins/publish-to-dify-marketplace/plugin-developer-guidelines.md)
    * [Plugin Privacy Protection Guidelines](plugins/publish-plugins/publish-to-dify-marketplace/plugin-privacy-protection-guidelines.md)
  * [Publish to Your Personal GitHub Repository](plugins/publish-plugins/publish-plugin-on-personal-github-repo.md)
  * [Package the Plugin File and Publish it](plugins/publish-plugins/package-plugin-file-and-publish.md)
  * [Signing Plugins for Third-Party Signature Verification](plugins/publish-plugins/signing-plugins-for-third-party-signature-verification.md)
* [FAQ](plugins/faq.md)

## Development

* [Backend](development/backend/README.md)
  * [DifySandbox](development/backend/sandbox/README.md)
    * [Contribution Guide](development/backend/sandbox/contribution.md)
* [Models Integration](development/models-integration/README.md)
  * [Integrate Open Source Models from Hugging Face](development/models-integration/hugging-face.md)
  * [Integrate Open Source Models from Replicate](development/models-integration/replicate.md)
  * [Integrate Local Models Deployed by Xinference](development/models-integration/xinference.md)
  * [Integrate Local Models Deployed by OpenLLM](development/models-integration/openllm.md)
  * [Integrate Local Models Deployed by LocalAI](development/models-integration/localai.md)
  * [Integrate Local Models Deployed by Ollama](development/models-integration/ollama.md)
  * [Integrate Models on LiteLLM Proxy](development/models-integration/litellm.md)
  * [Integrating with GPUStack for Local Model Deployment](development/models-integration/gpustack.md)
  * [Integrating AWS Bedrock Models (DeepSeek)](development/models-integration/aws-bedrock-deepseek.md)
* [Migration](development/migration/README.md)
  * [Migrating Community Edition to v1.0.0](development/migration/migrate-to-v1.md)

## Learn More

* [Use Cases](learn-more/use-cases/README.md)
  * [DeepSeek & Dify Integration Guide: Building AI Applications with Multi-Turn Reasoning](learn-more/use-cases/integrate-deepseek-to-build-an-ai-app.md)
  * [Private Deployment of Ollama + DeepSeek + Dify: Build Your Own AI Assistant](learn-more/use-cases/private-ai-ollama-deepseek-dify.md)
  * [Build a Notion AI Assistant](learn-more/use-cases/build-an-notion-ai-assistant.md)
  * [Create a MidJourney Prompt Bot with Dify](learn-more/use-cases/create-a-midjourney-prompt-bot-with-dify.md)
  * [Create an AI Chatbot with Business Data in Minutes](learn-more/use-cases/create-an-ai-chatbot-with-business-data-in-minutes.md)
  * [Integrating Dify Chatbot into Your Wix Website](learn-more/use-cases/how-to-integrate-dify-chatbot-to-your-wix-website.md)
  * [How to connect with AWS Bedrock Knowledge Base？](learn-more/use-cases/how-to-connect-aws-bedrock.md)
  * [Building the Dify Scheduler](learn-more/use-cases/dify-schedule.md)
  * [Building an AI Thesis Slack Bot on Dify](learn-more/use-cases/building-an-ai-thesis-slack-bot.md)
* [Extended Reading](learn-more/extended-reading/README.md)
  * [What is LLMOps?](learn-more/extended-reading/what-is-llmops.md)
  * [Retrieval-Augmented Generation (RAG)](learn-more/extended-reading/retrieval-augment/README.md)
    * [Hybrid Search](learn-more/extended-reading/retrieval-augment/hybrid-search.md)
    * [Re-ranking](learn-more/extended-reading/retrieval-augment/rerank.md)
    * [Retrieval Modes](learn-more/extended-reading/retrieval-augment/retrieval.md)
  * [How to Use JSON Schema Output in Dify?](learn-more/extended-reading/how-to-use-json-schema-in-dify.md)
* [FAQ](learn-more/faq/README.md)
  * [Self-Host](learn-more/faq/install-faq.md)
  * [LLM Configuration and Usage](learn-more/faq/use-llms-faq.md)
  * [Plugins](learn-more/faq/plugins.md)

## Policies

* [Open Source License](policies/open-source.md)
* [User Agreement](policies/agreement/README.md)
  * [Terms of Service](https://dify.ai/terms)
  * [Privacy Policy](https://dify.ai/privacy)
  * [Get Compliance Report](policies/agreement/get-compliance-report.md)

## Features

* [Workflow](features/workflow.md)
