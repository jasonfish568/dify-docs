# Connect to an External Knowledge Base

> To make a distinction, knowledge bases independent of the Dify platform are collectively referred to as **"external knowledge bases"** in this article.

## Functional Introduction

For developers with advanced content retrieval requirements, **the built-in knowledge base functionality and text retrieval mechanisms of the Dify platform may have limitations, particularly in terms of customizing recall results.**

Due to the requirement of higher accuracy of text retrieval and recall, as well as the need to manage internal materials, some developer teams choose to independently develop RAG algorithms and independently maintain text retrieval systems, or uniformly host content to cloud vendors' knowledge base services (such as [AWS Bedrock](https://aws.amazon.com/bedrock/)).

As a neutral platform for LLM application development, Dify is committed to providing developers with a wider range of options.

The **Connect to External Knowledge Base** feature enables integration between the Dify platform and external knowledge bases. Through API services, AI applications can access a broader range of information sources. This capability offers two key advantages:

* The Dify platform can directly obtain the text content hosted in the cloud service provider's knowledge base, so that developers do not need to repeatedly move the content to the knowledge base in Dify;
* The Dify platform can directly obtain the text content processed by algorithms in the self-built knowledge base. Developers only need to focus on the information retrieval mechanism of the self-built knowledge base and continuously optimize and improve the accuracy of information retrieval.

<figure><img src="../../.gitbook/assets/image (117).png" alt=""><figcaption><p>Principle of external knowledge base connection</p></figcaption></figure>

Here are the detailed steps for connecting to external knowledge:

## 1. Create a Compliant External Knowledge Base API

Create a compliant External Knowledge Base API before setting up the API service, please refer to Dify's [External Knowledge Base API](external-knowledge-api-documentation.md) specifications to ensure successful integration between your external knowledge base and Dify.

## 2. Add External Knowledge API

> Currently, when connecting to external knowledge bases, Dify only supports retrieval permissions and does not support optimization or modification of external knowledge bases. Developers need to maintain external knowledge bases themselves.

Navigate to the **"Knowledge"** page, click **"External Knowledge API"** in the upper right corner, then click **"Add External Knowledge API"**. Follow the page prompts to fill in the following information:

* Name Customizable name to distinguish different external knowledge APIs;
* API Endpoint The URL of the external knowledge base API endpoint, e.g., api-endpoint/retrieval; refer to the [External Knowledge API](external-knowledge-api-documentation.md) for detailed instructions;
* API Key Connection key for the external knowledge, refer to the [External Knowledge API](external-knowledge-api-documentation.md) for detailed instructions.

<figure><img src="../../../img/connect-kb-1-en.png" alt=""><figcaption><p>Associate External Knowledge API</p></figcaption></figure>

## 3. Connect to the External Knowledge Base

Go to the **"Knowledge"** page, click **"Connect to an External Knowledge Base"** under the Add Knowledge Base card to direct to the parameter configuration page.

<figure><img src="../../../img/connect-kb-2-en.png" alt=""><figcaption><p>Connect to the external knowledge base</p></figcaption></figure>

Fill in the following parameters:

* **Knowledge base name & description**
*   **External Knowledge API**

    Select the external knowledge base API associated in step 2; Dify will call the text content stored in the external knowledge base through the API connection method.
*   **External knowledge ID**

    Specify the particular external knowledge base ID to be associated, refer to the external knowledge base API definition for detailed instructions.
*   **Retrieval Setting**

    **Top K:** When a user sends a question, it will request the external knowledge API to obtain highly relevant content chunks. This parameter is used to filter text chunks with high similarity to the user's question. The default value is 3; the higher the value, the more text chunks with relevant similarities will be retrieval.

    **Score Threshold:** The similarity threshold for text chunk filtering, only retrievaling text chunks that exceed the set score. The default value is 0.5. A higher value indicates a higher requirement for similarity between the text and the question, expecting fewer retrievaled text chunks, and the results will be relatively more precise.

<figure><img src="../../../img/connect-kb-3-en.webp" alt=""><figcaption></figcaption></figure>

## 4. Test External Knowledge Base and Retrieval Results

After connected with the external knowledge base, developers can simulate possible question keywords in the **"Retrieval Testing"** to preview text chunks that might be retrieval. If you are unsatisfied with the retrieval results, try modifying the **External Knowledge Base Settings** or adjusting the retrieval strategy of the external knowledge base.

<figure><img src="../../../img/connect-kb-4-en.png" alt=""><figcaption><p>Test external knowledge base connection and retrieval</p></figcaption></figure>

## 5. Integrating External Knowledge base in Applications

*   **Chatbot / Agent** type application

    Associate the external knowledge base in the orchestration page within Chatbot / Agent type applications.

<figure><img src="../../../img/connect-kb-5-en.png" alt=""><figcaption><p>Chatbot / Agent</p></figcaption></figure>

*   **Chatflow / Workflow** type application

    Add a **"Knowledge Retrieval"** node and select the external knowledge base.

<figure><img src="../../../img/connect-kb-6-en.png" alt=""><figcaption><p>Chatflow / Workflow</p></figcaption></figure>

## 6. Manage External Knowledge

Navigate to the **"Knowledge"** page, external knowledge base cards will list an **EXTERNAL** label in the upper right corner. Select the knowledge base needs to be modified, click **"Settings"** to modify the following information:

* **Knowledge base name and description**
*   **Permissions**

    Provide **"Only me"**, **"All team members"**, and **"Partial team members"** permission scope. Those without permission will not be able to access the knowledge base. If you choose to make the knowledge base public to other members, it means that other members also have the rights to view, edit, and delete the knowledge base.
*   **Retrieval Setting**

    **Top K:** When a user sends a question, it will request the external knowledge API to obtain highly relevant content segments. This parameter is used to filter text chunks with high similarity to the user's question. The default value is 3; the higher the value, the more text chunks with relevant similarities will be retrievaled.

    **Score threshold:** The similarity threshold for text chunk filtering, only retrievaling text chunks that exceed the set score. The default value is 0.5. A higher value indicates a higher requirement for similarity between the text and the question, expecting fewer retrievaled text chunks, and the results will be relatively more precise.

The **"External Knowledge API"** and **"External Knowledge ID"** associated with the external knowledge base do not support modification. If modification is needed, please associate a new **"External Knowledge API"** and reset it.

<figure><img src="../../../img/connect-kb-7-en.webp" alt=""><figcaption></figcaption></figure>

### Connection Examples

#### AWS Bedrock

[How to connect with AWS Bedrock Knowledge Base](../../learn-more/use-cases/how-to-connect-aws-bedrock.md "mention")

#### LlamaCloud

Dify provides an official LlamaCloud plugin that helps you quickly connect to LlamaCloud knowledge bases.

##### Plugin Installation

1. Visit the Dify [Marketplace](https://marketplace.dify.ai/) and search for `LlamaCloud`
2. Install and configure the LlamaCloud plugin according to the instructions
3. Enable the plugin in the Dify platform
4. Fill in the LlamaCloud API key and other necessary information following the plugin configuration wizard
5. After configuration is complete, you can see the connected external knowledge base in your knowledge base list

With the LlamaCloud plugin, you can directly use LlamaCloud's powerful retrieval capabilities in the Dify platform without writing custom APIs.

For more information about how it works, please refer to the plugin's [GitHub repository](https://github.com/langgenius/dify-official-plugins/tree/main/extensions/llamacloud).

##### Video Tutorial

The following video demonstrates in detail how to use the LlamaCloud plugin to connect to external knowledge bases:

{% embed url="https://www.youtube.com/embed/FaOzKZRS-2E" %}

## FAQ

**How to Fix the Errors Occurring When Connecting to External Knowledge API?**

Solutions corresponding to each error code in the return information:

| Error Code | Result                              | Solutions                                                   |
| ---------- | ----------------------------------- | ----------------------------------------------------------- |
| 1001       | Invalid Authorization header format | Please check the Authorization header format of the request |
| 1002       | Authorization failed                | Please check whether the API Key you entered is correct.    |
| 2001       | The knowledge is not exist          | Please check the external repository                        |
