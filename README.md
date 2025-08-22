WisdomArc
License: MIT
React
Node.js

An innovative Agentic AI-powered philosophical companion that transforms conversations into interactive learning experiences through transparent chain-of-thought reasoning and multi-agent collaboration.

🌟 Features
Core Capabilities
🤖 Multi-Agent Architecture: Specialized philosopher agents (Socrates, Lao Tzu, Marcus Aurelius) collaborate transparently

🔍 Visible Chain-of-Thought: Step-by-step reasoning processes visible to users

🎭 Dynamic Persona Selection: Choose from various philosophical guides and emotional tones

🌍 Cross-Cultural Synthesis: Default philosopher that combines wisdom from multiple traditions

💡 Explainable AI: Interactive explanations revealing individual agent contributions

🎨 Modern Interactive UI: Flashy animations, responsive design, and dynamic avatars

Advanced Features
🗣️ Voice Support: Text-to-speech and speech-to-text capabilities

🌐 Multilingual: Automatic language detection and translation

📱 Mobile Responsive: Optimized for all device sizes

🧠 Metacognitive Learning: Models effective problem-solving techniques

🚀 Getting Started
Prerequisites
Node.js (v16.0 or higher)

npm or yarn package manager

Modern web browser

Installation
Clone the repository

bash
git clone https://github.com/yourusername/wisdomarc.git
cd wisdomarc
Install dependencies

bash
npm install
Set up environment variables

bash
cp .env.example .env
Edit .env file with your API keys and configuration:

text
REACT_APP_API_BASE_URL=your_backend_url
REACT_APP_OPENAI_API_KEY=your_openai_key
REACT_APP_CREWAI_API_KEY=your_crewai_key
Start the development server

bash
npm start
Open your browser
Navigate to http://localhost:3000

🏗️ Project Structure
text
wisdomarc/
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── Chatbot.js          # Main chatbot component
│   │   ├── AgentVisualization/ # Agent activity indicators
│   │   ├── ChainOfThought/     # Reasoning display components
│   │   └── PersonaSelector/    # Philosopher selection UI
│   ├── agents/
│   │   ├── SocratesAgent.js    # Socratic questioning agent
│   │   ├── LaoTzuAgent.js      # Taoist wisdom agent
│   │   ├── StoicAgent.js       # Stoic philosophy agent
│   │   └── CoordinatorAgent.js # Multi-agent coordinator
│   ├── services/
│   │   ├── api.js              # Backend API integration
│   │   ├── agenticFramework.js # CrewAI integration
│   │   └── speechService.js    # Voice capabilities
│   ├── utils/
│   │   ├── chainOfThought.js   # Reasoning utilities
│   │   └── philosophyEngine.js # Cross-cultural synthesis
│   ├── styles/
│   │   └── main.css            # Global styles
│   ├── App.js
│   └── index.js
├── .env.example
├── .gitignore
├── package.json
└── README.md
🤖 Agentic AI Architecture
WisdomArc employs a sophisticated multi-agent system built on the CrewAI framework:

Philosopher Agents
Socrates Agent: Specializes in questioning and self-discovery

Lao Tzu Agent: Provides flowing, natural wisdom

Marcus Aurelius Agent: Offers stoic resilience and practical philosophy

Buddha Agent: Focuses on mindfulness and compassion

Default Synthesis Agent: Combines insights from multiple traditions

Agent Collaboration
text
graph TD
    A[User Query] --> B[Coordinator Agent]
    B --> C[Socrates Agent]
    B --> D[Lao Tzu Agent]
    B --> E[Stoic Agent]
    C --> F[Response Synthesis]
    D --> F
    E --> F
    F --> G[Chain-of-Thought Display]
    G --> H[User Response]
🔧 Configuration
Environment Variables
bash
# API Configuration
REACT_APP_API_BASE_URL=http://localhost:3001
REACT_APP_OPENAI_API_KEY=your_openai_api_key

# Agentic AI Configuration
REACT_APP_CREWAI_API_KEY=your_crewai_api_key
REACT_APP_AGENT_TIMEOUT=30000

# Feature Flags
REACT_APP_ENABLE_VOICE=true
REACT_APP_ENABLE_MULTILINGUAL=true
REACT_APP_DEBUG_AGENTS=false
Persona Configuration
Customize available philosophers in src/config/personas.js:

javascript
export const personas = [
  {
    id: 'socrates',
    name: 'Socrates',
    description: 'Ancient Greek philosopher focused on self-knowledge',
    agent: 'SocratesAgent',
    mood: ['thoughtful', 'questioning']
  },
  // Add more personas...
];
🎯 Usage Examples
Basic Conversation
javascript
// Ask a philosophical question
"I'm feeling lost in life. What should I do?"

// WisdomArc Response with Chain-of-Thought:
// 1. Analyzing your emotional state...
// 2. Consulting Stoic principles...
// 3. Integrating Buddhist mindfulness...
// 4. Synthesizing perspectives...
// Result: [Comprehensive guidance with visible reasoning]
Persona Selection
javascript
// Select specific philosopher
setSelectedPersona('socrates');
// Result: Responses will follow Socratic questioning method

// Or let the system choose automatically
setPersona('auto');
// Result: AI selects best philosopher based on context
🧪 Testing
Run Tests
bash
npm test
Test Coverage
bash
npm run test:coverage
E2E Testing
bash
npm run test:e2e
🚀 Deployment
Build for Production
bash
npm run build
Deploy to Vercel
bash
npm install -g vercel
vercel
Deploy to Netlify
bash
npm run build
# Upload dist/ folder to Netlify
🤝 Contributing
We welcome contributions to WisdomArc! Please read our Contributing Guidelines for details.

Development Workflow
Fork the repository

Create a feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

Code Style
Use ESLint and Prettier for code formatting

Follow React best practices

Write meaningful commit messages

Add tests for new features

📈 Roadmap
Phase 1 (Current)
 Basic multi-agent architecture

 Chain-of-thought reasoning

 React frontend with persona selection

 Voice integration

 Multilingual support

Phase 2 (Next)
 Advanced emotion detection

 Learning from conversations

 Mobile app development

 Integration with meditation apps

Phase 3 (Future)
 VR/AR philosophical experiences

 Educational institution partnerships

 Enterprise wellness integration

 Research publication platform

📊 Performance
Response Time: < 2 seconds for complex philosophical queries

Agent Coordination: Parallel processing with < 500ms overhead

UI Responsiveness: 60fps animations on modern devices

Memory Usage: < 100MB typical session

🔒 Privacy & Security
Data Protection: No personal conversations stored permanently

API Security: All external API calls encrypted

User Privacy: Optional anonymous mode available

GDPR Compliant: Data deletion on request

📚 Documentation
API Documentation

Agent Development Guide

Philosophy Integration

Deployment Guide

🐛 Troubleshooting
Common Issues
Agent not responding:

bash
# Check agent configuration
npm run debug:agents

# Verify API keys
npm run verify:config
Build errors:

bash
# Clear cache
npm run clean
npm install
Voice features not working:

bash
# Check browser permissions
# Ensure HTTPS in production
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

👥 Team
Lead Developer: Your Name

Philosophy Consultant: [Consultant Name]

UI/UX Designer: [Designer Name]

🙏 Acknowledgments
CrewAI Framework for multi-agent architecture

OpenAI for language model capabilities

Ancient philosophers whose wisdom inspires this project

Open source community for tools and inspiration

📞 Support
Documentation: docs.wisdomarc.com

Issues: GitHub Issues

Discussions: GitHub Discussions

Email: support@wisdomarc.com

"The unexamined life is not worth living." - Socrates

WisdomArc: Where Ancient Wisdom Meets Modern AI ✨
