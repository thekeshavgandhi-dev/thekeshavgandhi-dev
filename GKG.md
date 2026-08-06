<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 960 1330" width="100%" height="100%" style="background: transparent;">
  <defs>
    <!-- Pulsing Glow Filter -->
    <filter id="neonGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="8" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>

    <!-- Interactive Shimmer/Border Effect -->
    <linearGradient id="shimmer" x1="-100%" y1="-100%" x2="200%" y2="200%">
      <stop offset="0%" stop-color="currentColor" stop-opacity="0" />
      <stop offset="40%" stop-color="currentColor" stop-opacity="0.7">
        <animate attributeName="offset" values="-100%;100%" dur="4s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="currentColor" stop-opacity="0" />
    </linearGradient>

    <!-- Base Card Background Template -->
    <g id="card-bg">
      <!-- Deep Dark Card Base -->
      <rect width="300" height="420" rx="16" fill="#111827" stroke="#1e293b" stroke-width="1.5" />
      <!-- Left Accent Border -->
      <rect x="0" y="0" width="4" height="420" rx="2" fill="currentColor" />
      <!-- Pulsing Background Glow -->
      <circle cx="150" cy="200" r="80" fill="currentColor" opacity="0.1" filter="url(#neonGlow)">
        <animate attributeName="opacity" values="0.1;0.4;0.1" dur="3s" repeatCount="indefinite" />
        <animate attributeName="r" values="80;110;80" dur="3s" repeatCount="indefinite" />
      </circle>
      <!-- Shimmering Border Stroke on Hover/Always -->
      <rect width="300" height="420" rx="16" fill="none" stroke="url(#shimmer)" stroke-width="2" opacity="0.8" />
    </g>
  </defs>

  <!-- ================= CARD 1: AI ENGINEERING ================= -->
  <g transform="translate(0, 0)" style="color: #8b5cf6;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.1s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.1s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <!-- Card Header -->
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="4s" repeatCount="indefinite" />
            <path d="M12 4a4 4 0 1 0 0 8 4 4 0 0 0 0-8Zm0 0v2m0 8v2M8 6H6a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h4m6-12h2a2 2 0 0 1 2 2v10a2 2 0 0 1-2 2h-4M9 18v-2a3 3 0 0 1 6 0v2" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Artificial Intelligence</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">AI Engineering</text>
        </g>
        <!-- Tech Logos -->
        <g>
          <image href="https://cdn.simpleicons.org/python" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/numpy" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/pandas" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/scikitlearn" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/tensorflow" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/pytorch" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/xgboost" x="30" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/lightgbm" x="72" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/catboost" x="114" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/opencv" x="156" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/mlflow" x="198" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/wandb" x="240" y="132" width="32" height="32" />
        </g>
        <!-- Badges -->
        <g>
          <rect x="30" y="180" width="84" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="72" y="196" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Feature Eng</text>
          
          <rect x="122" y="180" width="74" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="159" y="196" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Data Prep</text>
          
          <rect x="204" y="180" width="94" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="251" y="196" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Model Training</text>
          
          <rect x="30" y="212" width="82" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="71" y="228" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Model Eval</text>
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 2: GEN AI & LLMs ================= -->
  <g transform="translate(330, 0)" style="color: #06b6d4;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.15s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.15s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="3.5s" repeatCount="indefinite" />
            <path d="M15 14c.2-1 .7-1.6 1.5-2 .5-.2 1-.2 1.5 0 .7.4.9 1.3.5 2-.3.6-1 1.1-1.5 1.2a6.5 6.5 0 0 1-.7 3.7M9 18a6.5 6.5 0 0 1-4.5-11 2.5 2.5 0 0 1 4.3 1.5M9 18c0 1 .5 1.5 1.5 1.5S12 19 12 18m-8-5h16" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Large Language Models</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Generative AI & LLMs</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/openai" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/anthropic" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/googlegemini" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/mistral" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/meta" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/huggingface" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/langchain" x="30" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/ollama" x="72" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/llamaindex" x="114" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/dspy" x="156" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/haystack" x="198" y="132" width="32" height="32" />
        </g>
        <g>
          <rect x="30" y="180" width="86" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="73" y="196" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Prompt Eng</text>
          
          <rect x="124" y="180" width="52" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="150" y="196" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">RAG</text>
          
          <rect x="184" y="180" width="90" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="229" y="196" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Fine-Tuning</text>
          
          <rect x="30" y="212" width="84" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="72" y="228" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Embeddings</text>
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 3: AGENTIC AI ================= -->
  <g transform="translate(660, 0)" style="color: #ec4899;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.2s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.2s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="4.5s" repeatCount="indefinite" />
            <path d="M9 6a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM5 20a3 3 0 1 1 6 0 3 3 0 0 1-6 0Zm8 0a3 3 0 1 1 6 0 3 3 0 0 1-6 0ZM12 9v2m0 6v2M6 12h2m8 0h2" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Autonomous Agents</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Agentic AI</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/langgraph" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/crewai" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/autogen" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/agno" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/mcp" x="198" y="90" width="32" height="32" />
        </g>
        <g>
          <rect x="30" y="132" width="114" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="87" y="148" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Multi-Agent Sys.</text>
          
          <rect x="152" y="132" width="76" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="190" y="148" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">AI Agents</text>
          
          <rect x="30" y="164" width="96" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="78" y="180" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Tool Calling</text>
          
          <rect x="134" y="164" width="104" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="186" y="180" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Agent Memory</text>
          
          <rect x="30" y="196" width="104" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="82" y="212" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Orchestration</text>
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 4: FULL-STACK ================= -->
  <g transform="translate(0, 440)" style="color: #3b82f6;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.25s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.25s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="3s" repeatCount="indefinite" />
            <path d="m8 6-6 6 6 6m8 0 6-6-6-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Client & Server</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Full-Stack Dev</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/react" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/nextdotjs" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/typescript" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/javascript" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/html5" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/css3" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/tailwindcss" x="30" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/redux" x="72" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/shadcnui" x="114" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/framer" x="156" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/vite" x="198" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/nodejs" x="240" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/express" x="30" y="174" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/fastapi" x="72" y="174" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/django" x="114" y="174" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/flask" x="156" y="174" width="32" height="32" />
        </g>
        <g>
          <rect x="30" y="220" width="78" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="69" y="236" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">REST APIs</text>
          
          <rect x="116" y="220" width="64" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="148" y="236" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">GraphQL</text>
          
          <rect x="188" y="220" width="86" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="231" y="236" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">WebSockets</text>
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 5: CLOUD & DEVOPS ================= -->
  <g transform="translate(330, 440)" style="color: #14b8a6;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.3s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.3s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="3.8s" repeatCount="indefinite" />
            <path d="M17.5 19H9a7 7 0 1 1 6.7-9.2A5 5 0 0 1 17.5 19Z" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Infra & CI/CD</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Cloud & DevOps</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/amazonaws" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/docker" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/kubernetes" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/git" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/github" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/githubactions" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/linux" x="30" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/nginx" x="72" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/vercel" x="114" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/railway" x="156" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/render" x="198" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/netlify" x="240" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/digitalocean" x="30" y="174" width="32" height="32" />
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 6: DATABASES ================= -->
  <g transform="translate(660, 440)" style="color: #f59e0b;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.35s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.35s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="2.8s" repeatCount="indefinite" />
            <ellipse cx="12" cy="5" rx="9" ry="3" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" /><path d="M3 5v14c0 1.66 4 3 9 3s9-1.34 9-3V5" fill="none" stroke="currentColor" stroke-width="2" /><path d="M3 12c0 1.66 4 3 9 3s9-1.34 9-3" fill="none" stroke="currentColor" stroke-width="2" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Data Persistence</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Databases</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/mongodb" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/postgresql" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/mysql" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/redis" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/sqlite" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/supabase" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/firebase" x="30" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/pinecone" x="72" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/chromadb" x="114" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/faiss" x="156" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/weaviate" x="198" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/qdrant" x="240" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/milvus" x="30" y="174" width="32" height="32" />
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 7: AUTOMATION ================= -->
  <g transform="translate(0, 880)" style="color: #10b981;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.4s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.4s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="5s" repeatCount="indefinite" />
            <rect x="2" y="6" width="6" height="4" fill="none" stroke="currentColor" stroke-width="2" rx="1"/><path d="M8 10v2a4 4 0 0 0 8 0v-2" fill="none" stroke="currentColor" stroke-width="2" /><rect x="16" y="14" width="6" height="4" fill="none" stroke="currentColor" stroke-width="2" rx="1"/>
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Workflow Orchestration</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Automation</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/n8n" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/make" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/zapier" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/pipedream" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/selenium" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/playwright" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/puppeteer" x="30" y="132" width="32" height="32" />
        </g>
        <g>
          <rect x="30" y="174" width="94" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="77" y="190" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Browser Auto.</text>
          
          <rect x="132" y="174" width="58" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="161" y="190" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">API Int.</text>
          
          <rect x="198" y="174" width="78" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="237" y="190" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Webhooks</text>
          
          <rect x="30" y="206" width="78" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="69" y="222" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Cron Jobs</text>
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 8: SAAS ENGINEERING ================= -->
  <g transform="translate(330, 880)" style="color: #f472b6;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.45s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.45s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="3.2s" repeatCount="indefinite" />
            <rect x="3" y="3" width="18" height="18" rx="2" ry="2" fill="none" stroke="currentColor" stroke-width="2"/><path d="M3 9h18" fill="none" stroke="currentColor" stroke-width="2"/><path d="M9 21V9" fill="none" stroke="currentColor" stroke-width="2"/>
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Scalable Apps</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">SaaS Engineering</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/stripe" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/razorpay" x="72" y="90" width="32" height="32" />
        </g>
        <g>
          <rect x="30" y="140" width="86" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="73" y="156" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Multi-Tenant</text>
          
          <rect x="124" y="140" width="100" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="174" y="156" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Authentication</text>
          
          <rect x="30" y="172" width="50" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="55" y="188" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">RBAC</text>
          
          <rect x="88" y="172" width="90" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="133" y="188" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Subscriptions</text>
          
          <rect x="186" y="172" width="58" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="215" y="188" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Billing</text>
          
          <rect x="30" y="204" width="92" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="76" y="220" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">User Mgmt</text>
          
          <rect x="130" y="204" width="84" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="172" y="220" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Dashboards</text>
          
          <rect x="222" y="204" width="56" height="24" rx="6" fill="#ffffff" fill-opacity="0.05" stroke="#1e293b" />
          <text x="250" y="220" fill="#94a3b8" font-size="11" font-weight="500" font-family="sans-serif" text-anchor="middle">Email</text>
        </g>
      </g>
    </g>
  </g>

  <!-- ================= CARD 9: DEVELOPER TOOLKIT ================= -->
  <g transform="translate(660, 880)" style="color: #64748b;">
    <g>
      <animateTransform attributeName="transform" type="translate" from="0 30" to="0 0" begin="0.5s" dur="0.6s" fill="freeze" />
      <g opacity="0"><animate attributeName="opacity" from="0" to="1" begin="0.5s" dur="0.6s" fill="freeze" />
        <use href="#card-bg" />
        <g>
          <g>
            <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="4.2s" repeatCount="indefinite" />
            <path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.8-3.8a1 1 0 0 0 0-1.4L19.9 3a1 1 0 0 0-1.4 0l-3.8 3.8ZM9.3 17.7a1 1 0 0 0 0-1.4l-1.6-1.6a1 1 0 0 0-1.4 0l-3.8 3.8a1 1 0 0 0 0 1.4L4.1 21a1 1 0 0 0 1.4 0l3.8-3.8ZM5.3 12.4a2 2 0 0 1 0-2.8l4.3-4.3a2 2 0 0 1 2.8 0l4.3 4.3a2 2 0 0 1 0 2.8l-4.3 4.3a2 2 0 0 1-2.8 0l-4.3-4.3Z" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" />
          </g>
          <text x="56" y="32" fill="#94a3b8" font-size="11" font-weight="600" font-family="sans-serif" letter-spacing="1" text-transform="uppercase">Productivity Suite</text>
          <text x="56" y="58" fill="#ffffff" font-size="20" font-weight="700" font-family="sans-serif">Developer Toolkit</text>
        </g>
        <g>
          <image href="https://cdn.simpleicons.org/python" x="30" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/typescript" x="72" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/javascript" x="114" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/java" x="156" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/c" x="198" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/cplusplus" x="240" y="90" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/sqlite" x="30" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/gnubash" x="72" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/visualstudiocode" x="114" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/github" x="156" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/postman" x="198" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/docker" x="240" y="132" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/figma" x="30" y="174" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/notion" x="72" y="174" width="32" height="32" />
          <image href="https://cdn.simpleicons.org/jira" x="114" y="174" width="32" height="32" />
        </g>
      </g>
    </g>
  </g>

</svg>
