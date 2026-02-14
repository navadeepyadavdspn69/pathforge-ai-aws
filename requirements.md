# PathForge AI – Requirements

## 1. Problem Statement
Many students struggle to choose the right career path due to a lack of personalized guidance and structured learning plans. Most existing platforms provide generic advice that does not consider a student’s interests, strengths, or goals. This leads to poor career decisions, wasted time, and low motivation.

## 1.1 Why This Problem Matters Today
- Rapid growth of online learning platforms has created information overload.
- Students face confusion due to too many unstructured resources.
- Skill-based hiring is increasing, but guidance systems remain generic.
- There is a growing need for AI-driven, personalized career planning tools.

---

## 2. Target Users
- High school students preparing for competitive exams (JEE, BITSAT, NEET, etc.)
- College students exploring career options
- Job seekers looking to switch careers
- Self-learners and skill-based learners

---

## 3. Solution Overview
PathForge AI is an AI-powered career intelligence platform that analyzes a user’s current skills and compares them with their desired career role. It models each career as a dynamic skill graph, identifies skill gaps, ranks missing skills by priority, and generates a structured, step-by-step learning roadmap.

### Example Use Case
A student who wants to become a Data Scientist but only knows basic Python enters their goal and skills.  
The system maps the Data Scientist role into a skill graph, detects missing nodes such as statistics, SQL, and machine learning, ranks them by importance, and generates a 12-week learning roadmap with weekly milestones and projects.

---

## 4. Key Features
- Dynamic skill graph–based career modeling
- Skill-gap analysis based on target career roles
- Job-market-aware skill comparison
- Skill priority ranking (critical vs secondary skills)
- Personalized learning roadmap
- Weekly milestones and structured progression
- Recommended courses, projects, and learning resources
- Multilingual career guidance
- Low-bandwidth, text-first interface

---

## 5. Functional Requirements
- The system should allow users to input their current skills and career goals.
- The AI engine should map the target career to a dynamic skill graph.
- The system should analyze the skill gap using job-role datasets.
- The system should rank missing skills based on importance and dependencies.
- The system should generate a structured, time-bound learning roadmap.
- The system should support multiple languages for broader accessibility.
- The system should provide recommended learning resources.
- The system should store user profiles and progress.

---

## 6. Non-Functional Requirements
- Fast response time (under 5 seconds)
- Scalable to large user bases using AWS
- Secure handling of user data
- High availability and reliability
- Simple and intuitive user interface
- Optimized for low-bandwidth environments

---

## 7. Expected Impact
- Helps students make informed career decisions
- Reduces confusion about career paths
- Provides structured and personalized learning plans
- Improves confidence and skill development
- Generates personalized career roadmaps in under 5 seconds
- Reduces career planning time by up to 60% for new learners
- Scalable to over 1 million users using AWS serverless infrastructure
- Provides optimal learning paths using AI-based skill graph analysis

---

## 8. Future Scope
- Integration with real-time job portals
- AI-powered mock interviews
- Progress tracking and skill assessments
- Personalized internship and job recommendations
- Mobile application deployment
- Career path simulation engine

---

## 9. Existing Solutions and Limitations
Many existing skill-gap tools are designed for enterprise HR systems or resume optimization platforms. These systems are primarily built for corporate employees and job matching, rather than for individual students or self-learners.

Limitations of current solutions:
- Focus on resume optimization instead of skill development
- Designed mainly for corporate environments
- Lack structured, goal-based learning roadmaps
- Not optimized for low-bandwidth or multilingual users
- Do not model career paths using structured skill relationships

PathForge AI addresses these gaps by providing a student-centric, goal-driven learning roadmap system powered by dynamic skill graph analysis and scalable AWS infrastructure.

---

## 10. Innovation Highlights
- Dynamic skill graph engine that models careers as interconnected skill networks
- AI-driven skill-gap detection using graph-based analysis
- Skill priority ranking based on importance, dependency, and market demand
- Job-market-aware skill comparison using role-based datasets
- Multilingual career guidance for regional language users
- Low-bandwidth, text-first interface for broader accessibility
- Scalable cloud-based architecture using AWS serverless services
