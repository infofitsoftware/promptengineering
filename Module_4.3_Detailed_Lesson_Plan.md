# Module 4.3: Multi-Agent Systems and Orchestration
## Detailed Lesson Plan for Complete Beginners

### **Course Information**
- **Duration**: 4 hours
- **Format**: Interactive lecture + step-by-step hands-on labs
- **Prerequisites**: Completed Module 4.2 (Fine-tuning and Custom Models)
- **Learning Objectives**: By the end of this session, students will master agent-based architectures, tool calling, agent communication patterns, workflow orchestration, and build automated multi-agent systems

---

## **Part 1: Introduction to Multi-Agent Systems (60 minutes)**

### **Opening Hook - The Multi-Agent Success Story (15 minutes)**
**Meet Lisa - The Multi-Agent Systems Success Story**:
"Lisa was a software engineer at a fintech company struggling with complex customer onboarding that required multiple departments and systems. After implementing multi-agent systems, she automated 90% of the onboarding process, reduced processing time from 5 days to 2 hours, and got promoted to AI Systems Architect in 6 months. She now leads a team of 15 engineers, all building multi-agent systems that generate $5M+ in annual value for the company."

**What You'll Learn Today**:
- Professional agent-based architecture design and implementation
- Advanced tool calling and function usage techniques
- Agent communication patterns and coordination strategies
- Workflow orchestration and automation systems
- Building production-ready multi-agent applications
- Latest 2024 multi-agent tools and market trends

### **Understanding Multi-Agent Systems (45 minutes)**

**Think of Multi-Agent Systems Like Having a Team of Specialists**:
"Multi-agent systems are like having a team of specialists where each person has their own expertise and tools. They work together to solve complex problems that no single person could handle alone. Each agent is like a specialist who knows how to do specific tasks and can communicate with other specialists to coordinate their work."

**Why Multi-Agent Systems Are In High Demand**:
- **Market Demand**: 70% of enterprise AI projects use multi-agent systems
- **Complexity Handling**: Solve problems too complex for single agents
- **Efficiency**: 5-10x faster than sequential processing
- **Career Advancement**: Multi-agent engineers earn 50% more than standard AI engineers

**Real-World Multi-Agent Success Stories**:

**Story 1: Customer Service Automation**
- **Challenge**: Complex customer issues requiring multiple departments
- **Multi-Agent Solution**: 5 specialized agents (billing, technical, account, escalation, follow-up)
- **Result**: 80% faster resolution, 95% customer satisfaction
- **Revenue Impact**: $3M additional revenue through improved customer retention

**Story 2: Financial Trading System**
- **Challenge**: Real-time trading decisions requiring multiple data sources
- **Multi-Agent Solution**: 8 specialized agents (market analysis, risk assessment, execution, monitoring)
- **Result**: 40% better trading performance, 60% risk reduction
- **Revenue Impact**: $10M additional trading profits annually

**Story 3: Healthcare Diagnosis System**
- **Challenge**: Complex medical cases requiring multiple specialists
- **Multi-Agent Solution**: 6 specialized agents (symptoms analysis, lab results, imaging, treatment, monitoring, follow-up)
- **Result**: 50% faster diagnosis, 30% improvement in accuracy
- **Impact**: Saved 1000+ lives through faster, more accurate diagnoses

**Multi-Agent System Components**:

**1. Agent Architecture**
- **Purpose**: Define how individual agents work
- **Components**: Perception, reasoning, action, communication
- **Example**: Customer service agent that can understand, analyze, and respond

**2. Communication Protocols**
- **Purpose**: Enable agents to work together
- **Methods**: Message passing, shared memory, event-driven
- **Example**: Agents sharing information about customer issues

**3. Coordination Mechanisms**
- **Purpose**: Manage agent interactions and conflicts
- **Methods**: Centralized, decentralized, hierarchical
- **Example**: Manager agent coordinating specialist agents

**4. Workflow Orchestration**
- **Purpose**: Define and execute complex processes
- **Components**: Task scheduling, dependency management, error handling
- **Example**: Customer onboarding workflow with multiple steps

**Latest 2024 Multi-Agent Trends**:
- **Autonomous Agents**: Self-directed agents with goal-oriented behavior
- **Tool Integration**: Advanced tool calling and function usage
- **Real-time Coordination**: Live agent communication and collaboration
- **Human-AI Collaboration**: Seamless human and agent interaction
- **Enterprise Orchestration**: Production-ready multi-agent platforms

---

## **Part 2: Agent-Based Architectures (60 minutes)**

### **Understanding Agent Architectures (30 minutes)**

**Think of Agent Architecture Like Building a Robot**:
"Agent architecture is like designing a robot that can perceive its environment, think about what to do, take actions, and communicate with other robots. Each agent needs sensors (perception), a brain (reasoning), actuators (actions), and communication systems (interaction)."

**Core Agent Components**:

**1. Perception Module**
- **Purpose**: Understand the environment and inputs
- **Components**: Input processing, data interpretation, context awareness
- **Example**: Customer service agent understanding customer messages

**2. Reasoning Module**
- **Purpose**: Make decisions and plan actions
- **Components**: Knowledge base, decision logic, planning algorithms
- **Example**: Agent deciding which specialist to involve for a customer issue

**3. Action Module**
- **Purpose**: Execute tasks and interact with systems
- **Components**: Tool calling, API integration, system interaction
- **Example**: Agent updating customer records or sending notifications

**4. Communication Module**
- **Purpose**: Interact with other agents and humans
- **Components**: Message handling, protocol management, coordination
- **Example**: Agent requesting help from another specialist agent

**Agent Architecture Patterns**:

**Pattern 1: Reactive Agents**
```
Input → Processing → Action → Output
```
**Use Case**: Simple, fast responses to specific inputs
**Example**: Chatbot responding to common questions
**Pros**: Fast, simple, predictable
**Cons**: Limited reasoning, no memory

**Pattern 2: Deliberative Agents**
```
Input → Planning → Reasoning → Action → Output
```
**Use Case**: Complex decision-making and planning
**Example**: Financial advisor agent analyzing investment options
**Pros**: Sophisticated reasoning, goal-oriented
**Cons**: Slower, more complex

**Pattern 3: Hybrid Agents**
```
Input → Reactive Response + Deliberative Planning → Action → Output
```
**Use Case**: Balance between speed and sophistication
**Example**: Customer service agent with quick responses and deep analysis
**Pros**: Best of both worlds, flexible
**Cons**: More complex to implement

### **Agent Implementation Strategies (30 minutes)**

**Strategy 1: Single-Purpose Agents**
```
Agent 1: Data Collection
Agent 2: Data Analysis
Agent 3: Report Generation
Agent 4: Distribution
```
**Implementation**: Each agent has one specific responsibility
**Use Case**: Well-defined, sequential processes
**Example**: Document processing pipeline

**Strategy 2: Multi-Purpose Agents**
```
Agent 1: Customer Service (billing, technical, account)
Agent 2: Sales Support (leads, demos, proposals)
Agent 3: Operations (scheduling, monitoring, reporting)
```
**Implementation**: Each agent handles multiple related tasks
**Use Case**: Domain-specific expertise
**Example**: Industry-specific customer service

**Strategy 3: Hierarchical Agents**
```
Manager Agent
├── Specialist Agent 1
├── Specialist Agent 2
└── Specialist Agent 3
```
**Implementation**: Manager coordinates specialist agents
**Use Case**: Complex coordination and oversight
**Example**: Project management with multiple teams

**Strategy 4: Peer-to-Peer Agents**
```
Agent 1 ↔ Agent 2 ↔ Agent 3
```
**Implementation**: Agents communicate directly with each other
**Use Case**: Collaborative problem-solving
**Example**: Research team working on complex problems

---

## **Part 3: Tool Calling and Function Usage (60 minutes)**

### **Understanding Tool Calling (30 minutes)**

**Think of Tool Calling Like Having a Swiss Army Knife**:
"Tool calling is like having a Swiss Army Knife where each tool has a specific purpose. The agent can look at the available tools, decide which one to use, and then use it to accomplish a specific task. Each tool is like a specialized function that the agent can call when needed."

**Tool Calling Components**:

**1. Tool Definition**
- **Purpose**: Define what tools are available
- **Components**: Function name, parameters, description, examples
- **Example**: `get_weather(location, date)` function

**2. Tool Selection**
- **Purpose**: Choose the right tool for the task
- **Methods**: Rule-based, ML-based, context-aware
- **Example**: Agent choosing weather tool for weather-related questions

**3. Tool Execution**
- **Purpose**: Execute the selected tool
- **Components**: Parameter validation, execution, result handling
- **Example**: Calling weather API with location and date

**4. Result Processing**
- **Purpose**: Handle and interpret tool results
- **Components**: Error handling, data formatting, context integration
- **Example**: Converting weather data into user-friendly response

**Tool Categories**:

**1. Data Access Tools**
- **Purpose**: Retrieve information from databases and APIs
- **Examples**: Database queries, API calls, file reading
- **Use Case**: Getting customer information, product details

**2. Processing Tools**
- **Purpose**: Transform and analyze data
- **Examples**: Data analysis, calculations, text processing
- **Use Case**: Analyzing customer data, generating reports

**3. Communication Tools**
- **Purpose**: Send messages and notifications
- **Examples**: Email, SMS, Slack, webhooks
- **Use Case**: Sending confirmations, alerts, updates

**4. System Integration Tools**
- **Purpose**: Interact with external systems
- **Examples**: CRM updates, payment processing, scheduling
- **Use Case**: Updating customer records, processing orders

### **Function Usage Patterns (30 minutes)**

**Pattern 1: Sequential Tool Calling**
```
Task: Process customer order
1. get_customer_info(customer_id)
2. check_inventory(product_id)
3. calculate_total(items, discounts)
4. process_payment(customer_id, amount)
5. send_confirmation(customer_id, order_id)
```
**Use Case**: Step-by-step processes with dependencies
**Example**: Order processing workflow

**Pattern 2: Parallel Tool Calling**
```
Task: Generate comprehensive report
1. get_sales_data() (parallel)
2. get_customer_data() (parallel)
3. get_product_data() (parallel)
4. combine_results(all_data)
```
**Use Case**: Independent tasks that can run simultaneously
**Example**: Dashboard data collection

**Pattern 3: Conditional Tool Calling**
```
Task: Handle customer inquiry
if inquiry_type == "billing":
    get_billing_info(customer_id)
elif inquiry_type == "technical":
    get_technical_support(customer_id)
else:
    get_general_info(customer_id)
```
**Use Case**: Different paths based on conditions
**Example**: Customer service routing

**Pattern 4: Iterative Tool Calling**
```
Task: Find best solution
while not solution_found:
    try_solution(current_approach)
    if not successful:
        adjust_approach()
        try_solution(new_approach)
```
**Use Case**: Problem-solving with multiple attempts
**Example**: Troubleshooting technical issues

---

## **Part 4: Agent Communication Patterns (60 minutes)**

### **Understanding Agent Communication (30 minutes)**

**Think of Agent Communication Like Team Meetings**:
"Agent communication is like having team meetings where different specialists share information, coordinate their work, and make decisions together. Each agent needs to know how to send messages, receive information, and work together effectively."

**Communication Patterns**:

**1. Direct Communication**
```
Agent A → Message → Agent B
```
**Use Case**: Simple, direct information sharing
**Example**: Customer service agent asking billing agent for account info
**Pros**: Simple, fast, direct
**Cons**: Limited scalability, tight coupling

**2. Broadcast Communication**
```
Agent A → Message → All Agents
```
**Use Case**: Announcements and updates
**Example**: System maintenance notification to all agents
**Pros**: Efficient for announcements, loose coupling
**Cons**: May create noise, not targeted

**3. Mediated Communication**
```
Agent A → Message → Mediator → Agent B
```
**Use Case**: Complex coordination and routing
**Example**: Manager agent coordinating specialist agents
**Pros**: Centralized control, flexible routing
**Cons**: Single point of failure, potential bottleneck

**4. Event-Driven Communication**
```
Event → Event Bus → Interested Agents
```
**Use Case**: Reactive systems and notifications
**Example**: Order completion event notifying multiple agents
**Pros**: Loose coupling, scalable, reactive
**Cons**: Complex to implement, debugging challenges

### **Communication Protocols (30 minutes)**

**Protocol 1: Request-Response**
```
Agent A: "Can you get customer info for ID 12345?"
Agent B: "Here's the customer info: {name: John, email: john@example.com}"
```
**Use Case**: Synchronous information requests
**Example**: Customer service agent requesting account details
**Implementation**: HTTP-like request-response pattern

**Protocol 2: Publish-Subscribe**
```
Publisher: "New order received: Order #12345"
Subscribers: [Inventory Agent, Billing Agent, Shipping Agent]
```
**Use Case**: Asynchronous notifications and updates
**Example**: Order system notifying multiple departments
**Implementation**: Message queue or event bus

**Protocol 3: Message Passing**
```
Agent A: "I need help with technical issue #456"
Agent B: "I can help. What's the specific problem?"
Agent A: "Customer can't access their account"
Agent B: "Let me check the system status..."
```
**Use Case**: Conversational and collaborative work
**Example**: Agents working together to solve complex problems
**Implementation**: Chat-like message exchange

**Protocol 4: Shared Memory**
```
Shared Memory: {customer_id: 12345, status: "active", last_login: "2024-01-15"}
Agent A: Reads customer status
Agent B: Updates last login time
Agent C: Reads updated information
```
**Use Case**: Shared state and information
**Example**: Agents sharing customer session information
**Implementation**: Database or in-memory store

---

## **Part 5: Workflow Orchestration (60 minutes)**

### **Understanding Workflow Orchestration (30 minutes)**

**Think of Workflow Orchestration Like Conducting an Orchestra**:
"Workflow orchestration is like conducting an orchestra where you need to coordinate different musicians (agents) to play their parts at the right time, in the right order, and with the right tempo. The conductor (orchestrator) ensures everyone works together to create beautiful music (complete the workflow)."

**Workflow Components**:

**1. Task Definition**
- **Purpose**: Define what needs to be done
- **Components**: Task name, description, inputs, outputs, requirements
- **Example**: "Validate customer information" task

**2. Task Dependencies**
- **Purpose**: Define the order of task execution
- **Components**: Predecessors, successors, conditions, triggers
- **Example**: "Send confirmation" depends on "Process payment"

**3. Task Assignment**
- **Purpose**: Assign tasks to appropriate agents
- **Components**: Agent selection, load balancing, availability
- **Example**: Assign billing tasks to billing agents

**4. Execution Monitoring**
- **Purpose**: Track task progress and handle issues
- **Components**: Status tracking, error handling, retry logic
- **Example**: Monitor payment processing and retry if failed

**Workflow Patterns**:

**Pattern 1: Sequential Workflow**
```
Task 1 → Task 2 → Task 3 → Task 4
```
**Use Case**: Step-by-step processes with strict order
**Example**: Customer onboarding (signup → verification → activation → welcome)

**Pattern 2: Parallel Workflow**
```
Task 1 → Task 2
Task 3 → Task 4
```
**Use Case**: Independent tasks that can run simultaneously
**Example**: Order processing (inventory check + payment processing)

**Pattern 3: Conditional Workflow**
```
Task 1 → Decision Point
├─ Condition A → Task 2A
└─ Condition B → Task 2B
```
**Use Case**: Different paths based on conditions
**Example**: Customer service (billing issue → billing agent, technical issue → tech agent)

**Pattern 4: Loop Workflow**
```
Task 1 → Task 2 → Decision Point
├─ Success → Task 3
└─ Failure → Task 1 (retry)
```
**Use Case**: Retry logic and iterative processes
**Example**: Payment processing with retry on failure

### **Orchestration Strategies (30 minutes)**

**Strategy 1: Centralized Orchestration**
```
Orchestrator
├── Agent 1
├── Agent 2
└── Agent 3
```
**Implementation**: Single orchestrator controls all agents
**Use Case**: Complex coordination and oversight
**Example**: Project manager coordinating development team
**Pros**: Centralized control, easy monitoring
**Cons**: Single point of failure, potential bottleneck

**Strategy 2: Decentralized Orchestration**
```
Agent 1 ↔ Agent 2 ↔ Agent 3
```
**Implementation**: Agents coordinate directly with each other
**Use Case**: Collaborative and adaptive systems
**Example**: Research team working on complex problems
**Pros**: Resilient, scalable, adaptive
**Cons**: Complex coordination, difficult monitoring

**Strategy 3: Hybrid Orchestration**
```
Orchestrator
├── Sub-Orchestrator 1 → Agent 1, Agent 2
└── Sub-Orchestrator 2 → Agent 3, Agent 4
```
**Implementation**: Hierarchical orchestration with multiple levels
**Use Case**: Large-scale systems with multiple domains
**Example**: Enterprise system with department-level coordination
**Pros**: Scalable, organized, manageable
**Cons**: Complex to implement, multiple failure points

**Strategy 4: Event-Driven Orchestration**
```
Event → Event Bus → Orchestrator → Agents
```
**Implementation**: Orchestration triggered by events
**Use Case**: Reactive and responsive systems
**Example**: Customer service system responding to customer actions
**Pros**: Reactive, scalable, loose coupling
**Cons**: Complex event handling, debugging challenges

---

## **Part 6: Hands-on Lab - Building Multi-Agent Systems (60 minutes)**

### **Lab Setup - Getting Ready (10 minutes)**

**What You'll Need**:
- Access to Google Colab or local Python environment
- OpenAI API key or access to other LLM APIs
- Basic understanding of Python and APIs
- Sample data for your multi-agent system

**Step-by-Step Setup**:
1. Open Google Colab or your Python environment
2. Install required libraries: `pip install openai langchain`
3. Set up API keys and authentication
4. Prepare sample data for your multi-agent system

### **Lab Exercise 1: Basic Multi-Agent System (20 minutes)**

**Task**: Build a simple customer service multi-agent system

**Step-by-Step Instructions**:

**Step 1**: Set up the basic multi-agent system

```python
# Install required libraries
!pip install openai langchain

# Import libraries
import openai
from typing import Dict, List, Any
import json

# Set up OpenAI API
openai.api_key = "your-api-key-here"

# Define agent classes
class Agent:
    def __init__(self, name: str, role: str, tools: List[str]):
        self.name = name
        self.role = role
        self.tools = tools
        self.conversation_history = []
    
    def process_message(self, message: str, context: Dict = None) -> str:
        # Add message to conversation history
        self.conversation_history.append({"role": "user", "content": message})
        
        # Create system prompt for the agent
        system_prompt = f"""
        You are {self.name}, a {self.role} agent.
        Your available tools are: {', '.join(self.tools)}
        
        Your role is to help customers with {self.role} related issues.
        Be helpful, professional, and concise.
        If you need to use a tool, mention it in your response.
        """
        
        # Prepare messages for OpenAI
        messages = [{"role": "system", "content": system_prompt}]
        messages.extend(self.conversation_history)
        
        # Get response from OpenAI
        response = openai.ChatCompletion.create(
            model="gpt-3.5-turbo",
            messages=messages,
            max_tokens=200
        )
        
        agent_response = response.choices[0].message.content
        
        # Add response to conversation history
        self.conversation_history.append({"role": "assistant", "content": agent_response})
        
        return agent_response

# Create specialized agents
billing_agent = Agent("BillingBot", "billing", ["get_account_balance", "process_payment", "update_billing_info"])
technical_agent = Agent("TechBot", "technical support", ["check_system_status", "reset_password", "escalate_issue"])
account_agent = Agent("AccountBot", "account management", ["update_profile", "change_settings", "close_account"])

# Test individual agents
print("Testing Billing Agent:")
billing_response = billing_agent.process_message("I need to check my account balance")
print(f"Billing Agent: {billing_response}")

print("\nTesting Technical Agent:")
tech_response = technical_agent.process_message("I can't log into my account")
print(f"Technical Agent: {tech_response}")

print("\nTesting Account Agent:")
account_response = account_agent.process_message("I want to update my email address")
print(f"Account Agent: {account_response}")
```

**Step 2**: Create a coordinator agent

```python
class CoordinatorAgent:
    def __init__(self):
        self.agents = {
            "billing": billing_agent,
            "technical": technical_agent,
            "account": account_agent
        }
        self.conversation_history = []
    
    def route_message(self, message: str) -> str:
        # Simple routing logic based on keywords
        message_lower = message.lower()
        
        if any(word in message_lower for word in ["bill", "payment", "charge", "invoice", "balance"]):
            agent = self.agents["billing"]
            agent_type = "billing"
        elif any(word in message_lower for word in ["login", "password", "error", "bug", "technical"]):
            agent = self.agents["technical"]
            agent_type = "technical"
        elif any(word in message_lower for word in ["profile", "settings", "account", "update", "change"]):
            agent = self.agents["account"]
            agent_type = "account"
        else:
            # Default to general response
            return "I understand you need help. Could you please provide more details about your issue so I can connect you with the right specialist?"
        
        # Route to appropriate agent
        response = agent.process_message(message)
        return f"[{agent_type.upper()} AGENT] {response}"
    
    def handle_complex_query(self, message: str) -> str:
        # For complex queries that might need multiple agents
        message_lower = message.lower()
        
        if "billing" in message_lower and "technical" in message_lower:
            # Need both billing and technical agents
            billing_response = self.agents["billing"].process_message(message)
            tech_response = self.agents["technical"].process_message(message)
            return f"[COORDINATED RESPONSE]\nBilling: {billing_response}\nTechnical: {tech_response}"
        else:
            # Route to single agent
            return self.route_message(message)

# Test the coordinator
coordinator = CoordinatorAgent()

print("Testing Coordinator - Billing Query:")
response = coordinator.route_message("I have a billing question about my last invoice")
print(f"Coordinator: {response}")

print("\nTesting Coordinator - Technical Query:")
response = coordinator.route_message("I'm having trouble logging into my account")
print(f"Coordinator: {response}")

print("\nTesting Coordinator - Complex Query:")
response = coordinator.handle_complex_query("I can't log in and I think it's related to my billing issue")
print(f"Coordinator: {response}")
```

### **Lab Exercise 2: Advanced Multi-Agent System with Tools (20 minutes)**

**Task**: Build an advanced multi-agent system with tool calling

**Step-by-Step Instructions**:

**Step 1**: Create agents with tool calling capabilities

```python
class ToolCallingAgent:
    def __init__(self, name: str, role: str, tools: Dict[str, callable]):
        self.name = name
        self.role = role
        self.tools = tools
        self.conversation_history = []
    
    def call_tool(self, tool_name: str, parameters: Dict) -> str:
        if tool_name in self.tools:
            try:
                result = self.tools[tool_name](**parameters)
                return f"Tool '{tool_name}' executed successfully. Result: {result}"
            except Exception as e:
                return f"Tool '{tool_name}' failed with error: {str(e)}"
        else:
            return f"Tool '{tool_name}' not available"
    
    def process_message(self, message: str) -> str:
        # Add message to conversation history
        self.conversation_history.append({"role": "user", "content": message})
        
        # Create system prompt
        system_prompt = f"""
        You are {self.name}, a {self.role} agent.
        Available tools: {list(self.tools.keys())}
        
        When you need to use a tool, respond with:
        TOOL_CALL: tool_name(parameter1=value1, parameter2=value2)
        
        Be helpful and use tools when appropriate.
        """
        
        # Prepare messages
        messages = [{"role": "system", "content": system_prompt}]
        messages.extend(self.conversation_history)
        
        # Get response from OpenAI
        response = openai.ChatCompletion.create(
            model="gpt-3.5-turbo",
            messages=messages,
            max_tokens=200
        )
        
        agent_response = response.choices[0].message.content
        
        # Check if response contains tool call
        if "TOOL_CALL:" in agent_response:
            # Extract tool call
            tool_call_line = agent_response.split("TOOL_CALL:")[1].strip()
            tool_name = tool_call_line.split("(")[0]
            parameters_str = tool_call_line.split("(")[1].split(")")[0]
            
            # Parse parameters (simple parsing)
            parameters = {}
            if parameters_str:
                for param in parameters_str.split(","):
                    if "=" in param:
                        key, value = param.split("=")
                        parameters[key.strip()] = value.strip().strip('"')
            
            # Execute tool
            tool_result = self.call_tool(tool_name, parameters)
            agent_response = f"{agent_response}\n{tool_result}"
        
        # Add response to conversation history
        self.conversation_history.append({"role": "assistant", "content": agent_response})
        
        return agent_response

# Define tool functions
def get_customer_info(customer_id: str) -> str:
    # Simulate database lookup
    mock_data = {
        "12345": {"name": "John Doe", "email": "john@example.com", "balance": "$150.00"},
        "67890": {"name": "Jane Smith", "email": "jane@example.com", "balance": "$75.50"}
    }
    return json.dumps(mock_data.get(customer_id, {"error": "Customer not found"}))

def process_payment(customer_id: str, amount: str) -> str:
    # Simulate payment processing
    return f"Payment of {amount} processed successfully for customer {customer_id}"

def check_system_status() -> str:
    # Simulate system status check
    return "System status: All systems operational"

def reset_password(customer_id: str) -> str:
    # Simulate password reset
    return f"Password reset email sent to customer {customer_id}"

# Create agents with tools
billing_agent = ToolCallingAgent(
    "BillingBot", 
    "billing", 
    {
        "get_customer_info": get_customer_info,
        "process_payment": process_payment
    }
)

technical_agent = ToolCallingAgent(
    "TechBot", 
    "technical support", 
    {
        "get_customer_info": get_customer_info,
        "check_system_status": check_system_status,
        "reset_password": reset_password
    }
)

# Test agents with tool calling
print("Testing Billing Agent with Tools:")
response = billing_agent.process_message("Can you check the account balance for customer 12345?")
print(f"Billing Agent: {response}")

print("\nTesting Technical Agent with Tools:")
response = technical_agent.process_message("I need to reset the password for customer 67890")
print(f"Technical Agent: {response}")
```

**Step 2**: Create a workflow orchestrator

```python
class WorkflowOrchestrator:
    def __init__(self):
        self.agents = {
            "billing": billing_agent,
            "technical": technical_agent
        }
        self.workflows = {
            "customer_onboarding": [
                "get_customer_info",
                "check_system_status",
                "send_welcome_email"
            ],
            "payment_processing": [
                "get_customer_info",
                "process_payment",
                "send_confirmation"
            ]
        }
    
    def execute_workflow(self, workflow_name: str, parameters: Dict) -> List[str]:
        if workflow_name not in self.workflows:
            return [f"Workflow '{workflow_name}' not found"]
        
        results = []
        workflow_steps = self.workflows[workflow_name]
        
        for step in workflow_steps:
            if step == "get_customer_info":
                result = self.agents["billing"].call_tool("get_customer_info", parameters)
                results.append(f"Step: {step} - {result}")
            elif step == "process_payment":
                result = self.agents["billing"].call_tool("process_payment", parameters)
                results.append(f"Step: {step} - {result}")
            elif step == "check_system_status":
                result = self.agents["technical"].call_tool("check_system_status", {})
                results.append(f"Step: {step} - {result}")
            elif step == "send_welcome_email":
                results.append(f"Step: {step} - Welcome email sent to customer {parameters.get('customer_id', 'unknown')}")
            elif step == "send_confirmation":
                results.append(f"Step: {step} - Payment confirmation sent to customer {parameters.get('customer_id', 'unknown')}")
        
        return results
    
    def handle_complex_request(self, message: str) -> str:
        # Analyze message to determine workflow
        message_lower = message.lower()
        
        if "onboard" in message_lower or "new customer" in message_lower:
            # Extract customer ID from message
            customer_id = "12345"  # In real implementation, extract from message
            results = self.execute_workflow("customer_onboarding", {"customer_id": customer_id})
            return "Customer Onboarding Workflow:\n" + "\n".join(results)
        elif "payment" in message_lower or "pay" in message_lower:
            customer_id = "12345"  # In real implementation, extract from message
            amount = "$50.00"  # In real implementation, extract from message
            results = self.execute_workflow("payment_processing", {"customer_id": customer_id, "amount": amount})
            return "Payment Processing Workflow:\n" + "\n".join(results)
        else:
            return "I can help with customer onboarding or payment processing. Please specify which workflow you need."

# Test the workflow orchestrator
orchestrator = WorkflowOrchestrator()

print("Testing Customer Onboarding Workflow:")
response = orchestrator.handle_complex_request("I need to onboard a new customer")
print(f"Orchestrator: {response}")

print("\nTesting Payment Processing Workflow:")
response = orchestrator.handle_complex_request("I need to process a payment")
print(f"Orchestrator: {response}")
```

### **Lab Exercise 3: Multi-Agent Communication System (10 minutes)**

**Task**: Implement agent-to-agent communication

**Step-by-Step Instructions**:

**Step 1**: Create a communication system

```python
class CommunicationSystem:
    def __init__(self):
        self.message_queue = []
        self.agents = {}
    
    def register_agent(self, agent_name: str, agent):
        self.agents[agent_name] = agent
    
    def send_message(self, from_agent: str, to_agent: str, message: str, message_type: str = "request"):
        message_data = {
            "from": from_agent,
            "to": to_agent,
            "message": message,
            "type": message_type,
            "timestamp": "2024-01-15T10:30:00Z"
        }
        self.message_queue.append(message_data)
        
        # Process message immediately
        if to_agent in self.agents:
            return self.agents[to_agent].process_message(message)
        else:
            return f"Agent {to_agent} not found"
    
    def broadcast_message(self, from_agent: str, message: str, message_type: str = "announcement"):
        responses = []
        for agent_name in self.agents:
            if agent_name != from_agent:
                response = self.send_message(from_agent, agent_name, message, message_type)
                responses.append(f"{agent_name}: {response}")
        return responses
    
    def get_message_history(self, agent_name: str = None):
        if agent_name:
            return [msg for msg in self.message_queue if msg["to"] == agent_name or msg["from"] == agent_name]
        return self.message_queue

# Create communication system
comm_system = CommunicationSystem()

# Register agents
comm_system.register_agent("billing", billing_agent)
comm_system.register_agent("technical", technical_agent)

# Test agent-to-agent communication
print("Testing Agent-to-Agent Communication:")
response = comm_system.send_message("billing", "technical", "I need to check if the system is working before processing a payment")
print(f"Technical Agent Response: {response}")

print("\nTesting Broadcast Communication:")
responses = comm_system.broadcast_message("billing", "System maintenance scheduled for tonight at 2 AM")
for response in responses:
    print(f"Broadcast Response: {response}")

print("\nMessage History:")
history = comm_system.get_message_history()
for msg in history:
    print(f"{msg['from']} → {msg['to']}: {msg['message']}")
```

---

## **Assessment and Wrap-up (15 minutes)**

### **Quick Knowledge Check (5 minutes)**
**Questions**:
1. What are the main components of an agent architecture?
2. How do agents communicate with each other?
3. What is workflow orchestration?
4. How do you implement tool calling in agents?

### **Key Takeaways (5 minutes)**
1. **Multi-agent systems solve complex problems** - coordinate multiple specialists
2. **Agent architecture matters** - design for specific roles and capabilities
3. **Communication is key** - agents need to work together effectively
4. **Workflow orchestration coordinates** - manage complex processes
5. **Tool calling enhances capabilities** - agents can interact with external systems

### **Preview of Next Session (5 minutes)**
"Next time, we'll dive into Module 4.4: AI Ethics and Responsible AI. We'll learn about bias detection and mitigation, fairness in AI systems, transparency and explainability, and privacy-preserving prompting. You'll become an AI ethics expert!"

---

## **Homework Assignment**

### **Practice Exercises**:
1. **Build a multi-agent system** for a specific business process
2. **Implement agent communication** with different patterns
3. **Create a workflow orchestrator** for complex processes
4. **Add tool calling capabilities** to your agents

### **Real-World Application**:
1. **Start a multi-agent project** for a real business need
2. **Apply your multi-agent skills** to solve actual problems
3. **Conduct performance analysis** on different architectures
4. **Share your multi-agent systems** in the class forum

### **Reflection Questions**:
1. Which agent architecture was most effective for your use case?
2. How will you use multi-agent systems in your career?
3. What challenges did you face in agent communication?
4. How will you measure the success of your multi-agent system?

---

## **Instructor Notes**

### **Common Student Questions**:
- **"How many agents should I use?"** → Start with 3-5 agents, add more as needed
- **"How do I handle agent conflicts?"** → Use coordination mechanisms and clear roles
- **"What's the best communication pattern?"** → Choose based on your system's needs
- **"How do I scale multi-agent systems?"** → Use hierarchical and event-driven patterns

### **Troubleshooting for Beginners**:
- **"My agents aren't communicating"** → Check message formats and agent registration
- **"Workflow is getting stuck"** → Add error handling and timeout mechanisms
- **"System is too slow"** → Use parallel processing and optimize agent logic
- **"Agents are conflicting"** → Implement better coordination and role definition

### **Engagement Strategies**:
- **Use real examples**: Connect to their work or business interests
- **Encourage experimentation**: Let them try different agent architectures
- **Celebrate improvements**: When they build working systems, acknowledge it
- **Connect to career goals**: Show how multi-agent skills help their job prospects

### **Making It Accessible**:
- **Provide templates**: Give them starting points for different agent types
- **Use simple language**: Avoid jargon and complex technical concepts
- **Offer multiple examples**: Show different approaches to the same problem
- **Give practical frameworks**: Structures they can follow

### **What to Do If Students Struggle**:
1. **Start with simple examples**: Don't make them tackle complex multi-agent systems immediately
2. **Provide step-by-step guidance**: Break down complex tasks into manageable steps
3. **Encourage practice**: The more they build multi-agent systems, the better they get
4. **Focus on understanding**: Help them understand the concepts, not just the code

---

## **Resources for Students**

### **Multi-Agent System Templates**:

**Basic Agent Template**:
```python
class BasicAgent:
    def __init__(self, name, role, tools):
        self.name = name
        self.role = role
        self.tools = tools
        self.conversation_history = []
    
    def process_message(self, message):
        # Process message and return response
        pass
    
    def call_tool(self, tool_name, parameters):
        # Execute tool and return result
        pass
```

**Communication System Template**:
```python
class CommunicationSystem:
    def __init__(self):
        self.message_queue = []
        self.agents = {}
    
    def register_agent(self, agent_name, agent):
        # Register agent in the system
        pass
    
    def send_message(self, from_agent, to_agent, message):
        # Send message between agents
        pass
    
    def broadcast_message(self, from_agent, message):
        # Broadcast message to all agents
        pass
```

**Workflow Orchestrator Template**:
```python
class WorkflowOrchestrator:
    def __init__(self):
        self.agents = {}
        self.workflows = {}
    
    def execute_workflow(self, workflow_name, parameters):
        # Execute workflow with given parameters
        pass
    
    def handle_complex_request(self, message):
        # Route complex requests to appropriate workflows
        pass
```

### **Multi-Agent System Checklist**:

**Agent Design**:
- [ ] Define clear agent roles and responsibilities
- [ ] Implement proper agent architecture
- [ ] Add tool calling capabilities
- [ ] Include error handling and logging

**Communication**:
- [ ] Implement communication protocols
- [ ] Add message queuing and routing
- [ ] Include broadcast and direct messaging
- [ ] Handle communication failures

**Coordination**:
- [ ] Define coordination mechanisms
- [ ] Implement conflict resolution
- [ ] Add load balancing and scaling
- [ ] Include monitoring and metrics

**Workflow Management**:
- [ ] Define workflow patterns and templates
- [ ] Implement task scheduling and dependencies
- [ ] Add error handling and retry logic
- [ ] Include workflow monitoring and reporting

### **Multi-Agent System Best Practices**:

**Agent Design Principles**:
- Single responsibility principle
- Clear interfaces and contracts
- Proper error handling
- Logging and monitoring

**Communication Best Practices**:
- Use standard message formats
- Implement proper error handling
- Add message validation
- Include timeout mechanisms

**Coordination Strategies**:
- Define clear hierarchies
- Implement conflict resolution
- Add load balancing
- Include failover mechanisms

**Workflow Management**:
- Use workflow templates
- Implement proper error handling
- Add monitoring and metrics
- Include rollback capabilities

### **Multi-Agent System Use Cases**:

**Enterprise Applications**:
- Customer service automation
- Business process automation
- Supply chain management
- Project management

**Industry-Specific Systems**:
- Healthcare diagnosis and treatment
- Financial trading and analysis
- Manufacturing and quality control
- Education and training

**Consumer Applications**:
- Personal assistants
- Smart home automation
- E-commerce and recommendations
- Social media and content

**Research and Development**:
- Scientific discovery
- Drug development
- Climate modeling
- Space exploration
