<style>
.tech-stack-wrapper {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  max-width: 1000px;
  margin: 0 auto;
  padding: 20px 0;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}
@media (max-width: 768px) {
  .tech-stack-wrapper {
    grid-template-columns: 1fr;
  }
}
.tech-card {
  background: #111827;
  border: 1px solid #1e293b;
  border-left: 4px solid var(--accent);
  border-radius: 12px;
  padding: 24px;
  position: relative;
  display: flex;
  flex-direction: column;
  overflow: hidden;
  opacity: 0;
  animation: fadeUp 0.6s cubic-bezier(0.22, 1, 0.36, 1) forwards;
  transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);
}
.tech-card:nth-child(1) { animation-delay: 0.1s; }
.tech-card:nth-child(2) { animation-delay: 0.15s; }
.tech-card:nth-child(3) { animation-delay: 0.2s; }
.tech-card:nth-child(4) { animation-delay: 0.25s; }
.tech-card:nth-child(5) { animation-delay: 0.3s; }
.tech-card:nth-child(6) { animation-delay: 0.35s; }
.tech-card:nth-child(7) { animation-delay: 0.4s; }
.tech-card:nth-child(8) { animation-delay: 0.45s; }
.tech-card:nth-child(9) { animation-delay: 0.5s; }
.tech-card::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 100%;
  height: 100%;
  background: radial-gradient(circle at 0% 0%, var(--glow) 0%, transparent 70%);
  opacity: 0;
  transition: opacity 0.4s ease;
  pointer-events: none;
}
.tech-card:hover {
  transform: translateY(-8px) scale(1.01);
  border-color: var(--accent);
  box-shadow: 0 20px 40px -10px var(--glow);
}
.tech-card:hover::before {
  opacity: 1;
}
.card-header {
  display: flex;
  align-items: flex-start;
  gap: 16px;
  margin-bottom: 20px;
  position: relative;
  z-index: 1;
}
.card-icon {
  width: 36px;
  height: 36px;
  stroke-width: 2px;
  stroke: var(--accent);
  fill: none;
  flex-shrink: 0;
  animation: float 3s ease-in-out infinite;
}
.card-info {
  display: flex;
  flex-direction: column;
}
.card-subtitle {
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #94a3b8;
  margin-bottom: 4px;
}
.card-title {
  margin: 0;
  font-size: 18px;
  font-weight: 700;
  background: linear-gradient(to right, #ffffff, var(--accent));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.tech-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  position: relative;
  z-index: 1;
  margin-top: auto;
}
.tech-icon {
  width: 34px;
  height: 34px;
  padding: 6px;
  background: #1e293b;
  border-radius: 8px;
  transition: all 0.2s ease;
  border: 1px solid transparent;
}
.tech-card:hover .tech-icon {
  background: #334155;
  border-color: var(--accent);
}
.tech-icon:hover {
  transform: scale(1.25) rotate(-6deg);
  background: #1e293b;
  box-shadow: 0 0 15px var(--glow);
  border-color: var(--accent);
}
.tech-badge {
  display: inline-flex;
  align-items: center;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid #1e293b;
  padding: 5px 10px;
  border-radius: 6px;
  font-size: 11px;
  font-weight: 500;
  color: #cbd5e1;
  transition: all 0.2s;
}
.tech-badge:hover {
  background: var(--accent);
  color: #000;
  border-color: transparent;
  transform: scale(1.05);
  box-shadow: 0 0 12px var(--glow);
}
@keyframes fadeUp {
  0% { opacity: 0; transform: translateY(20px); }
  100% { opacity: 1; transform: translateY(0); }
}
@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-4px); }
}
</style>
<div class="tech-stack-wrapper">
  <div class="tech-card" style="--accent: #8b5cf6; --glow: rgba(139, 92, 246, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M12 4a4 4 0 1 0 0 8 4 4 0 0 0 0-8Zm0 0v2m0 8v2M8 6H6a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h4m6-12h2a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-4M9 18v-2a3 3 0 0 1 6 0v2"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Artificial Intelligence</span>
        <h3 class="card-title">AI Engineering</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/python" class="tech-icon" title="Python"/>
      <img src="https://cdn.simpleicons.org/numpy" class="tech-icon" title="NumPy"/>
      <img src="https://cdn.simpleicons.org/pandas" class="tech-icon" title="Pandas"/>
      <img src="https://cdn.simpleicons.org/scikitlearn" class="tech-icon" title="Scikit-learn"/>
      <img src="https://cdn.simpleicons.org/tensorflow" class="tech-icon" title="TensorFlow"/>
      <img src="https://cdn.simpleicons.org/pytorch" class="tech-icon" title="PyTorch"/>
      <img src="https://cdn.simpleicons.org/xgboost" class="tech-icon" title="XGBoost"/>
      <img src="https://cdn.simpleicons.org/lightgbm" class="tech-icon" title="LightGBM"/>
      <img src="https://cdn.simpleicons.org/catboost" class="tech-icon" title="CatBoost"/>
      <img src="https://cdn.simpleicons.org/opencv" class="tech-icon" title="OpenCV"/>
      <img src="https://cdn.simpleicons.org/mlflow" class="tech-icon" title="MLflow"/>
      <img src="https://cdn.simpleicons.org/wandb" class="tech-icon" title="Weights & Biases"/>
      <span class="tech-badge">Feature Eng</span>
      <span class="tech-badge">Data Prep</span>
      <span class="tech-badge">Model Training</span>
      <span class="tech-badge">Model Eval</span>
    </div>
  </div>
  <div class="tech-card" style="--accent: #06b6d4; --glow: rgba(6, 182, 212, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M15 14c.2-1 .7-1.6 1.5-2 .5-.2 1-.2 1.5 0 .7.4.9 1.3.5 2-.3.6-1 1.1-1.5 1.2a6.5 6.5 0 0 1-.7 3.7M9 18a6.5 6.5 0 0 1-4.5-11 2.5 2.5 0 0 1 4.3 1.5M9 18c0 1 .5 1.5 1.5 1.5S12 19 12 18m-8-5h16"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Large Language Models</span>
        <h3 class="card-title">Generative AI & LLMs</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/openai" class="tech-icon" title="OpenAI"/>
      <img src="https://cdn.simpleicons.org/anthropic" class="tech-icon" title="Claude"/>
      <img src="https://cdn.simpleicons.org/googlegemini" class="tech-icon" title="Gemini"/>
      <img src="https://cdn.simpleicons.org/mistral" class="tech-icon" title="Mistral"/>
      <img src="https://cdn.simpleicons.org/meta" class="tech-icon" title="Llama"/>
      <img src="https://cdn.simpleicons.org/huggingface" class="tech-icon" title="Hugging Face"/>
      <img src="https://cdn.simpleicons.org/langchain" class="tech-icon" title="LangChain"/>
      <img src="https://cdn.simpleicons.org/ollama" class="tech-icon" title="Ollama"/>
      <img src="https://cdn.simpleicons.org/llamaindex" class="tech-icon" title="LlamaIndex"/>
      <img src="https://cdn.simpleicons.org/dspy" class="tech-icon" title="DSPy"/>
      <img src="https://cdn.simpleicons.org/haystack" class="tech-icon" title="Haystack"/>
      <span class="tech-badge">Prompt Eng</span>
      <span class="tech-badge">RAG</span>
      <span class="tech-badge">Fine-Tuning</span>
      <span class="tech-badge">Embeddings</span>
    </div>
  </div>
  <div class="tech-card" style="--accent: #ec4899; --glow: rgba(236, 72, 153, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M9 6a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM5 20a3 3 0 1 1 6 0 3 3 0 0 1-6 0Zm8 0a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM12 9v2m0 6v2M6 12h2m8 0h2"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Autonomous Agents</span>
        <h3 class="card-title">Agentic AI</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/langgraph" class="tech-icon" title="LangGraph"/>
      <img src="https://cdn.simpleicons.org/crewai" class="tech-icon" title="CrewAI"/>
      <img src="https://cdn.simpleicons.org/autogen" class="tech-icon" title="AutoGen"/>
      <img src="https://cdn.simpleicons.org/agno" class="tech-icon" title="Agno (PhiData)"/>
      <img src="https://cdn.simpleicons.org/mcp" class="tech-icon" title="MCP"/>
      <span class="tech-badge">Multi-Agent Sys.</span>
      <span class="tech-badge">AI Agents</span>
      <span class="tech-badge">Tool Calling</span>
      <span class="tech-badge">Agent Memory</span>
      <span class="tech-badge">Orchestration</span>
      <span class="tech-badge">Planning Agents</span>
      <span class="tech-badge">Autonomous Agents</span>
    </div>
  </div>
  <div class="tech-card" style="--accent: #3b82f6; --glow: rgba(59, 130, 246, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="m8 6-6 6 6 6m8 0 6-6-6-6"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Client & Server</span>
        <h3 class="card-title">Full-Stack Development</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/react" class="tech-icon" title="React"/>
      <img src="https://cdn.simpleicons.org/nextdotjs" class="tech-icon" title="Next.js"/>
      <img src="https://cdn.simpleicons.org/typescript" class="tech-icon" title="TypeScript"/>
      <img src="https://cdn.simpleicons.org/javascript" class="tech-icon" title="JavaScript"/>
      <img src="https://cdn.simpleicons.org/html5" class="tech-icon" title="HTML5"/>
      <img src="https://cdn.simpleicons.org/css3" class="tech-icon" title="CSS3"/>
      <img src="https://cdn.simpleicons.org/tailwindcss" class="tech-icon" title="Tailwind CSS"/>
      <img src="https://cdn.simpleicons.org/redux" class="tech-icon" title="Redux"/>
      <img src="https://cdn.simpleicons.org/shadcnui" class="tech-icon" title="Shadcn UI"/>
      <img src="https://cdn.simpleicons.org/framer" class="tech-icon" title="Framer Motion"/>
      <img src="https://cdn.simpleicons.org/vite" class="tech-icon" title="Vite"/>
      <img src="https://cdn.simpleicons.org/nodejs" class="tech-icon" title="Node.js"/>
      <img src="https://cdn.simpleicons.org/express" class="tech-icon" title="Express.js"/>
      <img src="https://cdn.simpleicons.org/fastapi" class="tech-icon" title="FastAPI"/>
      <img src="https://cdn.simpleicons.org/django" class="tech-icon" title="Django"/>
      <img src="https://cdn.simpleicons.org/flask" class="tech-icon" title="Flask"/>
      <span class="tech-badge">REST APIs</span>
      <span class="tech-badge">GraphQL</span>
      <span class="tech-badge">WebSockets</span>
    </div>
  </div>
  <div class="tech-card" style="--accent: #14b8a6; --glow: rgba(20, 184, 166, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M17.5 19H9a7 7 0 1 1 6.7-9.2A5 5 0 0 1 17.5 19Z"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Infrastructure & CI/CD</span>
        <h3 class="card-title">Cloud & DevOps</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/amazonaws" class="tech-icon" title="AWS"/>
      <img src="https://cdn.simpleicons.org/docker" class="tech-icon" title="Docker"/>
      <img src="https://cdn.simpleicons.org/kubernetes" class="tech-icon" title="Kubernetes"/>
      <img src="https://cdn.simpleicons.org/git" class="tech-icon" title="Git"/>
      <img src="https://cdn.simpleicons.org/github" class="tech-icon" title="GitHub"/>
      <img src="https://cdn.simpleicons.org/githubactions" class="tech-icon" title="GitHub Actions"/>
      <img src="https://cdn.simpleicons.org/linux" class="tech-icon" title="Linux"/>
      <img src="https://cdn.simpleicons.org/nginx" class="tech-icon" title="Nginx"/>
      <img src="https://cdn.simpleicons.org/vercel" class="tech-icon" title="Vercel"/>
      <img src="https://cdn.simpleicons.org/railway" class="tech-icon" title="Railway"/>
      <img src="https://cdn.simpleicons.org/render" class="tech-icon" title="Render"/>
      <img src="https://cdn.simpleicons.org/netlify" class="tech-icon" title="Netlify"/>
      <img src="https://cdn.simpleicons.org/digitalocean" class="tech-icon" title="DigitalOcean"/>
    </div>
  </div>
  <div class="tech-card" style="--accent: #f59e0b; --glow: rgba(245, 158, 11, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><ellipse cx="12" cy="5" rx="9" ry="3"/><path d="M3 5v14c0 1.66 4 3 9 3s9-1.34 9-3V5"/><path d="M3 12c0 1.66 4 3 9 3s9-1.34 9-3"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Data Persistence</span>
        <h3 class="card-title">Databases</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/mongodb" class="tech-icon" title="MongoDB"/>
      <img src="https://cdn.simpleicons.org/postgresql" class="tech-icon" title="PostgreSQL"/>
      <img src="https://cdn.simpleicons.org/mysql" class="tech-icon" title="MySQL"/>
      <img src="https://cdn.simpleicons.org/redis" class="tech-icon" title="Redis"/>
      <img src="https://cdn.simpleicons.org/sqlite" class="tech-icon" title="SQLite"/>
      <img src="https://cdn.simpleicons.org/supabase" class="tech-icon" title="Supabase"/>
      <img src="https://cdn.simpleicons.org/firebase" class="tech-icon" title="Firebase"/>
      <img src="https://cdn.simpleicons.org/pinecone" class="tech-icon" title="Pinecone"/>
      <img src="https://cdn.simpleicons.org/chromadb" class="tech-icon" title="ChromaDB"/>
      <img src="https://cdn.simpleicons.org/faiss" class="tech-icon" title="FAISS"/>
      <img src="https://cdn.simpleicons.org/weaviate" class="tech-icon" title="Weaviate"/>
      <img src="https://cdn.simpleicons.org/qdrant" class="tech-icon" title="Qdrant"/>
      <img src="https://cdn.simpleicons.org/milvus" class="tech-icon" title="Milvus"/>
    </div>
  </div>
  <div class="tech-card" style="--accent: #10b981; --glow: rgba(16, 185, 129, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><rect x="2" y="6" width="6" height="4"/><path d="M8 10v2a4 4 0 0 0 8 0v-2"/><rect x="16" y="14" width="6" height="4"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Workflow Orchestration</span>
        <h3 class="card-title">Automation</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/n8n" class="tech-icon" title="n8n"/>
      <img src="https://cdn.simpleicons.org/make" class="tech-icon" title="Make"/>
      <img src="https://cdn.simpleicons.org/zapier" class="tech-icon" title="Zapier"/>
      <img src="https://cdn.simpleicons.org/pipedream" class="tech-icon" title="Pipedream"/>
      <img src="https://cdn.simpleicons.org/selenium" class="tech-icon" title="Selenium"/>
      <img src="https://cdn.simpleicons.org/playwright" class="tech-icon" title="Playwright"/>
      <img src="https://cdn.simpleicons.org/puppeteer" class="tech-icon" title="Puppeteer"/>
      <span class="tech-badge">Browser Auto.</span>
      <span class="tech-badge">API Int.</span>
      <span class="tech-badge">Webhooks</span>
      <span class="tech-badge">Cron Jobs</span>
      <span class="tech-badge">Workflow Auto.</span>
    </div>
  </div>
  <div class="tech-card" style="--accent: #f472b6; --glow: rgba(244, 114, 182, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"/><path d="M3 9h18"/><path d="M9 21V9"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Scalable Applications</span>
        <h3 class="card-title">SaaS Engineering</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/stripe" class="tech-icon" title="Stripe"/>
      <img src="https://cdn.simpleicons.org/razorpay" class="tech-icon" title="Razorpay"/>
      <span class="tech-badge">Multi-Tenant</span>
      <span class="tech-badge">Authentication</span>
      <span class="tech-badge">RBAC</span>
      <span class="tech-badge">Subscriptions</span>
      <span class="tech-badge">Billing</span>
      <span class="tech-badge">User Mgmt</span>
      <span class="tech-badge">Dashboards</span>
      <span class="tech-badge">Email Services</span>
      <span class="tech-badge">Notifications</span>
      <span class="tech-badge">Analytics</span>
    </div>
  </div>
  <div class="tech-card" style="--accent: #64748b; --glow: rgba(100, 116, 139, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.8-3.8a1 1 0 0 0 0-1.4L19.9 3a1 1 0 0 0-1.4 0l-3.8 3.8ZM9.3 17.7a1 1 0 0 0 0-1.4l-1.6-1.6a1 1 0 0 0-1.4 0l-3.8 3.8a1 1 0 0 0 0 1.4L4.1 21a1 1 0 0 0 1.4 0l3.8-3.8ZM5.3 12.4a2 2 0 0 1 0-2.8l4.3-4.3a2 2 0 0 1 2.8 0l4.3 4.3a2 2 0 0 1 0 2.8l-4.3 4.3a2 2 0 0 1-2.8 0l-4.3-4.3Z"/></svg>
      <div class="card-info">
        <span class="card-subtitle">Productivity Suite</span>
        <h3 class="card-title">Developer Toolkit</h3>
      </div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.simpleicons.org/python" class="tech-icon" title="Python"/>
      <img src="https://cdn.simpleicons.org/typescript" class="tech-icon" title="TypeScript"/>
      <img src="https://cdn.simpleicons.org/javascript" class="tech-icon" title="JavaScript"/>
      <img src="https://cdn.simpleicons.org/java" class="tech-icon" title="Java"/>
      <img src="https://cdn.simpleicons.org/c" class="tech-icon" title="C"/>
      <img src="https://cdn.simpleicons.org/cplusplus" class="tech-icon" title="C++"/>
      <img src="https://cdn.simpleicons.org/sqlite" class="tech-icon" title="SQL"/>
      <img src="https://cdn.simpleicons.org/gnubash" class="tech-icon" title="Bash"/>
      <img src="https://cdn.simpleicons.org/visualstudiocode" class="tech-icon" title="VS Code"/>
      <img src="https://cdn.simpleicons.org/github" class="tech-icon" title="GitHub"/>
      <img src="https://cdn.simpleicons.org/postman" class="tech-icon" title="Postman"/>
      <img src="https://cdn.simpleicons.org/docker" class="tech-icon" title="Docker Desktop"/>
      <img src="https://cdn.simpleicons.org/figma" class="tech-icon" title="Figma"/>
      <img src="https://cdn.simpleicons.org/notion" class="tech-icon" title="Notion"/>
      <img src="https://cdn.simpleicons.org/jira" class="tech-icon" title="Jira"/>
    </div>
  </div>
</div>
