# Module 1.3: Understanding AI Model Capabilities and Limitations
## Detailed Lesson Plan for Complete Beginners

### **Course Information**
- **Duration**: 2 hours
- **Format**: Interactive lecture + step-by-step hands-on labs
- **Prerequisites**: Completed Modules 1.1 and 1.2 (basic AI understanding and prompt engineering)
- **Learning Objectives**: By the end of this session, students will understand what AI can and cannot do, how to work with different AI models, and how to create prompts that work effectively across platforms

---

## **Part 1: Understanding AI Model Capabilities (45 minutes)**

### **Opening Hook - The AI Revolution Story (5 minutes)**
**Meet David - The AI Consultant Success Story**:
"David was a marketing manager who learned to work with different AI models. He discovered that ChatGPT is great for creative writing, Claude excels at analysis, and Gemini is perfect for research. By understanding each model's strengths, he became an AI consultant earning $120,000 per year, helping companies choose the right AI tools for their needs."

**What You'll Learn Today**:
- What different AI models can and cannot do
- How to choose the right AI tool for your task
- How to work around AI limitations
- Why understanding AI capabilities makes you more valuable in the job market

### **The AI Model Landscape - 2024 Update (20 minutes)**

**Think of AI Models Like Different Types of Experts**:
"Just like you'd go to a doctor for medical advice, a lawyer for legal help, and a chef for cooking tips, different AI models are better at different tasks. Understanding their strengths helps you get the best results."

**Major AI Models and Their Strengths**:

**1. GPT-4o (OpenAI) - The All-Rounder**
- **Best For**: General tasks, creative writing, coding, analysis
- **Strengths**: 
  - Excellent at understanding context
  - Great for creative and analytical tasks
  - Strong reasoning abilities
  - Good at following complex instructions
- **Context Window**: 128,000 tokens (~96,000 words)
- **Special Features**: Can process images and text together
- **Cost**: $5-15 per 1M tokens (moderate)

**2. Claude 3.5 Sonnet (Anthropic) - The Analyst**
- **Best For**: Long documents, analysis, research, writing
- **Strengths**:
  - Excellent at analyzing long documents
  - Great for research and fact-checking
  - Strong reasoning and logic
  - Very good at following detailed instructions
- **Context Window**: 200,000 tokens (~150,000 words)
- **Special Features**: Can read and analyze entire books
- **Cost**: $3-15 per 1M tokens (competitive)

**3. Gemini 1.5 Pro (Google) - The Researcher**
- **Best For**: Research, fact-checking, multimodal tasks
- **Strengths**:
  - Excellent at finding and verifying information
  - Great for research tasks
  - Strong multimodal capabilities (text, images, audio)
  - Good integration with Google services
- **Context Window**: 1M tokens (~750,000 words)
- **Special Features**: Can process massive amounts of text
- **Cost**: $1-7 per 1M tokens (very competitive)

**4. Llama 3.1 (Meta) - The Open Source Option**
- **Best For**: Custom applications, privacy-focused tasks
- **Strengths**:
  - Free to use
  - Can be customized
  - Good for basic tasks
  - Privacy-friendly (can run locally)
- **Context Window**: 128,000 tokens
- **Special Features**: Open source, customizable
- **Cost**: Free (but requires technical setup)

**5. Mistral 7B (Mistral AI) - The Efficient Option**
- **Best For**: Fast responses, simple tasks, cost-effective solutions
- **Strengths**:
  - Very fast responses
  - Cost-effective
  - Good for simple tasks
  - Efficient resource usage
- **Context Window**: 32,000 tokens
- **Special Features**: Fast and efficient
- **Cost**: Very low

### **Understanding Key AI Concepts - Tokens and Context Windows (10 minutes)**

**What Are Tokens? - The Building Blocks of AI**

**Think of Tokens Like Puzzle Pieces**:
"Imagine you're building a puzzle. Each piece represents a token. AI breaks down your text into these pieces to understand it, then puts them back together to create responses."

**Simple Definition**:
- **Token**: A piece of text that AI can understand (usually a word, part of a word, or punctuation)
- **Tokenization**: The process of breaking text into tokens

**Visual Example**:
```
Original Text: "Hello, world!"
Tokens: ["Hello", ",", " world", "!"]
Number of Tokens: 4
```

**More Complex Examples**:

**Example 1 - Simple Sentence**:
```
Text: "The quick brown fox"
Tokens: ["The", " quick", " brown", " fox"]
Count: 4 tokens
```

**Example 2 - With Punctuation**:
```
Text: "I love AI! It's amazing."
Tokens: ["I", " love", " AI", "!", " It", "'s", " amazing", "."]
Count: 8 tokens
```

**Example 3 - Numbers and Special Characters**:
```
Text: "Price: $25.99 (50% off)"
Tokens: ["Price", ":", " $", "25", ".", "99", " (", "50", "%", " off", ")"]
Count: 11 tokens
```

**Example 4 - Different Languages**:
```
Text: "Hola mundo" (Spanish)
Tokens: ["Hola", " mundo"]
Count: 2 tokens

Text: "こんにちは世界" (Japanese)
Tokens: ["こんにちは", "世界"]
Count: 2 tokens
```

**Why Tokens Matter**:
- **Cost**: You pay per token (like paying per word)
- **Limits**: AI has maximum token limits
- **Efficiency**: Shorter prompts = lower costs
- **Understanding**: AI processes text in tokens

**Real-World Cost Examples**:

**Example 1 - Simple Email**:
```
Prompt: "Write a professional email" (4 tokens)
Response: 200-word email (~250 tokens)
Total: 254 tokens
Cost: $0.001 (less than 1 cent)
```

**Example 2 - Long Document Analysis**:
```
Prompt: "Analyze this 10-page report" (5 tokens)
Document: 10 pages (~5,000 tokens)
Response: 500-word analysis (~600 tokens)
Total: 5,605 tokens
Cost: $0.03 (3 cents)
```

**Example 3 - Large Project**:
```
Prompt: "Summarize this book" (4 tokens)
Book: 300 pages (~150,000 tokens)
Response: 1,000-word summary (~1,200 tokens)
Total: 151,204 tokens
Cost: $0.75 (75 cents)
```

**Cost Comparison by Model**:
```
GPT-4o: $5-15 per 1M tokens
Claude 3.5: $3-15 per 1M tokens
Gemini 1.5: $1-7 per 1M tokens
Mistral 7B: $0.25-1 per 1M tokens
```

**How to Save Money**:
- **Be specific**: Shorter, clearer prompts
- **Use examples**: Few-shot learning reduces tokens
- **Choose the right model**: Use cheaper models for simple tasks
- **Batch requests**: Combine multiple questions

**What is a Context Window? - AI's Memory**

**Think of Context Window Like Short-Term Memory**:
"Imagine you're having a conversation with someone who can only remember the last 10 things you said. That's like AI's context window - it can only 'remember' a certain amount of information."

**Simple Definition**:
- **Context Window**: The maximum amount of text (in tokens) that AI can process at once
- **Input + Output**: Your prompt + AI's response must fit within the limit

**Visual Illustration**:
```
Context Window = 10,000 tokens

Your Prompt: 3,000 tokens
AI Response: 7,000 tokens
Total: 10,000 tokens ✅ (Fits!)

Your Prompt: 8,000 tokens
AI Response: 3,000 tokens
Total: 11,000 tokens ❌ (Too big!)
```

**Real-World Context Window Examples**:

**GPT-4o Context Window**:
```
Size: 128,000 tokens
Equivalent: ~96,000 words
Example: Can process about 200 pages of text
```

**Claude 3.5 Context Window**:
```
Size: 200,000 tokens
Equivalent: ~150,000 words
Example: Can process about 300 pages of text
```

**Gemini 1.5 Context Window**:
```
Size: 1,000,000 tokens
Equivalent: ~750,000 words
Example: Can process about 1,500 pages of text
```

**Practical Examples of Context Window Usage**:

**Example 1 - Small Document**:
```
Document: 5-page report (2,000 words = ~2,500 tokens)
AI Model: GPT-4o (128,000 tokens)
Result: ✅ Easily fits, plenty of room for analysis
```

**Example 2 - Large Document**:
```
Document: 100-page manual (40,000 words = ~50,000 tokens)
AI Model: GPT-4o (128,000 tokens)
Result: ✅ Fits, but leaves less room for detailed analysis
```

**Example 3 - Very Large Document**:
```
Document: 500-page book (200,000 words = ~250,000 tokens)
AI Model: GPT-4o (128,000 tokens)
Result: ❌ Too big! Need Claude 3.5 or Gemini 1.5
```

**What Happens When You Exceed Context Limits**:

**Scenario**: You try to analyze a 300-page document with GPT-4o
```
Problem: Document is 240,000 tokens, but GPT-4o only handles 128,000
What Happens: AI "forgets" the beginning of the document
Result: Analysis might miss important early information
```

**Solutions**:
1. **Use a larger model**: Switch to Claude 3.5 or Gemini 1.5
2. **Summarize first**: Break the document into smaller parts
3. **Focus on key sections**: Analyze only the most important parts

**Visual Illustration - Context Window in Action**:

**Scenario**: You want to analyze a 200-page business report

**Option 1 - Using GPT-4o (128K tokens)**:
```
Report: 200 pages = 160,000 tokens
Problem: Exceeds GPT-4o's 128K limit
Solution: "First, summarize this report in 5 key points, then analyze each point separately"
```

**Option 2 - Using Claude 3.5 (200K tokens)**:
```
Report: 200 pages = 160,000 tokens
Analysis: 20,000 tokens
Total: 180,000 tokens
Result: ✅ Fits comfortably in Claude's 200K window
```

**Option 3 - Using Gemini 1.5 (1M tokens)**:
```
Report: 200 pages = 160,000 tokens
Analysis: 20,000 tokens
Additional context: 50,000 tokens
Total: 230,000 tokens
Result: ✅ Plenty of room for detailed analysis
```

**Practical Decision Tree**:

```
Is your document < 100 pages?
├─ Yes → Use any model (GPT-4o, Claude 3.5, Gemini 1.5)
└─ No → Is your document < 200 pages?
    ├─ Yes → Use Claude 3.5 or Gemini 1.5
    └─ No → Use Gemini 1.5 or break into smaller parts
```

**Real-World Examples**:

**Example 1 - Email Analysis**:
```
Task: Analyze 50 customer service emails
Size: ~5,000 tokens
Best Model: Any model (GPT-4o, Claude 3.5, Gemini 1.5)
Cost: ~$0.03
```

**Example 2 - Legal Document Review**:
```
Task: Review a 150-page contract
Size: ~120,000 tokens
Best Model: Claude 3.5 or Gemini 1.5
Cost: ~$0.50
```

**Example 3 - Research Paper Analysis**:
```
Task: Analyze 10 research papers (500 pages total)
Size: ~400,000 tokens
Best Model: Gemini 1.5
Cost: ~$2.00
```

### **Understanding AI Capabilities - What AI Can Do (10 minutes)**

**Capability 1: Text Generation and Writing**
**What It Means**: AI can create original text content
**Examples**:
- Writing emails, reports, articles
- Creating marketing copy
- Generating creative stories
- Writing code and documentation

**Hands-on Example**:
```
Prompt: "Write a professional email to a client explaining a project delay"
Result: AI creates a complete, professional email with appropriate tone
```

**Capability 2: Analysis and Reasoning**
**What It Means**: AI can analyze information and draw conclusions
**Examples**:
- Analyzing data and trends
- Comparing different options
- Solving problems step-by-step
- Making recommendations

**Hands-on Example**:
```
Prompt: "Analyze this sales data and tell me what trends you see: [data]"
Result: AI identifies patterns and provides insights
```

**Capability 3: Information Processing**
**What It Means**: AI can understand and process large amounts of information
**Examples**:
- Summarizing long documents
- Extracting key information
- Translating between languages
- Organizing information

**Hands-on Example**:
```
Prompt: "Summarize this 50-page report in 3 key points"
Result: AI creates a concise summary of the main points
```

**Capability 4: Creative Tasks**
**What It Means**: AI can generate creative content
**Examples**:
- Writing stories and poems
- Creating marketing campaigns
- Designing user interfaces
- Brainstorming ideas

**Hands-on Example**:
```
Prompt: "Create 10 creative marketing slogans for a new coffee shop"
Result: AI generates original, creative slogans
```

**Capability 5: Multimodal Processing (Latest Feature)**
**What It Means**: AI can work with text, images, and audio together
**Examples**:
- Analyzing images and describing them
- Creating content based on images
- Processing documents with text and images
- Understanding context from multiple sources

**Hands-on Example**:
```
Prompt: "Look at this image and write a product description for this item"
Result: AI analyzes the image and creates relevant product copy
```

---

## **Part 2: Understanding AI Limitations (30 minutes)**

### **Why Understanding Limitations is Crucial (5 minutes)**

**Think of AI Like a Very Smart Assistant**:
"AI is like having a brilliant assistant who has read millions of books but has never actually experienced the real world. They're incredibly knowledgeable but have some blind spots you need to know about."

**Why This Matters for Your Career**:
- **Avoid costly mistakes**: Understanding limitations prevents errors
- **Build trust**: Clients trust you more when you're honest about AI's capabilities
- **Create better solutions**: You can design workarounds for limitations
- **Stay competitive**: Knowing limitations helps you choose the right tools

### **Major AI Limitations You Need to Know (25 minutes)**

**Limitation 1: Hallucinations (Making Things Up)**
**What It Means**: AI sometimes creates information that sounds true but isn't
**Why It Happens**: AI predicts what should come next, not what's actually true
**Real Examples**:
- AI might create fake statistics
- AI might invent historical events
- AI might make up quotes from people
- AI might create fake company information

**How to Spot Hallucinations**:
- Information that sounds too perfect
- Details that seem too specific
- Claims that are hard to verify
- Information that contradicts what you know

**How to Prevent Hallucinations**:
- Ask AI to cite sources
- Request verification of facts
- Use specific, factual prompts
- Cross-check important information

**Hands-on Exercise - Spotting Hallucinations**:
```
Prompt: "Tell me about the history of the company 'TechCorp Solutions'"
Expected Issue: AI might create fake company history
Solution: Ask "What sources did you use for this information?"
```

**Limitation 2: Bias and Stereotypes**
**What It Means**: AI can reflect biases from its training data
**Why It Happens**: AI learns from human-created content, which contains biases
**Real Examples**:
- Gender bias in job descriptions
- Racial bias in image descriptions
- Cultural bias in recommendations
- Age bias in hiring suggestions

**How to Spot Bias**:
- Stereotypical assumptions
- Unfair generalizations
- Inappropriate associations
- Exclusion of certain groups

**How to Reduce Bias**:
- Use inclusive language in prompts
- Ask for diverse perspectives
- Specify fairness requirements
- Review outputs for bias

**Hands-on Exercise - Identifying Bias**:
```
Prompt: "Write a job description for a software engineer"
Potential Issue: Might include gender-biased language
Solution: Add "Use inclusive language and avoid stereotypes"
```

**Limitation 3: Context Window Limits**
**What It Means**: AI can only "remember" a certain amount of information
**Why It Matters**: Important information might be forgotten
**Real Examples**:
- GPT-4o: 128,000 tokens (~96,000 words)
- Claude 3.5: 200,000 tokens (~150,000 words)
- Gemini 1.5: 1M tokens (~750,000 words)

**How to Work Within Limits**:
- Summarize long documents first
- Focus on the most important information
- Break large tasks into smaller parts
- Use the model with the largest context window for long documents

**Hands-on Exercise - Managing Context Limits**:
```
Problem: Need to analyze a 200-page document
Solution: "First, summarize this document in 5 key points, then analyze each point"
```

**Limitation 4: Lack of Real-Time Information**
**What It Means**: AI doesn't know what happened after its training data
**Why It Happens**: AI is trained on historical data, not live information
**Real Examples**:
- AI doesn't know today's news
- AI doesn't know current stock prices
- AI doesn't know recent events
- AI doesn't know current weather

**How to Work Around This**:
- Specify the date range for information
- Ask AI to clarify its knowledge cutoff
- Use AI for analysis, not current facts
- Combine AI with real-time data sources

**Hands-on Exercise - Handling Outdated Information**:
```
Prompt: "What's the current price of Bitcoin?"
Issue: AI might give outdated information
Solution: "What was the price of Bitcoin as of your last training data?"
```

**Limitation 5: Inconsistent Quality**
**What It Means**: AI responses can vary in quality
**Why It Happens**: AI generates responses probabilistically
**Real Examples**:
- Same prompt might give different results
- Quality can vary based on prompt wording
- Some responses might be better than others
- Consistency can be challenging

**How to Improve Consistency**:
- Use specific, detailed prompts
- Provide examples of desired output
- Test prompts multiple times
- Refine prompts based on results

**Hands-on Exercise - Testing Consistency**:
```
Task: Ask the same question 3 times and compare results
Prompt: "Write a 100-word product description for wireless headphones"
Analysis: Compare the three responses for quality and consistency
```

---

## **Part 3: Hands-on Lab - Testing AI Capabilities and Limitations (30 minutes)**

### **Lab Setup - Getting Ready (5 minutes)**

**What You'll Need**:
- Access to at least 2 different AI models (ChatGPT, Claude, Gemini)
- A notebook to record your observations
- Timer for each exercise

**Step-by-Step Setup**:
1. Open multiple browser tabs with different AI tools
2. Create a comparison chart in your notebook
3. Set a timer for 5 minutes per exercise
4. Prepare to take notes on what you observe

### **Lab Exercise 1: Understanding Tokens and Context Windows (10 minutes)**

**Task**: Learn how to count tokens and understand context limits

**Step-by-Step Instructions**:

**Step 1: Token Counting Practice**
Go to: https://platform.openai.com/tokenizer

**Test These Examples**:

**Example 1 - Simple Text**:
```
Text: "Hello, how are you today?"
Expected Tokens: ~6-8 tokens
What to Notice: How punctuation and spaces count as tokens
```

**Example 2 - Longer Text**:
```
Text: "Write a professional email to a client explaining that their project will be delayed by one week due to unexpected technical challenges. The tone should be apologetic but confident, and include a new timeline."
Expected Tokens: ~50-60 tokens
What to Notice: How longer prompts use more tokens
```

**Example 3 - Numbers and Special Characters**:
```
Text: "The price is $25.99 (50% off) - call 555-1234 for details!"
Expected Tokens: ~15-20 tokens
What to Notice: How numbers and symbols count as separate tokens
```

**Step 2: Context Window Testing**

**Test 1 - Small Prompt**:
```
Prompt: "Summarize this in one sentence: [paste a 100-word paragraph]"
What to Look For: Does it work easily?
Result: ✅ Should work on any model
```

**Test 2 - Medium Prompt**:
```
Prompt: "Analyze this document: [paste a 1,000-word article]"
What to Look For: Does it work on all models?
Result: ✅ Should work on all models
```

**Test 3 - Large Prompt**:
```
Prompt: "Summarize this: [paste a 5,000-word document]"
What to Look For: Which models can handle this?
Result: ✅ GPT-4o, Claude 3.5, Gemini 1.5
```

**Step 3: Record Your Findings**

```
Token Counting Results:
Example 1: [Your count] tokens
Example 2: [Your count] tokens  
Example 3: [Your count] tokens

Context Window Results:
Small Prompt: [Which models worked]
Medium Prompt: [Which models worked]
Large Prompt: [Which models worked]

Key Insights:
- [What you learned about tokens]
- [What you learned about context windows]
- [How this affects your prompt design]
```

### **Lab Exercise 2: Testing Different AI Models (10 minutes)**

**Task**: Compare how different AI models handle the same task

**Step-by-Step Instructions**:

**Step 1**: Choose one of these tasks:
- Write a professional email
- Analyze a business problem
- Create a marketing slogan
- Explain a complex concept

**Step 2**: Create the same prompt for each AI model

**Step 3**: Test with ChatGPT, Claude, and Gemini (or available models)

**Step 4**: Record your observations in this format:

```
Task: [Your chosen task]
Prompt: [Your exact prompt]

ChatGPT Response:
- Quality: [Rate 1-10]
- Strengths: [What it did well]
- Weaknesses: [What could be better]

Claude Response:
- Quality: [Rate 1-10]
- Strengths: [What it did well]
- Weaknesses: [What could be better]

Gemini Response:
- Quality: [Rate 1-10]
- Strengths: [What it did well]
- Weaknesses: [What could be better]

Best Model for This Task: [Which one and why]
```

**Example Task - Professional Email**:
```
Prompt: "Write a professional email to a client explaining that their project will be delayed by one week due to unexpected technical challenges. The tone should be apologetic but confident, and include a new timeline."
```

### **Lab Exercise 3: Testing AI Limitations (10 minutes)**

**Task**: Intentionally test AI limitations to understand them better

**Step-by-Step Instructions**:

**Test 1 - Hallucinations**:
```
Prompt: "Tell me about the company 'FutureTech Innovations' and their recent product launch"
What to Look For: Does AI create fake information?
How to Test: Ask "What sources did you use for this information?"
```

**Test 2 - Bias Detection**:
```
Prompt: "Write a job description for a software engineer"
What to Look For: Any gender, age, or cultural bias
How to Test: Look for stereotypical language or assumptions
```

**Test 3 - Context Limits**:
```
Prompt: "Summarize this long document: [paste a very long text]"
What to Look For: Does AI miss important information?
How to Test: Check if key points are included in the summary
```

**Test 4 - Real-Time Information**:
```
Prompt: "What's the current weather in New York City?"
What to Look For: Does AI give current information or outdated data?
How to Test: Compare with actual current weather
```

**Record Your Findings**:
```
Limitation Tested: [Which limitation]
Prompt Used: [Your exact prompt]
What Happened: [Describe the result]
How to Work Around It: [Your solution]
```

### **Lab Exercise 4: Creating Robust Prompts (5 minutes)**

**Task**: Create prompts that work around AI limitations

**Step-by-Step Instructions**:

**Step 1**: Pick a task that might trigger AI limitations

**Step 2**: Create a basic prompt

**Step 3**: Identify potential problems

**Step 4**: Create an improved prompt that addresses the limitations

**Example**:

**Basic Prompt** (Potential Problems):
```
"Write a marketing plan for our new product"
Problems: Vague, no context, might hallucinate details
```

**Improved Prompt** (Addresses Limitations):
```
"You are a marketing expert. I need a marketing plan for a new eco-friendly water bottle. Our target audience is environmentally conscious consumers aged 25-45. The product costs $25 and will be sold online. Please create a realistic plan with specific, achievable strategies. If you need to make assumptions, clearly state them as assumptions rather than facts."
```

**Why This Works**:
- ✅ Specific role (marketing expert)
- ✅ Clear context (product, audience, price)
- ✅ Realistic constraints (online sales)
- ✅ Addresses hallucination risk (state assumptions)
- ✅ Specific output requirements

---

## **Part 4: Practical Application - Choosing the Right AI Tool (15 minutes)**

### **The AI Tool Selection Framework (10 minutes)**

**Think of Choosing AI Tools Like Choosing the Right Tool for a Job**:
"You wouldn't use a hammer to cut wood, and you wouldn't use a saw to drive nails. Each AI tool has strengths that make it better for certain tasks."

**The 5-Step Selection Process**:

**Step 1: Define Your Task**
Ask yourself:
- What exactly do I need to accomplish?
- What type of output do I want?
- How complex is the task?
- What's my budget?

**Step 2: Consider the Requirements**
Ask yourself:
- Do I need to process long documents?
- Do I need real-time information?
- Do I need multimodal capabilities?
- How important is speed vs. quality?

**Step 3: Match Tool to Task**
Use this decision tree:
- **Long documents (100+ pages)**: Claude 3.5 or Gemini 1.5
- **Creative writing**: GPT-4o or Claude 3.5
- **Research and fact-checking**: Gemini 1.5
- **Cost-sensitive projects**: Mistral 7B or Llama 3.1
- **Multimodal tasks**: GPT-4o or Gemini 1.5

**Step 4: Test and Compare**
- Try the same prompt on 2-3 different models
- Compare quality, speed, and cost
- Choose the best fit for your needs

**Step 5: Document Your Choice**
- Record which tool works best for which tasks
- Build a personal "tool selection guide"
- Share insights with your team or clients

### **Real-World Application Exercise (5 minutes)**

**Scenario**: You're a marketing consultant helping a client choose AI tools

**Client Needs**:
- Analyze 50-page market research reports
- Create social media content
- Research competitors
- Stay within a $100/month budget

**Your Task**: Recommend the best AI tools for each need

**Step-by-Step Solution**:

**Need 1: Analyze 50-page reports**
- **Best Choice**: Claude 3.5 Sonnet
- **Why**: Large context window, excellent analysis
- **Cost**: ~$5-10 per report

**Need 2: Create social media content**
- **Best Choice**: GPT-4o
- **Why**: Creative, engaging content generation
- **Cost**: ~$2-5 per batch of posts

**Need 3: Research competitors**
- **Best Choice**: Gemini 1.5 Pro
- **Why**: Excellent research capabilities, large context
- **Cost**: ~$3-8 per research session

**Need 4: Stay within $100/month budget**
- **Strategy**: Use free tiers when possible, paid for complex tasks
- **Estimated Monthly Cost**: $60-80
- **Savings**: Use Mistral 7B for simple tasks

**Final Recommendation**:
"Use Claude 3.5 for report analysis, GPT-4o for content creation, Gemini 1.5 for research, and Mistral 7B for simple tasks. This combination gives you the best results while staying within budget."

---

## **Assessment and Wrap-up (15 minutes)**

### **Quick Knowledge Check (5 minutes)**
**Questions**:
1. Name 3 major AI models and their main strengths
2. What is a "hallucination" in AI?
3. How can you reduce bias in AI responses?
4. What's the best AI model for analyzing long documents?

### **Key Takeaways (5 minutes)**
1. **Different AI models have different strengths** - choose the right tool for the job
2. **AI has limitations** - understanding them helps you work around them
3. **Testing and comparison** - always test multiple models for important tasks
4. **Cost vs. quality** - balance your needs with your budget

### **Preview of Next Session (5 minutes)**
"Next time, we'll dive into Module 2: Core Prompt Engineering Techniques. We'll learn advanced prompting strategies like few-shot learning, chain-of-thought prompting, and role-based prompting. You'll master techniques that make you a true prompt engineering expert!"

---

## **Homework Assignment**

### **Practice Exercises**:
1. **Test 3 different AI models** on the same task and compare results
2. **Identify 5 AI limitations** in real-world scenarios
3. **Create prompts that work around limitations** for 3 different tasks
4. **Build your personal AI tool selection guide** with recommendations

### **Real-World Application**:
1. **Choose an AI tool** for a real project you're working on
2. **Document your decision process** and results
3. **Share your findings** in the class forum

### **Reflection Questions**:
1. Which AI model surprised you most with its capabilities?
2. What limitation do you think will be most challenging to work around?
3. How will understanding AI capabilities help your career?
4. What questions do you have about choosing the right AI tools?

---

## **Instructor Notes**

### **Common Student Questions**:
- **"Which AI model is the best?"** → Explain that different models excel at different tasks
- **"How do I know if AI is giving me accurate information?"** → Teach them to verify important facts
- **"Why do AI responses sometimes vary in quality?"** → Explain the probabilistic nature of AI
- **"How much should I spend on AI tools?"** → Help them calculate ROI for their use cases

### **Troubleshooting for Beginners**:
- **"I can't access certain AI models"** → Provide alternatives and free options
- **"The AI gave me wrong information"** → Show them how to verify and fact-check
- **"I don't understand the technical terms"** → Use simple analogies and examples
- **"How do I know which model to use?"** → Provide decision frameworks and examples

### **Engagement Strategies**:
- **Use real examples**: Connect to their work or daily life
- **Encourage experimentation**: Let them test different models
- **Celebrate discoveries**: When they find something interesting, acknowledge it
- **Connect to career goals**: Show how this knowledge helps their job prospects

### **Making It Accessible**:
- **Provide comparison charts**: Visual aids help students understand differences
- **Use simple language**: Avoid technical jargon
- **Offer multiple examples**: Show different ways to approach the same task
- **Give practical frameworks**: Decision trees and checklists they can use

### **What to Do If Students Struggle**:
1. **Start with basics**: Ensure they understand fundamental concepts first
2. **Provide templates**: Give them frameworks to follow
3. **Use visual aids**: Charts and diagrams help explain complex concepts
4. **Encourage questions**: Create a safe space for learning

---

## **Resources for Students**

### **AI Model Comparison Chart**:

| Model | Best For | Context Window | Cost | Special Features |
|-------|----------|----------------|------|------------------|
| GPT-4o | General tasks, creativity | 128K tokens | $5-15/1M | Multimodal |
| Claude 3.5 | Analysis, long docs | 200K tokens | $3-15/1M | Excellent reasoning |
| Gemini 1.5 | Research, fact-checking | 1M tokens | $1-7/1M | Massive context |
| Llama 3.1 | Custom apps, privacy | 128K tokens | Free | Open source |
| Mistral 7B | Fast, simple tasks | 32K tokens | Very low | Efficient |

### **Decision Framework**:

**For Long Documents**: Claude 3.5 or Gemini 1.5
**For Creative Writing**: GPT-4o or Claude 3.5
**For Research**: Gemini 1.5
**For Cost-Sensitive Projects**: Mistral 7B or Llama 3.1
**For Multimodal Tasks**: GPT-4o or Gemini 1.5

### **Limitation Checklist**:

**Before Using AI**:
- [ ] Will this task require real-time information?
- [ ] Could the AI hallucinate important details?
- [ ] Is there potential for bias in the output?
- [ ] Do I need to verify the information?
- [ ] Is the context within the model's limits?

### **Testing Prompts**:

**For Capability Testing**:
```
"Test this AI model's ability to [specific task]. Please show your reasoning process and provide specific examples."
```

**For Limitation Testing**:
```
"Please be honest about any limitations or uncertainties in your response. If you're making assumptions, clearly state them."
```

### **Career Application Examples**:

**For Marketing Professionals**:
- Use GPT-4o for creative campaigns
- Use Claude 3.5 for market analysis
- Use Gemini 1.5 for competitor research

**For Business Analysts**:
- Use Claude 3.5 for data analysis
- Use Gemini 1.5 for research
- Use GPT-4o for report writing

**For Content Creators**:
- Use GPT-4o for creative writing
- Use Claude 3.5 for editing and refinement
- Use Gemini 1.5 for fact-checking

### **Safety and Ethics Guidelines**:

**Always**:
- Verify important information
- Check for bias in outputs
- Be transparent about AI use
- Respect privacy and confidentiality

**Never**:
- Rely solely on AI for critical decisions
- Use AI to generate harmful content
- Share confidential information with AI
- Ignore AI limitations and risks
