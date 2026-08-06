<style>
  /* Grid Layout and Font */
  .tech-stack-wrapper {
    display: grid !important;
    grid-template-columns: repeat(3, 1fr) !important;
    gap: 20px !important;
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  }
  @media (max-width: 768px) {
    .tech-stack-wrapper { grid-template-columns: 1fr !important; }
  }

  /* Animated Cards */
  .tech-card {
    background: #111827;
    border: 1px solid #1e293b;
    border-left: 4px solid var(--accent);
    border-radius: 12px;
    padding: 24px;
    position: relative;
    display: flex;
    flex-direction: column;
    opacity: 0;
    animation: fadeUp 0.6s cubic-bezier(0.22, 1, 0.36, 1) forwards;
    transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  }

  /* Staggered Delays */
  .tech-card:nth-child(1) { animation-delay: 0.1s; }
  .tech-card:nth-child(2) { animation-delay: 0.15s; }
  .tech-card:nth-child(3) { animation-delay: 0.2s; }
  .tech-card:nth-child(4) { animation-delay: 0.25s; }
  .tech-card:nth-child(5) { animation-delay: 0.3s; }
  .tech-card:nth-child(6) { animation-delay: 0.35s; }
  .tech-card:nth-child(7) { animation-delay: 0.4s; }
  .tech-card:nth-child(8) { animation-delay: 0.45s; }
  .tech-card:nth-child(9) { animation-delay: 0.5s; }

  /* Glow Effect on Hover */
  .tech-card::before {
    content: "";
    position: absolute;
    top: -50%; left: -50%; width: 100%; height: 100%;
    background: radial-gradient(circle at 0% 0%, var(--glow) 0%, transparent 70%);
    opacity: 0;
    transition: opacity 0.4s ease;
    pointer-events: none;
  }
  .tech-card:hover {
    transform: translateY(-8px) scale(1.01);
    border-color: var(--accent);
    box-shadow: 0 20px 40px -10px var(--glow) !important;
  }
  .tech-card:hover::before { opacity: 1; }

  /* Header Section */
  .card-header { display: flex; align-items: flex-start; gap: 16px; margin-bottom: 20px; position: relative; z-index: 1; }
  .card-icon { width: 36px; height: 36px; stroke-width: 2px; stroke: var(--accent); fill: none; flex-shrink: 0; animation: float 3s ease-in-out infinite; }
  .card-info { display: flex; flex-direction: column; }
  .card-subtitle { font-size: 11px; font-weight: 600; letter-spacing: 1px; text-transform: uppercase; color: #94a3b8; margin-bottom: 4px; }
  .card-title { margin: 0; font-size: 18px; font-weight: 700; background: linear-gradient(to right, #ffffff, var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

  /* Tech Grid */
  .tech-grid { display: flex; flex-wrap: wrap; gap: 8px; position: relative; z-index: 1; margin-top: auto; }
  .tech-icon { width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; transition: all 0.2s ease; border: 1px solid transparent; }
  .tech-card:hover .tech-icon { background: #334155; border-color: var(--accent); }
  .tech-icon:hover { transform: scale(1.25) rotate(-6deg); background: #1e293b; box-shadow: 0 0 15px var(--glow); border-color: var(--accent); }
  .tech-badge { display: inline-flex; align-items: center; background: rgba(255, 255, 255, 0.05); border: 1px solid #1e293b; padding: 5px 10px; border-radius: 6px; font-size: 11px; font-weight: 500; color: #cbd5e1; transition: all 0.2s; }
  .tech-badge:hover { background: var(--accent); color: #000; border-color: transparent; transform: scale(1.05); box-shadow: 0 0 12px var(--glow); }

  /* Animations */
  @keyframes fadeUp { 0% { opacity: 0; transform: translateY(20px); } 100% { opacity: 1; transform: translateY(0); } }
  @keyframes float { 0%, 100% { transform: translateY(0px); } 50% { transform: translateY(-4px); } }
</style>

<div class="tech-stack-wrapper">
  <!-- Card 1: AI Engineering -->
  <div class="tech-card" style="--accent: #8b5cf6; --glow: rgba(139, 92, 246, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M12 4a4 4 0 1 0 0 8 4 4 0 0 0 0-8Zm0 0v2m0 8v2M8 6H6a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h4m6-12h2a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-4M9 18v-2a3 3 0 0 1 6 0v2"/></svg>
      <div class="card-info"><span class="card-subtitle">Artificial Intelligence</span><h3 class="card-title">AI Engineering</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" class="tech-icon" title="Python"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" class="tech-icon" title="NumPy"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" class="tech-icon" title="Pandas"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/scikitlearn/scikitlearn-original.svg" class="tech-icon" title="Scikit-learn"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" class="tech-icon" title="TensorFlow"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pytorch/pytorch-original.svg" class="tech-icon" title="PyTorch"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/opencv/opencv-original.svg" class="tech-icon" title="OpenCV"/>
      <span class="tech-badge">XGBoost</span><span class="tech-badge">LightGBM</span><span class="tech-badge">CatBoost</span>
    </div>
  </div>

  <!-- Card 2: Gen AI & LLMs -->
  <div class="tech-card" style="--accent: #06b6d4; --glow: rgba(6, 182, 212, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M15 14c.2-1 .7-1.6 1.5-2 .5-.2 1-.2 1.5 0 .7.4.9 1.3.5 2-.3.6-1 1.1-1.5 1.2a6.5 6.5 0 0 1-.7 3.7M9 18a6.5 6.5 0 0 1-4.5-11 2.5 2.5 0 0 1 4.3 1.5M9 18c0 1 .5 1.5 1.5 1.5S12 19 12 18m-8-5h16"/></svg>
      <div class="card-info"><span class="card-subtitle">Large Language Models</span><h3 class="card-title">Generative AI & LLMs</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/openai/openai-original.svg" class="tech-icon" title="OpenAI"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/anthropic/anthropic-original.svg" class="tech-icon" title="Claude"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/langchain/langchain-original.svg" class="tech-icon" title="LangChain"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ollama/ollama-original.svg" class="tech-icon" title="Ollama"/>
      <span class="tech-badge">Gemini</span><span class="tech-badge">Mistral</span><span class="tech-badge">Llama</span><span class="tech-badge">RAG</span><span class="tech-badge">Fine-Tuning</span><span class="tech-badge">Prompt Eng</span>
    </div>
  </div>

  <!-- Card 3: Agentic AI -->
  <div class="tech-card" style="--accent: #ec4899; --glow: rgba(236, 72, 153, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M9 6a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM5 20a3 3 0 1 1 6 0 3 3 0 0 1-6 0Zm8 0a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM12 9v2m0 6v2M6 12h2m8 0h2"/></svg>
      <div class="card-info"><span class="card-subtitle">Autonomous Agents</span><h3 class="card-title">Agentic AI</h3></div>
    </div>
    <div class="tech-grid">
      <span class="tech-badge">LangGraph</span><span class="tech-badge">CrewAI</span><span class="tech-badge">AutoGen</span><span class="tech-badge">Agno</span>
      <span class="tech-badge">Multi-Agent</span><span class="tech-badge">Tool Calling</span><span class="tech-badge">Orchestration</span>
    </div>
  </div>

  <!-- Card 4: Full-Stack -->
  <div class="tech-card" style="--accent: #3b82f6; --glow: rgba(59, 130, 246, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="m8 6-6 6 6 6m8 0 6-6-6-6"/></svg>
      <div class="card-info"><span class="card-subtitle">Client & Server</span><h3 class="card-title">Full-Stack Development</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" class="tech-icon" title="React"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" class="tech-icon" title="Next.js"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" class="tech-icon" title="TypeScript"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" class="tech-icon" title="Node.js"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg" class="tech-icon" title="Django"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/fastapi/fastapi-original.svg" class="tech-icon" title="FastAPI"/>
      <span class="tech-badge">GraphQL</span><span class="tech-badge">REST APIs</span>
    </div>
  </div>

  <!-- Card 5: Cloud & DevOps -->
  <div class="tech-card" style="--accent: #14b8a6; --glow: rgba(20, 184, 166, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M17.5 19H9a7 7 0 1 1 6.7-9.2A5 5 0 0 1 17.5 19Z"/></svg>
      <div class="card-info"><span class="card-subtitle">Infrastructure & CI/CD</span><h3 class="card-title">Cloud & DevOps</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" class="tech-icon" title="AWS"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" class="tech-icon" title="Docker"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kubernetes/kubernetes-original.svg" class="tech-icon" title="K8s"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/githubactions/githubactions-original.svg" class="tech-icon" title="GitHub Actions"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nginx/nginx-original.svg" class="tech-icon" title="Nginx"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vercel/vercel-original.svg" class="tech-icon" title="Vercel"/>
    </div>
  </div>

  <!-- Card 6: Databases -->
  <div class="tech-card" style="--accent: #f59e0b; --glow: rgba(245, 158, 11, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><ellipse cx="12" cy="5" rx="9" ry="3"/><path d="M3 5v14c0 1.66 4 3 9 3s9-1.34 9-3V5"/><path d="M3 12c0 1.66 4 3 9 3s9-1.34 9-3"/></svg>
      <div class="card-info"><span class="card-subtitle">Data Persistence</span><h3 class="card-title">Databases</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" class="tech-icon" title="MongoDB"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" class="tech-icon" title="PostgreSQL"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" class="tech-icon" title="MySQL"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg" class="tech-icon" title="Redis"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/supabase/supabase-original.svg" class="tech-icon" title="Supabase"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" class="tech-icon" title="Firebase"/>
    </div>
  </div>

  <!-- Card 7: Automation -->
  <div class="tech-card" style="--accent: #10b981; --glow: rgba(16, 185, 129, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><rect x="2" y="6" width="6" height="4"/><path d="M8 10v2a4 4 0 0 0 8 0v-2"/><rect x="16" y="14" width="6" height="4"/></svg>
      <div class="card-info"><span class="card-subtitle">Workflow Orchestration</span><h3 class="card-title">Automation</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/n8n/n8n-original.svg" class="tech-icon" title="n8n"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/zapier/zapier-original.svg" class="tech-icon" title="Zapier"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/selenium/selenium-original.svg" class="tech-icon" title="Selenium"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/playwright/playwright-original.svg" class="tech-icon" title="Playwright"/>
      <span class="tech-badge">Webhooks</span><span class="tech-badge">Cron Jobs</span>
    </div>
  </div>

  <!-- Card 8: SaaS Engineering -->
  <div class="tech-card" style="--accent: #f472b6; --glow: rgba(244, 114, 182, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"/><path d="M3 9h18"/><path d="M9 21V9"/></svg>
      <div class="card-info"><span class="card-subtitle">Scalable Applications</span><h3 class="card-title">SaaS Engineering</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/stripe/stripe-original.svg" class="tech-icon" title="Stripe"/>
      <span class="tech-badge">Multi-Tenant</span><span class="tech-badge">Auth</span><span class="tech-badge">RBAC</span><span class="tech-badge">Subscriptions</span><span class="tech-badge">Dashboards</span>
    </div>
  </div>

  <!-- Card 9: Toolkit -->
  <div class="tech-card" style="--accent: #64748b; --glow: rgba(100, 116, 139, 0.4);">
    <div class="card-header">
      <svg class="card-icon" viewBox="0 0 24 24"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.8-3.8a1 1 0 0 0 0-1.4L19.9 3a1 1 0 0 0-1.4 0l-3.8 3.8ZM9.3 17.7a1 1 0 0 0 0-1.4l-1.6-1.6a1 1 0 0 0-1.4 0l-3.8 3.8a1 1 0 0 0 0 1.4L4.1 21a1 1 0 0 0 1.4 0l3.8-3.8ZM5.3 12.4a2 2 0 0 1 0-2.8l4.3-4.3a2 2 0 0 1 2.8 0l4.3 4.3a2 2 0 0 1 0 2.8l-4.3 4.3a2 2 0 0 1-2.8 0l-4.3-4.3Z"/></svg>
      <div class="card-info"><span class="card-subtitle">Productivity Suite</span><h3 class="card-title">Developer Toolkit</h3></div>
    </div>
    <div class="tech-grid">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" class="tech-icon" title="VS Code"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" class="tech-icon" title="GitHub"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postman/postman-original.svg" class="tech-icon" title="Postman"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg" class="tech-icon" title="Figma"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/notion/notion-original.svg" class="tech-icon" title="Notion"/>
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jira/jira-original.svg" class="tech-icon" title="Jira"/>
    </div>
  </div>
</div>
<style>
  @keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-4px); }
  }
</style>
<div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; max-width: 1000px; margin: 0 auto; padding: 20px 0; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;">
  <!-- CARD 1: AI Engineering -->
  <div style="background: #111827; border: 1px solid #1e293b; border-left: 4px solid #8b5cf6; border-radius: 12px; padding: 24px; position: relative; display: flex; flex-direction: column; transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);" onmouseover="this.style.transform='translateY(-8px) scale(1.01)'; this.style.boxShadow='0 20px 40px -10px rgba(139,92,246,0.5)';" onmouseout="this.style.transform='translateY(0px) scale(1)'; this.style.boxShadow='none';">
    <div style="display: flex; align-items: flex-start; gap: 16px; margin-bottom: 20px;">
      <svg style="width: 36px; height: 36px; stroke: #8b5cf6; fill: none; stroke-width: 2px; animation: float 3s ease-in-out infinite;" viewBox="0 0 24 24"><path d="M12 4a4 4 0 1 0 0 8 4 4 0 0 0 0-8Zm0 0v2m0 8v2M8 6H6a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h4m6-12h2a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-4M9 18v-2a3 3 0 0 1 6 0v2"/></svg>
      <div>
        <span style="font-size: 11px; font-weight: 600; letter-spacing: 1px; color: #94a3b8; text-transform: uppercase;">Artificial Intelligence</span>
        <h3 style="margin: 0; font-size: 18px; font-weight: 700; color: #ffffff;">AI Engineering</h3>
      </div>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 8px;">
      <img src="https://cdn.simpleicons.org/python" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/numpy" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/pandas" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/scikitlearn" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/tensorflow" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/pytorch" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/xgboost" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/lightgbm" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/catboost" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/opencv" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/mlflow" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/wandb" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(139,92,246,0.5)'; this.style.borderColor='#8b5cf6';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
    </div>
  </div>

  <!-- CARD 2: Generative AI & LLMs -->
  <div style="background: #111827; border: 1px solid #1e293b; border-left: 4px solid #06b6d4; border-radius: 12px; padding: 24px; position: relative; display: flex; flex-direction: column; transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);" onmouseover="this.style.transform='translateY(-8px) scale(1.01)'; this.style.boxShadow='0 20px 40px -10px rgba(6,182,212,0.5)';" onmouseout="this.style.transform='translateY(0px) scale(1)'; this.style.boxShadow='none';">
    <div style="display: flex; align-items: flex-start; gap: 16px; margin-bottom: 20px;">
      <svg style="width: 36px; height: 36px; stroke: #06b6d4; fill: none; stroke-width: 2px; animation: float 3s ease-in-out infinite;" viewBox="0 0 24 24"><path d="M15 14c.2-1 .7-1.6 1.5-2 .5-.2 1-.2 1.5 0 .7.4.9 1.3.5 2-.3.6-1 1.1-1.5 1.2a6.5 6.5 0 0 1-.7 3.7M9 18a6.5 6.5 0 0 1-4.5-11 2.5 2.5 0 0 1 4.3 1.5M9 18c0 1 .5 1.5 1.5 1.5S12 19 12 18m-8-5h16"/></svg>
      <div>
        <span style="font-size: 11px; font-weight: 600; letter-spacing: 1px; color: #94a3b8; text-transform: uppercase;">Large Language Models</span>
        <h3 style="margin: 0; font-size: 18px; font-weight: 700; color: #ffffff;">Generative AI & LLMs</h3>
      </div>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 8px;">
      <img src="https://cdn.simpleicons.org/openai" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/anthropic" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/googlegemini" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/mistral" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/meta" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/huggingface" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/langchain" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/ollama" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/llamaindex" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/dspy" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/haystack" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(6,182,212,0.5)'; this.style.borderColor='#06b6d4';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
    </div>
  </div>

  <!-- CARD 3: Agentic AI -->
  <div style="background: #111827; border: 1px solid #1e293b; border-left: 4px solid #ec4899; border-radius: 12px; padding: 24px; position: relative; display: flex; flex-direction: column; transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);" onmouseover="this.style.transform='translateY(-8px) scale(1.01)'; this.style.boxShadow='0 20px 40px -10px rgba(236,72,153,0.5)';" onmouseout="this.style.transform='translateY(0px) scale(1)'; this.style.boxShadow='none';">
    <div style="display: flex; align-items: flex-start; gap: 16px; margin-bottom: 20px;">
      <svg style="width: 36px; height: 36px; stroke: #ec4899; fill: none; stroke-width: 2px; animation: float 3s ease-in-out infinite;" viewBox="0 0 24 24"><path d="M9 6a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM5 20a3 3 0 1 1 6 0 3 3 0 0 1-6 0Zm8 0a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM12 9v2m0 6v2M6 12h2m8 0h2"/></svg>
      <div>
        <span style="font-size: 11px; font-weight: 600; letter-spacing: 1px; color: #94a3b8; text-transform: uppercase;">Autonomous Agents</span>
        <h3 style="margin: 0; font-size: 18px; font-weight: 700; color: #ffffff;">Agentic AI</h3>
      </div>
    </div>
    <div style="display: flex; flex-wrap: wrap; gap: 8px;">
      <img src="https://cdn.simpleicons.org/langgraph" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(236,72,153,0.5)'; this.style.borderColor='#ec4899';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/crewai" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(236,72,153,0.5)'; this.style.borderColor='#ec4899';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/autogen" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(236,72,153,0.5)'; this.style.borderColor='#ec4899';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/agno" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(236,72,153,0.5)'; this.style.borderColor='#ec4899';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
      <img src="https://cdn.simpleicons.org/mcp" style="width: 34px; height: 34px; padding: 6px; background: #1e293b; border-radius: 8px; border: 1px solid transparent; transition: all 0.2s;" onmouseover="this.style.transform='scale(1.25) rotate(-6deg)'; this.style.boxShadow='0 0 15px rgba(236,72,153,0.5)'; this.style.borderColor='#ec4899';" onmouseout="this.style.transform='scale(1) rotate(0deg)'; this.style.boxShadow='none'; this.style.borderColor='transparent';"/>
    </div>
  </div>
</div>
<div align="center" style="margin:0; padding:0; line-height:0;">
  <img src="Banner.png" alt="Bannerr" width="100%">
</div>
<p align="center">
  <a href="https://github.com/AbdullahBakir97"><img src="https://komarev.com/ghpvc/?username=AbdullahBakir97&label=PROFILE%20VIEWS&color=F90001&style=for-the-badge&v=20260806" alt="Profile views" /></a>
  <a href="https://github.com/AbdullahBakir97?tab=followers"><img src="https://img.shields.io/github/followers/AbdullahBakir97?label=FOLLOWERS&style=for-the-badge&color=F90001&logo=github&logoColor=white&v=20260806" alt="GitHub followers" /></a>
  <a href="https://github.com/AbdullahBakir97"><img src="https://img.shields.io/github/stars/AbdullahBakir97?affiliations=OWNER&label=TOTAL%20STARS&style=for-the-badge&color=F90001&logo=github&logoColor=white&v=20260806" alt="Total stars" /></a>
  <a href="https://codetime.dev"><img src="https://img.shields.io/endpoint?style=for-the-badge&color=F90001&url=https%3A%2F%2Fapi.codetime.dev%2Fshield%3Fid%3D23432%26project%3D%26in=12096000000&v=20260806" alt="CodeTime hours" /></a>
</p>

<!-- 🏷️ PROFESSIONAL BADGES — contact / availability row -->
<p align="center">
  <a href="mailto:abdullah.bakir.1997@gmail.com"><img src="https://img.shields.io/badge/EMAIL-D44638?style=for-the-badge&logo=gmail&logoColor=white&v=20260806" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/abdullah-bakir-809065273/"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&v=20260806" alt="LinkedIn" /></a>
  <a href="https://t.me/BlackSea0011"><img src="https://img.shields.io/badge/TELEGRAM-26A5E4?style=for-the-badge&logo=telegram&logoColor=white&v=20260806" alt="Telegram" /></a>
  <a href="https://github.com/AbdullahBakir97"><img src="https://img.shields.io/badge/Open_to_Work-00C853?style=for-the-badge&logo=googlechat&logoColor=white&v=20260806" alt="Open to work" /></a>
</p>

<div align="center">
  <img src="./assets/redline.gif" width="100%" alt=""/>
</div>
<p align="center">
  <a href="https://thekeshavgandhi.dev">
    <img src="https://img.shields.io/badge/Portfolio-Visit-blue?style=for-the-badge">
  </a>

  <a href="https://linkedin.com/in/YOUR-LINKEDIN">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge">
  </a>

  <a href="https://youtube.com/@YOURCHANNEL">
    <img src="https://img.shields.io/badge/YouTube-Subscribe-red?style=for-the-badge">
  </a>

  <a href="https://instagram.com/thekeshavgandhi.dev">
    <img src="https://img.shields.io/badge/Instagram-Follow-purple?style=for-the-badge">
  </a>
</p>

---
<h2 id="contributions" align="center">🐍 Contribution Graph</h2>


# 👨‍💻 About Me

```yaml
Name: Keshav Gandhi
Role: Full-Stack Developer & AI Engineer
Location: India 🇮🇳
Company: Techarvel Ltd
Mission: Building impactful AI & SaaS products

Currently Building:
  - AI SaaS Products
  - Startup Ecosystem
  - Full-Stack Applications

Learning:
  - Advanced AI Engineering
  - System Design
  - Cloud Architecture
  - Machine Learning
````

---

# 🚀 Tech Arsenal

### Languages

<p>
<img src="https://skillicons.dev/icons?i=python,javascript,typescript,java,c,cpp,html,css,bash" />
</p>

### Frontend

<p>
<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,vite,redux" />
</p>

### Backend

<p>
<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi,django" />
</p>

### Mobile

<p>
<img src="https://skillicons.dev/icons?i=flutter,react" />
</p>

### AI / ML

<p>
<img src="https://skillicons.dev/icons?i=python,tensorflow,pytorch" />
</p>

* Machine Learning
* Deep Learning
* LLMs
* Prompt Engineering
* RAG
* AI Agents
* Computer Vision
* NLP
* Generative AI

### Databases

<p>
<img src="https://skillicons.dev/icons?i=mongodb,mysql,postgresql,firebase,supabase" />
</p>

### Cloud & DevOps

<p>
<img src="https://skillicons.dev/icons?i=aws,docker,linux,git,github,vercel,netlify" />
</p>

---

# 🧠 AI Stack

✔ OpenAI

✔ Claude

✔ Gemini

✔ LangChain

✔ CrewAI

✔ Vector Databases

✔ AI Agents

✔ RAG Systems

✔ Automation Workflows

✔ N8N

✔ MCP

✔ LLM Applications

---

# 🏢 Ventures

### 🚀 Techarvel Ltd

Building innovative technology products.

### 🧪 Techarvel Labs

Research, AI & Innovation.

### 🎬 Techarvel Studios

Digital Experiences & Product Design.

---

# 🌐 Connect With Me

<p align="center">

<a href="YOUR-LINKEDIN">
LinkedIn
</a> •

<a href="YOUR-PORTFOLIO">
Portfolio
</a> •

<a href="YOUR-YOUTUBE">
YouTube
</a> •

<a href="YOUR-INSTAGRAM">
Instagram
</a> •

<a href="YOUR-TWITTER">
Twitter/X
</a> •

<a href="YOUR-KAGGLE">
Kaggle
</a> •

<a href="YOUR-DEVTO">
Dev.to
</a> •

<a href="YOUR-MEDIUM">
Medium
</a>

</p>

---

# 📈 GitHub Analytics

<p align="center">
<img src="https://github-readme-stats.vercel.app/api?username=YOURUSERNAME&show_icons=true&theme=tokyonight" />
</p>

<p align="center">
<img src="https://github-readme-streak-stats.herokuapp.com/?user=YOURUSERNAME&theme=tokyonight" />
</p>

<p align="center">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOURUSERNAME&layout=compact&theme=tokyonight" />
</p>

---

# 🏆 GitHub Trophies

<p align="center">
<img src="https://github-profile-trophy.vercel.app/?username=YOURUSERNAME&theme=algolia&column=4" />
</p>

---

# 🐍 Contribution Snake

<p align="center">
<img src="https://raw.githubusercontent.com/YOURUSERNAME/YOURUSERNAME/output/github-contribution-grid-snake.svg" />
</p>

---

# 🎮 Fun Zone

### Coding Mood

```text
☕ Coffee → Code → Build → Deploy → Repeat
```

### Current Status

```text
Building the future with AI.
```

### Random Dev Quote

> First solve the problem.
> Then write the code.

---

# 💡 Vision

Building India's next generation AI-first technology company.

⭐ If you like my work, follow my journey.


Dono profiles ka positioning alag rakhega to personal brand zyada strong lagega.
```
