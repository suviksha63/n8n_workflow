# AI Content Creator Agent using n8n

## Objective
To build a no-code AI-powered content creation workflow using n8n that automates research and content generation for multiple platforms.

## Tools Used
- n8n workflow automation
- Tavily Search API (for real-time research)
- Google Gemini AI (for content generation)
- Google Sheets (for input and output storage)

## Workflow Process
1. Google Sheets stores content topics with status "Pending".
2. n8n reads topics from the sheet.
3. Tavily API fetches real-time research for the topic.
4. Gemini AI generates:
   - LinkedIn post
   - X (Twitter) post
   - Blog summary
5. Generated content is automatically written back to Google Sheets and the status is updated to "Completed".

## Sample Input
Topic: AI in Healthcare

## Sample Output
LinkedIn Post: AI is transforming healthcare by enabling predictive diagnostics and personalized treatment...

Tweet: AI is revolutionizing healthcare with smarter diagnostics and automation. #AI #HealthTech

Blog Summary: Artificial Intelligence is rapidly transforming healthcare by improving diagnostic accuracy, optimizing treatment plans, and enhancing patient outcomes.

## Prompt Design
The prompt instructs Gemini AI to generate platform-specific content including:
- Professional LinkedIn post
- Short tweet for X
- Informative blog summary
