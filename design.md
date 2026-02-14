# PathForge AI – System Design

## 1. Solution Overview
PathForge AI is an AI-powered skill-gap analysis and career planning platform. It analyzes a user’s current skills and compares them with their desired career role. The system models each career as a dynamic skill graph, identifies missing skills, ranks them by priority, and generates a structured learning roadmap.

The platform acts as a virtual career intelligence system, guiding users from their current state to their target career using AI-driven skill graph analysis.

The system leverages AWS serverless infrastructure to ensure scalability, reliability, and cost-efficient deployment across large user bases.

---

## 2. System Components
- User Interface (Frontend)
- API Gateway
- Serverless Backend
- Skill Graph Engine
- AI Recommendation Engine
- Database
- Storage

---

## 3. Technology Stack

### Frontend
- HTML, CSS, JavaScript
- AWS Amplify (hosting and deployment)

### Backend
- Python (Flask or FastAPI)
- AWS Lambda (serverless backend)

### AI Services
- AWS Bedrock for skill-gap analysis and roadmap generation

### Database
- AWS DynamoDB for storing:
  - User profiles
  - Skill graphs
  - Roadmap results

### Storage
- AWS S3 for static assets and learning resources

---

## 4. AWS System Architecture
The system is built using a serverless AWS architecture:

1. The user interacts with the web interface hosted on AWS Amplify.
2. The frontend sends user data to an API endpoint.
3. API Gateway forwards the request to AWS Lambda.
4. Lambda processes the data and invokes the Skill Graph Engine.
5. The engine sends structured prompts to AWS Bedrock.
6. Bedrock performs skill-gap analysis and generates a roadmap.
7. Results are stored in DynamoDB.
8. The response is returned to the frontend and displayed to the user.

---

## 5. Core Modules

### A. User Profile Module
- Collects user career goals
- Stores current skills
- Maintains user progress data

### B. Skill Graph Engine
- Models each career as a graph of skills
- Each node represents a skill
- Edges represent dependencies or prerequisites
- Stores graph structure in DynamoDB

### C. Skill Gap Analysis Module
- Maps user skills onto the career skill graph
- Detects missing nodes
- Identifies weak or incomplete skill paths

### D. Learning Roadmap Engine
- Ranks missing skills based on:
  - Importance
  - Market demand
  - Dependency depth
- Generates a structured, time-bound learning plan
- Creates weekly milestones

### E. AI Guidance Assistant
- Provides conversational career guidance
- Answers user questions about skills and careers
- Suggests next steps in the roadmap

### F. Progress Tracking Module
- Tracks completed skills
- Updates skill-gap analysis dynamically
- Recommends next learning steps

---

## 6. Skill Gap Analysis Logic
1. The system maps the selected career to a predefined skill graph derived from job-role datasets.
2. Each skill node contains:
   - Importance score
   - Dependency links
   - Market demand weight
3. User-provided skills are matched against graph nodes.
4. Missing nodes are identified.
5. Skills are ranked based on:
   - Importance
   - Dependency depth
   - Market demand
6. The roadmap engine generates an optimal learning path.

---

## 7. Data Flow
User Input → Frontend (Amplify)  
Frontend → API Gateway  
API Gateway → AWS Lambda  
Lambda → Skill Graph Engine  
Skill Graph Engine → AWS Bedrock (AI analysis)  
Bedrock → Lambda (response)  
Lambda → DynamoDB (store results)  
Lambda → Frontend → User

---

## 8. Scalability and Future Enhancements
- Integration with real job portals
- Real-time progress tracking
- AI-based mock interviews
- Multilingual support using AWS AI services
- Mobile app deployment
- Career path simulation engine
- Large-scale deployment using AWS serverless architecture

---

## 9. Why AWS
PathForge AI uses AWS serverless services to ensure scalability, reliability, and cost efficiency.

- AWS Bedrock enables scalable AI-driven skill-gap analysis.
- AWS Lambda provides serverless backend processing.
- DynamoDB ensures fast and scalable user data storage.
- Amplify allows rapid frontend deployment.

This architecture allows the system to scale from hundreds to millions of users without major infrastructure changes.
