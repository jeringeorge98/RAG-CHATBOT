# RAG Chatbot in AmazonBedrock


**RAG (Retrieval Augmented Generation) chatbot** is an AI-powered chatbot that enhances AI language models by incorporating documentation or/and source URLs as the data source. This technique enables the chatbot to provide accurate and up-to-date responses, even if the required information is the latest or unavailable online. While non-RAG chatbots rely on pre-trained data and may struggle to offer current or specialized knowledge, the RAG chatbots can retrieve information from a specific knowledge base or external sources. This makes RAG chatbots particularly useful for applications, where up-to-date information is critical, such as legal or government updates, product releases, or personalized content.

## Table of Contents

- [Used Tools and Concepts](#used-tools-and-concepts)
- [Objectives](#objectives)
- [Workfkow](#workflow)
- [Document](#document)
- [Demo](#demo)

## Used Tools and Concepts:

![AWS](https://img.shields.io/badge/AWS%20-%20?style=for-the-badge&logo=AmazonWebServices&logoColor=FF9900&logoSize=auto&color=232F3E)
![Amazon Bedrock](https://custom-icon-badges.demolab.com/badge/Amazon%20Bedrock%20-%20?style=for-the-badge&logo=amazon-bedrock&color=01a88d)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3%20-%20?style=for-the-badge&logo=AmazonS3&logoColor=white&color=%23569A31)
![Amazon OpenSearch Service](https://custom-icon-badges.demolab.com/badge/Amazon%20OpenSearch%20Service%20-%20?style=for-the-badge&logo=amazon-opensearch&color=884df7)

The AWS services I used in this project were Amazon Bedrock, S3, and OpenSearch Serverless. Key concepts include storing data in S3, adding source URLs through Web Crawler, creating a Knowledge Base, requesting access to AI models, how chatbot generates responses using AI models and Knowledge Base, and utilizing vector stores for efficient retrieval.

## Objectives

**I. Use Case 1** – Personalized Q&A Chatbot for thesis



**II. Use Case 2** – Financial News Updates



## Workflow

1. **Add Data Source**
   - **Use Case 1**
     - **Store Data in S3** - Stored relevant documentation in **Amazon S3** as the chatbot's data source.
   - **Use Case 2**
     - **Add Source URLs** - Instead of S3, added source URLs as the data source through **Web Crawler**.
2. **Create a Knowledge Base** - Created a Knowledge Base in **Amazon Bedrock** to enable retrieval-based AI responses.
3. **Request Access to AI Models** - Selected and requested access to specific AI models, enabling the AI models to convert search results into human-like text.
4. **Configure Vector Store** - Used **OpenSearch Serverless** for vector-based search, allowing efficient retrieval of relevant information.
5. **Sync Knowledge Base** - Synchronized the data from **S3** to the **Knowledge Base** to ensure the following three keys:
   - **Ingesting**: Bedrock takes the data from S3.
   - **Processing**: Bedrock chunks and embeds the data.
   - **Storing**: Bedrock stores the processed data in the vector store (OpenSearch Serverless).

By following these flows, the AI chatbot is transformed into the **RAG chatbot**, significantly improving its ability to generate informed responses.

## Document


## Demo

**I. Use Case 1** – Personalized Q&A Chatbot

<table>
   <tr>
      <!-- Left Side -->
<!--       <td style="vertical-align: top; width: 50%;">
         <img src="https://github.com/user-attachments/assets/d93f0aa7-f96c-44b5-b744-cdaae4ee0f1e" width="100%" />
         <img src="https://github.com/user-attachments/assets/d4971f5b-3d81-4f96-b3eb-a7b11df66e94" width="100%" />
      </td>
      <!-- Right Side -->
<!--       <td style="vertical-align: top; width: 50%;">
         <img src="https://github.com/user-attachments/assets/0caef54c-5e57-407a-b311-90f9f2980793" width="100%" />
         <img src="https://github.com/user-attachments/assets/bfaecd97-1d23-4181-aea3-0a2b45dc9f54" width="100%" />
      </td> -->
   </tr> 
</table>

**II. Use Case 2** – Automated Immigration Updates



