# 🚀 Parasite SEO AI Agent (Browser Automation)

![TaskAGI Compatible](https://img.shields.io/badge/TaskAGI-Compatible-blue)
![Browser Automation](https://img.shields.io/badge/Browser-Automation-green)
![No API Required](https://img.shields.io/badge/No%20API-Required-orange)
![AI Powered](https://img.shields.io/badge/AI-Claude%20Sonnet%204.5-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)

**The first parasite SEO automation agent that works with ANY website - no API required.**

Automate your parasite SEO strategy across Medium, Dev.to, LinkedIn, Reddit, RapidAPI, WordPress, and any platform using AI-powered browser automation. Post hundreds of SEO-optimized articles to high-authority domains without writing a single line of code.

![Parasite SEO Browser Automation Workflow](https://taskagi.net/storage/images/agents/github-parasite-seo-ai-agent.png)

---

## Overview

The **Parasite SEO AI Agent** revolutionizes automated content distribution by leveraging browser automation instead of platform APIs. While traditional SEO automation is limited to platforms that offer public APIs, this agent can post content to literally any website that accepts user-generated content through a web form.

This breakthrough approach means you can now automate parasite SEO campaigns on platforms like Medium, Dev.to, LinkedIn Articles, Reddit, Hashnode, and countless others - even if they don't have public APIs or charge premium prices for API access.

**How it works:** The agent reads keywords from your Google Sheets tracking spreadsheet, uses Claude AI to generate perfectly optimized ~300-word articles, then uses browser automation to log into your target platform and post the content exactly as a human would. It verifies successful publishing, updates your tracking sheet, and moves on to the next keyword - all while you sleep.

**Deploy this agent with TaskAGI's 1-click deployment feature** and start building high-quality backlinks on authority domains within minutes. No coding required, no API limitations, unlimited platform compatibility.

👉 **[Deploy on TaskAGI.net](https://taskagi.net/agents/parasite-seo-ai-agent-deployed)**

---

## Why Browser Automation Changes Everything

### Traditional API-Based Limitations

Most parasite SEO tools are severely limited:
- ❌ Only work with platforms that have public APIs
- ❌ Require expensive API access fees
- ❌ Subject to API rate limits and restrictions
- ❌ Break when platforms change their API
- ❌ Limited to 5-10 supported platforms maximum

### Browser Automation Advantages

This agent breaks free from those constraints:
- ✅ Works with **ANY** website (500+ potential platforms)
- ✅ No API costs - just your existing account logins
- ✅ Posts content like a real human user
- ✅ Bypasses API rate limits entirely
- ✅ Adapts to any platform in minutes by updating CSS selectors

**Result:** You can build backlinks on hundreds of high-authority domains that competitors can't access through traditional automation tools.

---

## Features

### Core Capabilities

- **Universal Platform Compatibility**: Post to any website with a content submission form - Medium, Dev.to, LinkedIn Articles, Reddit, WordPress, Ghost, Hashnode, Quora, and 500+ more platforms
- **AI-Powered Content Generation**: Claude Sonnet 4.5 creates natural, SEO-optimized 300-word articles tailored to each keyword with engaging titles and relevant content
- **Intelligent Keyword Management**: Reads target keywords from Google Sheets, processes only "DRAFT" status entries, automatically updates to "PUBLISHED" after successful posting
- **Batch Processing**: Process up to 1,000 keywords in a single workflow execution with automatic iteration through your keyword list
- **Human-Like Posting Behavior**: Browser automation includes realistic wait times, natural mouse movements, and form interactions that mimic human users
- **Verification & Error Handling**: Confirms successful publishing before marking keywords as complete, stops workflow if posting fails to prevent data corruption
- **Session Management**: Maintains browser sessions across multiple posts for efficient batch processing without repeated logins
- **Pre-Configured Templates**: Ready-to-use setup for RapidAPI with easy customization guides for 20+ popular platforms

### Technical Specifications

- **Browser Engine**: Chromium-based automation with anti-detection features
- **AI Model**: Anthropic Claude Sonnet 4.5 (configurable)
- **Content Length**: 300 words optimized for engagement and SEO
- **Processing Speed**: 2-3 minutes per article including AI generation and posting
- **Concurrency**: Single-threaded to prevent platform rate limiting
- **Storage**: Google Sheets for keyword tracking and status management

---

## Prerequisites

### Required TaskAGI Account

- **Account Type**: Personal Plan or higher (Free plan supports limited executions)
- **AI Credits**: Approximately 50 credits per article (for Claude AI generation)
- **Get Started**: [Sign up for TaskAGI](https://taskagi.net/register)

### Required Integrations

You'll need to configure these integrations in your TaskAGI account:

1. **Google Sheets Integration**
   - Used for: Keyword tracking and status management
   - Setup: Connect via TaskAGI integrations page
   - Cost: Free (no additional credits)

2. **Anthropic Integration**
   - Used for: AI content generation with Claude Sonnet 4.5
   - Setup: Add API key from [Anthropic Console](https://console.anthropic.com/)
   - Cost: ~50 AI credits per article generated

3. **Browser Automation Integration**
   - Used for: Automated posting to target platforms
   - Setup: Built-in to TaskAGI (no additional setup)
   - Cost: ~20 AI credits per posting session
   - Note: Uses browser-use framework with OpenAI GPT-4o

### Platform Accounts

- Active account on your target platform(s) with posting privileges
- Login credentials ready for browser automation setup
- Verified email if required by the platform
- Understanding of platform posting guidelines to avoid spam flags

### Google Sheets Template

Your tracking spreadsheet must include these columns:
- **Keyword**: Your target SEO keyword/phrase
- **Status**: Either "DRAFT" (ready to post) or "PUBLISHED" (already posted)
- **Additional columns**: Optional (URL, date posted, traffic data, etc.)

---

## Quick Start

### Step 1: Access the Agent on TaskAGI

1. Visit the agent landing page: **[Parasite SEO AI Agent](https://taskagi.net/agents/parasite-seo-ai-agent-deployed)**
2. Log in to your TaskAGI account (or create one if you don't have an account)
3. Review the agent overview and workflow diagram

### Step 2: One-Click Deployment

1. Click the **"Deploy This Agent"** button on the landing page
2. TaskAGI will automatically:
   - Import the complete workflow configuration
   - Create a new agent instance in your account
   - Set up all 12 workflow nodes with default settings
   - Configure node connections and data flow
3. You'll be redirected to your new agent's configuration page

### Step 3: Basic Configuration

Configure these essential settings before your first run:

**Google Sheets Node (Node 1):**
- Paste your Google Sheets URL containing keywords
- Ensure sheet has "Keyword" and "Status" columns
- Mark initial keywords as "DRAFT" status

**Browser Automation Nodes (Nodes 4, 6, 8):**
- Node 4: Update login URL and credentials for your target platform
- Node 6: Verify content editor CSS selector matches your platform
- Node 8: Update publish button selector if different from default

**Test Configuration:**
1. Start with just 2-3 "DRAFT" keywords for testing
2. Click "Run Agent" to execute a test run
3. Monitor execution in real-time on the TaskAGI dashboard
4. Verify articles posted successfully on target platform
5. Confirm Google Sheets updated to "PUBLISHED" status

### Expected Outcome

After successful setup:
- Agent processes all "DRAFT" keywords from your spreadsheet
- Claude AI generates unique, SEO-optimized content for each keyword
- Browser automation posts articles to your target platform automatically
- Google Sheets updates with "PUBLISHED" status for completed keywords
- You can schedule the agent to run daily/weekly for continuous posting

---

## Detailed Setup Guide

### Google Sheets Integration Setup

**Step 1: Create Your Tracking Spreadsheet**

1. Create a new Google Sheet or copy this structure:

```
| Keyword                          | Status    | URL Posted  | Date Posted |
|----------------------------------|-----------|-------------|-------------|
| how to build rest api            | DRAFT     |             |             |
| python web scraping tutorial     | DRAFT     |             |             |
| best seo practices 2025          | DRAFT     |             |             |
```

2. Column requirements:
   - **Keyword** (Column A): Your target keyword or topic
   - **Status** (Column B): Must be either "DRAFT" or "PUBLISHED"
   - Additional columns are optional but recommended for tracking

**Step 2: Configure Google Sheets Access**

1. In TaskAGI dashboard, go to Integrations → Google Sheets
2. Click "Connect Google Account"
3. Authorize TaskAGI to access your Google Sheets
4. Copy your spreadsheet URL
5. Paste URL into Node 1 configuration in your agent workflow

**Step 3: Test Sheet Access**

1. Run Node 1 independently to verify connection
2. Check that TaskAGI can read your keyword data
3. Verify "DRAFT" status keywords are detected correctly

---

### Anthropic (Claude AI) Integration Setup

**Step 1: Get Anthropic API Key**

1. Visit [Anthropic Console](https://console.anthropic.com/)
2. Sign up or log in to your account
3. Navigate to API Keys section
4. Create a new API key with appropriate permissions
5. Copy the API key (starts with "sk-ant-")

**Step 2: Configure in TaskAGI**

1. Go to TaskAGI dashboard → Integrations → Anthropic
2. Paste your API key
3. Test connection to verify it works
4. Set default model to "claude-sonnet-4.5" for best results

**Step 3: Customize Content Generation Prompt**

The default prompt in Node 3 generates SEO-optimized content. You can customize it:

```
Generate a natural, engaging 300-word article about: {{nodes.2.current_keyword}}

Requirements:
- Create an attention-grabbing title (60 characters max)
- Write in conversational, human tone
- Include keyword naturally 3-4 times
- Add 2-3 subheadings for readability
- Focus on providing genuine value to readers
- End with actionable takeaway
- Optimize for SEO but prioritize readability

Format output as:
Title: [Your Title Here]

[Article content with subheadings...]
```

**Cost Estimation:**
- ~50 AI credits per article
- 100 articles = ~5,000 credits
- Personal Plan includes 10,000 credits/month

---

### Browser Automation Integration Setup

**Step 1: Configure Browser Automation Integration**

1. In TaskAGI dashboard, go to Integrations → Browser Automation
2. No API key needed - this integration uses built-in capabilities
3. The integration uses browser-use framework with OpenAI GPT-4o

**Step 2: Configure Login Node (Node 4)**

This is the most critical configuration step. Default settings are for RapidAPI:

```
URL: https://rapidapi.com/hub/tutorials
Task: Click "Sign In", enter email: your-email@example.com, enter password: your-password, click login button
```

**Platform-Specific Login Examples:**

**Medium:**
```
URL: https://medium.com/new-story
Task: Click "Sign in", click "Sign in with email", enter email: your-email@example.com, click continue, enter password: your-password, click sign in
```

**Dev.to:**
```
URL: https://dev.to/new
Task: Click "Log in", enter email: your-email@example.com, enter password: your-password, click "Continue"
```

**LinkedIn Articles:**
```
URL: https://www.linkedin.com/pulse/new/
Task: Enter email: your-email@example.com, click next, enter password: your-password, click sign in
```

**Step 3: Configure Content Pasting Node (Node 6)**

Update the task to match your platform's editor:

**Default (RapidAPI):**
```
Task: Find the main content editor textarea and paste: {{nodes.3.article_content}}
```

**Medium:**
```
Task: Click into the article title field, paste title, press tab, paste content: {{nodes.3.article_content}}
```

**Dev.to:**
```
Task: Click the markdown editor, paste: {{nodes.3.article_content}}
```

**Step 4: Configure Publish Node (Node 8)**

Update to match your platform's publish button:

**Default (RapidAPI):**
```
Task: Click the "Save" or "Publish" button to post the article
```

**Medium:**
```
Task: Click "Ready to publish?", then click "Publish now"
```

**Dev.to:**
```
Task: Click "Publish" button at bottom of editor
```

**Step 5: Test Browser Automation**

1. Run a single test execution with one keyword
2. Watch browser automation in action (visible in TaskAGI dashboard)
3. Verify it can log in successfully
4. Check that content pastes correctly
5. Confirm article publishes successfully

---

### Platform-Specific Configuration Examples

#### Medium Configuration

**Node 4 (Login):**
- URL: `https://medium.com/new-story`
- Task: `Click "Sign in", click "Sign in with email", enter email: YOUR_EMAIL, click continue, enter password: YOUR_PASSWORD, click sign in, wait for editor to load`

**Node 6 (Paste Content):**
- Task: `Click the title placeholder "Title", paste "{{nodes.3.title}}", press Tab key, paste article content: {{nodes.3.article_content}}`

**Node 8 (Publish):**
- Task: `Click "Ready to publish?" button, then click "Publish now" button`

**Node 9 (Verification):**
- Condition: `Check if URL contains "/p/" which indicates successful publication`

---

#### Dev.to Configuration

**Node 4 (Login):**
- URL: `https://dev.to/new`
- Task: `Click "Log in" link, enter email: YOUR_EMAIL, enter password: YOUR_PASSWORD, click "Continue" button`

**Node 6 (Paste Content):**
- Task: `Click into the markdown editor (large textarea), paste title with # prefix: # {{nodes.3.title}}, press enter twice, paste content: {{nodes.3.article_content}}`

**Node 8 (Publish):**
- Task: `Scroll to bottom, click "Publish" button (blue button at bottom right)`

**Node 9 (Verification):**
- Condition: `Check if page shows "Your post has been published" confirmation message`

---

#### LinkedIn Articles Configuration

**Node 4 (Login):**
- URL: `https://www.linkedin.com/pulse/new/`
- Task: `Enter email: YOUR_EMAIL, click Next, enter password: YOUR_PASSWORD, click Sign in, wait for article editor`

**Node 6 (Paste Content):**
- Task: `Click "Headline" field, paste: {{nodes.3.title}}, click into article content editor, paste: {{nodes.3.article_content}}`

**Node 8 (Publish):**
- Task: `Click "Next" button at top right, click "Publish" button on confirmation screen`

**Node 9 (Verification):**
- Condition: `Check if URL changes to /posts/ which indicates published article`

---

#### Reddit Configuration

**Node 4 (Login):**
- URL: `https://www.reddit.com/r/YOUR_SUBREDDIT/submit`
- Task: `Click "Log In", enter username: YOUR_USERNAME, enter password: YOUR_PASSWORD, click Log In button`

**Node 6 (Paste Content):**
- Task: `Click "Title" field, paste: {{nodes.3.title}}, click "Text" tab, click into text editor, paste: {{nodes.3.article_content}}`

**Node 8 (Publish):**
- Task: `Click blue "Post" button at bottom right`

**Node 9 (Verification):**
- Condition: `Check if URL contains /comments/ which indicates successful post creation`

---

## Usage Examples

### Example 1: Batch Publishing to Medium

**Scenario:** You have 50 software development keywords and want to build authority on Medium.

**Setup:**
1. Create Google Sheet with 50 keywords marked as "DRAFT"
2. Configure browser automation for Medium (see platform examples above)
3. Customize AI prompt to match Medium's style (more narrative, storytelling approach)
4. Set loop to maximum 50 iterations

**Execution:**
```
Workflow processes:
- Keyword 1: "how to build rest api" → AI generates article → Posts to Medium → Marks PUBLISHED
- Keyword 2: "python web scraping guide" → AI generates article → Posts to Medium → Marks PUBLISHED
- ... continues for all 50 keywords
```

**Result:** 50 high-quality Medium articles published over ~2-3 hours, each optimized for different SEO keywords.

---

### Example 2: Multi-Platform Parasite SEO Campaign

**Scenario:** You want to maximize backlink diversity by posting to 5 different platforms.

**Setup:**
1. Clone the agent 5 times (one for each platform)
2. Configure each clone for different platform:
   - Agent 1: Medium
   - Agent 2: Dev.to
   - Agent 3: LinkedIn Articles
   - Agent 4: Hashnode
   - Agent 5: RapidAPI
3. Use same Google Sheet for all agents
4. Add "Platform" column to sheet to track where each keyword was posted

**Execution:**
- Run Agent 1 (Medium): Processes 10 keywords
- Run Agent 2 (Dev.to): Processes same 10 keywords with different content
- Run Agent 3 (LinkedIn): Processes same 10 keywords with professional angle
- And so on...

**Result:** 50 total articles (10 keywords × 5 platforms) with maximum domain authority diversity.

---

### Example 3: Niche-Specific Reddit Automation

**Scenario:** You manage a SaaS product and want to provide value in 10 relevant subreddits.

**Setup:**
1. Research 10 subreddits where your audience hangs out
2. Create keyword list focused on pain points (not promotional)
3. Customize AI prompt to generate helpful, non-salesy content
4. Configure browser automation for Reddit posting
5. Set different subreddit URL for each batch

**Execution:**
```
r/webdev batch: 5 keywords about web development challenges
r/startups batch: 5 keywords about startup marketing
r/entrepreneur batch: 5 keywords about business automation
... continues for all subreddits
```

**Result:** Genuine value-add content in niche communities, building reputation and organic traffic.

---

### Example 4: Scheduled Daily Publishing

**Scenario:** You want to post 3 new articles every day on autopilot.

**Setup:**
1. Maintain Google Sheet with 100+ "DRAFT" keywords
2. Configure loop limit to 3 iterations (stops after 3 articles)
3. Set up TaskAGI schedule to run daily at 8 AM
4. Monitor Google Sheet to add more keywords as needed

**Execution:**
- Day 1: Posts 3 articles, marks them PUBLISHED
- Day 2: Posts next 3 articles, marks them PUBLISHED
- Day 3: Posts next 3 articles, marks them PUBLISHED
- Continues until all DRAFT keywords exhausted

**Result:** Consistent publishing schedule without manual work, 90 articles per month on autopilot.

---

### Example 5: Content Refresh Strategy

**Scenario:** You want to update old articles with fresh content monthly.

**Setup:**
1. Add "Last Updated" column to Google Sheet
2. Add "Content Version" column to track revisions
3. Configure conditional logic to re-post keywords older than 30 days
4. Update AI prompt to reference previous content for consistency

**Execution:**
- Agent checks "Last Updated" date
- Finds keywords not updated in 30+ days
- Generates fresh version of content
- Posts update to same platform
- Updates "Last Updated" timestamp

**Result:** Evergreen content stays relevant and maintains SEO rankings.

---

## Troubleshooting

### Common Issues and Solutions

#### Workflow Stuck in "Pending" Status

**Problem:** Agent shows "pending" status for extended period.

**Cause:** Queue workers not running on TaskAGI infrastructure.

**Solution:**
- Wait 2-3 minutes (normal processing time)
- If stuck longer than 5 minutes, contact TaskAGI support
- Check TaskAGI status page for any ongoing incidents

---

#### Browser Automation Can't Find Elements

**Problem:** Browser automation fails to click buttons or fill forms.

**Cause:** Platform updated their HTML structure or CSS selectors changed.

**Solution:**
1. Enable "headed mode" in browser automation to watch execution
2. Inspect the page to find current CSS selectors
3. Update Node 4, 6, and 8 with new selectors
4. Use more robust selectors:
   - Bad: `.btn-123` (class names change frequently)
   - Good: `button[aria-label="Publish"]` (semantic attributes more stable)
5. Add longer wait times if elements load slowly

---

#### Google Sheets "PUBLISHED" Status Not Updating

**Problem:** Articles post successfully but sheet still shows "DRAFT".

**Cause:** Node 11 (update status) configuration incorrect or permissions issue.

**Solution:**
1. Verify Google Sheets integration has write permissions
2. Check Node 10 successfully finds the correct row
3. Confirm Node 11 receives correct row reference from Node 10
4. Test Node 11 independently to isolate the issue
5. Ensure "Status" column name exactly matches in sheet (case-sensitive)

---

#### AI-Generated Content Quality Issues

**Problem:** Claude generates low-quality, generic, or off-topic content.

**Cause:** Prompt needs refinement or keyword too vague.

**Solution:**
1. Improve keyword specificity in Google Sheet
   - Bad: "marketing"
   - Good: "email marketing automation for ecommerce"
2. Enhance AI prompt in Node 3:
   - Add more context about target audience
   - Specify tone and style requirements
   - Include example article structure
3. Increase temperature for more creativity (if too robotic)
4. Decrease temperature for more consistency (if too random)

---

#### Platform Flags Content as Spam

**Problem:** Posted articles get removed or account flagged for spam.

**Cause:** Posting too frequently or content appears automated.

**Solution:**
1. **Reduce posting frequency:**
   - Limit loop to 3-5 articles per execution
   - Schedule runs every 12-24 hours instead of continuous
2. **Improve content uniqueness:**
   - Increase AI temperature to 0.8-0.9
   - Add randomization to article structure
   - Include platform-specific formatting
3. **Add human touches:**
   - Include personal anecdotes in prompt
   - Vary article length (200-400 words instead of fixed 300)
   - Use different content templates for different keywords
4. **Follow platform guidelines:**
   - Read community rules for each platform
   - Avoid promotional content
   - Focus on genuinely helpful information
   - Engage with other content (manually) to build reputation

---

## Frequently Asked Questions

### What is parasite SEO and why use browser automation?

**Parasite SEO** is the strategy of leveraging high-authority domains (like Medium, Dev.to, LinkedIn) to rank your content in Google search results. These platforms already have strong domain authority (DA 90+), so your content can rank faster than on your own website.

**Browser automation** is the game-changer because most high-DA platforms either don't have public APIs or severely restrict API access. Traditional automation tools can only work with 5-10 platforms that offer APIs. Browser automation works with ANY website that accepts content through web forms - opening up 500+ potential platforms for your parasite SEO strategy.

---

### Which platforms work best with this agent?

**Recommended High-DA Platforms (No API Required):**
- **Medium** (DA 96): Best for long-form thought leadership content
- **Dev.to** (DA 87): Ideal for technical tutorials and developer content
- **LinkedIn Articles** (DA 99): Perfect for B2B and professional insights
- **Reddit** (DA 91): Great for niche communities (focus on value, not promotion)
- **Hashnode** (DA 82): Growing platform for developer content
- **RapidAPI Blog** (DA 75): Pre-configured default in this agent

**Also Compatible (Require Minor Configuration Changes):**
- Quora, Stack Overflow, GitHub Discussions, HackerNoon, Substack, Ghost, WordPress, Wix, Webflow blogs, and hundreds more

---

### How do I avoid getting flagged as spam?

**Follow these best practices:**

1. **Post valuable content only:**
   - Focus on genuinely helpful information
   - Answer real questions your audience has
   - Avoid promotional language or sales pitches

2. **Respect posting frequency:**
   - Don't post more than 5 articles per day per platform
   - Space out executions by 12-24 hours
   - Some platforms (like Reddit) require even slower posting

3. **Vary your content:**
   - Use different article structures
   - Adjust AI temperature for uniqueness
   - Don't repeat the same keyword variations

4. **Build account reputation first:**
   - Manually engage with other content on the platform
   - Get some activity on your profile before automation
   - Add a complete bio and profile picture

5. **Follow platform guidelines:**
   - Read community rules and content policies
   - Stay within topic guidelines for each platform
   - Use appropriate tags and categories

---

### How much does it cost to run this agent?

**AI Credit Costs (per article):**
- Claude AI content generation: ~50 credits
- Browser automation posting: ~20 credits
- **Total per article: ~70 credits**

**Monthly Cost Examples:**

**100 Articles Per Month:**
- Credits needed: 7,000
- Personal Plan ($29/month): Includes 10,000 credits ✅
- Additional cost: $0 (within included credits)

**500 Articles Per Month:**
- Credits needed: 35,000
- Personal Plan base: 10,000 credits
- Additional credits needed: 25,000 credits (~$25)
- **Total monthly cost: $29 + $25 = $54**

**1,000 Articles Per Month:**
- Credits needed: 70,000
- Enterprise Plan ($99/month): Includes 100,000 credits ✅
- Additional cost: $0 (within included credits)

---

### Can I customize the AI-generated content style?

**Absolutely!** Node 3 (Claude AI) is fully customizable. You can modify:

**Content Length:**
```
Generate a [100/300/500/1000]-word article about: {{nodes.2.current_keyword}}
```

**Writing Tone:**
```
Tone options:
- Professional and authoritative (for B2B platforms)
- Casual and conversational (for Reddit, Dev.to)
- Academic and research-backed (for thought leadership)
- Friendly and approachable (for beginner tutorials)
```

**Article Structure:**
```
Format requirements:
- Start with a provocative question
- Include 3 specific examples
- Add bullet points for key takeaways
- End with a call-to-action
- Use storytelling format with personal anecdotes
```

---

## License

MIT License

Copyright (c) 2025 TaskAGI

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
