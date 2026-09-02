<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mohammad Zaid Ali - Software Developer</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        .container {
            background: white;
            border-radius: 10px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }
        header {
            text-align: center;
            padding: 30px 0;
            border-bottom: 3px solid #667eea;
            margin-bottom: 30px;
        }
        h1 {
            font-size: 2.5em;
            margin: 0;
            color: #2c3e50;
        }
        .contact-links {
            margin: 20px 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
        }
        .contact-links a {
            display: inline-block;
            padding: 10px 20px;
            background: #667eea;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: all 0.3s;
            font-weight: 500;
        }
        .contact-links a:hover {
            background: #5568d3;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }
        .summary {
            background: #f8f9fa;
            padding: 25px;
            border-left: 5px solid #667eea;
            margin: 30px 0;
            border-radius: 5px;
        }
        .summary h2 {
            margin-top: 0;
            color: #667eea;
        }
        .achievements {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }
        .achievement-item {
            background: white;
            padding: 15px;
            border-left: 4px solid #28a745;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .achievement-item strong {
            color: #28a745;
        }
        h2 {
            color: #2c3e50;
            border-bottom: 2px solid #667eea;
            padding-bottom: 10px;
            margin-top: 40px;
        }
        .tech-section {
            margin: 30px 0;
        }
        .tech-category {
            margin: 20px 0;
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
        }
        .tech-category h3 {
            color: #667eea;
            margin-top: 0;
            font-size: 1.3em;
        }
        .tech-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        .badge {
            display: inline-block;
            padding: 8px 15px;
            background: #667eea;
            color: white;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: 500;
        }
        .experience-item {
            margin: 30px 0;
            padding: 25px;
            background: #f8f9fa;
            border-radius: 8px;
            border-left: 5px solid #667eea;
        }
        .experience-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            margin-bottom: 15px;
        }
        .job-title {
            font-size: 1.3em;
            font-weight: bold;
            color: #2c3e50;
        }
        .company {
            color: #667eea;
            font-weight: 600;
        }
        .duration {
            color: #6c757d;
            font-style: italic;
        }
        .experience-item ul {
            margin: 15px 0;
            padding-left: 25px;
        }
        .experience-item li {
            margin: 10px 0;
            line-height: 1.6;
        }
        .experience-item li::marker {
            color: #667eea;
            font-weight: bold;
        }
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        .project-card {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 8px;
            border-top: 4px solid #667eea;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
        }
        .project-card h3 {
            color: #667eea;
            margin-top: 0;
        }
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 15px 0;
        }
        .tech-tag {
            background: #e7f3ff;
            color: #0366d6;
            padding: 5px 12px;
            border-radius: 15px;
            font-size: 0.85em;
            font-weight: 500;
        }
        .education {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 8px;
            margin: 30px 0;
        }
        .education h3 {
            color: #667eea;
            margin-top: 0;
        }
        .cert-badge {
            display: inline-block;
            background: #28a745;
            color: white;
            padding: 8px 15px;
            border-radius: 5px;
            margin-top: 10px;
            font-weight: 500;
        }
        footer {
            text-align: center;
            margin-top: 50px;
            padding: 30px;
            background: #f8f9fa;
            border-radius: 8px;
            border-top: 3px solid #667eea;
        }
        footer h3 {
            color: #2c3e50;
            margin-bottom: 20px;
        }
        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }
        .cta-button {
            display: inline-block;
            padding: 12px 30px;
            background: #667eea;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-weight: 600;
            transition: all 0.3s;
        }
        .cta-button:hover {
            background: #5568d3;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }
        .cta-button.secondary {
            background: #28a745;
        }
        .cta-button.secondary:hover {
            background: #218838;
        }
        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }
            h1 {
                font-size: 1.8em;
            }
            .experience-header {
                flex-direction: column;
                align-items: flex-start;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Mohammad Zaid Ali</h1>
            <p style="font-size: 1.2em; color: #6c757d; margin: 10px 0;">Software Developer | AI/LLM Systems | Cloud Architecture</p>
            
            <div class="contact-links">
                <a href="mailto:mzaid.zhcet@gmail.com">📧 Email</a>
                <a href="https://linkedin.com/in/mzaidali" target="_blank">💼 LinkedIn</a>
                <a href="https://github.com/Zaidtech" target="_blank">🔗 GitHub</a>
                <a href="tel:+917037172999">📱 +91-7037172999</a>
            </div>
        </header>

        <section class="summary">
            <h2>👨‍💻 Professional Summary</h2>
            <p>Senior Software Developer with <strong>3+ years</strong> of expertise in <strong>full-stack development</strong>, <strong>enterprise Agentic AI systems</strong>, and <strong>scalable cloud architectures</strong> (AWS/GCP). Currently architecting <strong>legacy-to-modern language modernization</strong> solutions, parsing <strong>7.5M+ lines of ASM code</strong> and extracting lineage for <strong>600,000+ variables</strong>.</p>
            
            <div class="achievements">
                <div class="achievement-item">
                    <strong>⚡ 25% Faster</strong><br>
                    BigQuery queries for 10M+ records
                </div>
                <div class="achievement-item">
                    <strong>🚀 99.9% Consistency</strong><br>
                    ETL pipelines processing 20M+ records
                </div>
                <div class="achievement-item">
                    <strong>🤖 Months → 10 Seconds</strong><br>
                    LLM chatbot for legacy lineage tracking
                </div>
                <div class="achievement-item">
                    <strong>📊 60% Time Reduction</strong><br>
                    Using RAG systems (LangChain + FAISS)
                </div>
            </div>
        </section>

        <section class="tech-section">
            <h2>🛠️ Technical Arsenal</h2>
            
            <div class="tech-category">
                <h3>Languages & Frameworks</h3>
                <div class="tech-badges">
                    <span class="badge">Java 17/21</span>
                    <span class="badge">TypeScript</span>
                    <span class="badge">Python</span>
                    <span class="badge">ASM</span>
                    <span class="badge">Spring Boot</span>
                    <span class="badge">React</span>
                    <span class="badge">Flask</span>
                    <span class="badge">FastAPI</span>
                    <span class="badge">AngularJS</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>Cloud & DevOps</h3>
                <div class="tech-badges">
                    <span class="badge">AWS (S3, Lambda, EC2, Glue)</span>
                    <span class="badge">GCP (BigQuery)</span>
                    <span class="badge">Docker</span>
                    <span class="badge">Jenkins</span>
                    <span class="badge">Kafka</span>
                    <span class="badge">CI/CD</span>
                    <span class="badge">Apigee</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>AI/LLM & Data Engineering</h3>
                <div class="tech-badges">
                    <span class="badge">RAG</span>
                    <span class="badge">LangChain</span>
                    <span class="badge">LangGraph</span>
                    <span class="badge">MCP</span>
                    <span class="badge">OpenAI APIs</span>
                    <span class="badge">Agentic AI</span>
                    <span class="badge">FAISS</span>
                    <span class="badge">Pinecone</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>Databases</h3>
                <div class="tech-badges">
                    <span class="badge">PostgreSQL</span>
                    <span class="badge">MySQL</span>
                    <span class="badge">Snowflake</span>
                    <span class="badge">Redis</span>
                    <span class="badge">Neo4j</span>
                </div>
            </div>
        </section>

        <section>
            <h2>💼 Professional Experience</h2>

            <div class="experience-item">
                <div class="experience-header">
                    <div>
                        <div class="job-title">🔹 Software Developer</div>
                        <div class="company">OpZen.ai</div>
                    </div>
                    <div>
                        <div class="duration">Feb 2026 – Present</div>
                        <div style="color: #6c757d;">Remote, India</div>
                    </div>
                </div>
                <ul>
                    <li>🧠 Engineered <strong>custom ASM/C++ parser</strong> using Tree-sitter for enterprise Credit Authorization system (IBM z/OS), processing <strong>22,000+ files</strong> and <strong>7.5M+ lines of code</strong> to capture <strong>600,000+ variables</strong></li>
                    <li>📊 Indexed <strong>50GB+ call graph data</strong>, enabling <strong>millisecond-level</strong> variable lineage tracing from root to terminal</li>
                    <li>🤖 Deployed <strong>LLM-powered chatbot</strong> over indexed blueprints, reducing legacy tracking time from <strong>months → 10 seconds</strong></li>
                    <li>⚙️ Architected testing harness using AI coding agent, establishing rules-extraction framework that accelerated decision-to-implementation cycle from <strong>months → days</strong></li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div>
                        <div class="job-title">🔹 Software Engineer II <span style="color: #28a745;">(Promoted)</span></div>
                        <div class="company">Zenon Analytics</div>
                    </div>
                    <div>
                        <div class="duration">Nov 2024 – Jan 2026</div>
                        <div style="color: #6c757d;">Noida, India</div>
                    </div>
                </div>
                <ul>
                    <li>🚀 Reworked Dow Jones FAST Tool engine by moving forecasting logic into database stored procedures; lowered query latency by <strong>25%</strong> and heap memory usage by <strong>40%</strong> for <strong>10M+ records</strong></li>
                    <li>⚡ Designed serverless ETL pipeline with AWS Glue and Lambda to process <strong>20M+ records</strong> from Parquet; maintained <strong>99.9% data consistency</strong></li>
                    <li>🔍 Assembled internal RAG system (LangChain + FAISS) for decision support; trimmed manual analysis time by <strong>60%</strong></li>
                    <li>📉 Drove KeyBank and ADP delivery by handling P1 incidents, dropping client-reported bugs by <strong>15%</strong></li>
                    <li>👨‍🏫 Mentored <strong>10+ engineers</strong> on Java/Linux practices, improving new-hire onboarding time by <strong>30%</strong></li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="experience-header">
                    <div>
                        <div class="job-title">🔹 Software Engineer I</div>
                        <div class="company">Zenon Analytics</div>
                    </div>
                    <div>
                        <div class="duration">Jul 2023 – Nov 2024</div>
                        <div style="color: #6c757d;">Noida, India</div>
                    </div>
                </div>
                <ul>
                    <li>🔒 Orchestrated <strong>Apigee API Gateway</strong> integration handling <strong>10K+ daily transactions</strong> with rate limiting and policy controls</li>
                    <li>⏱️ Streamlined ACH payment tracking by hardening secure file processing in Java; compressed report generation from <strong>1 week → 3 hours</strong> (<strong>85% efficiency gain</strong>)</li>
                    <li>🔐 Rolled out enterprise <strong>SSO (Okta/SAML)</strong> with Active Directory, enabling role provisioning for <strong>5,000+ users</strong></li>
                    <li>📤 Delivered metadata-driven bulk upload engine with GraphQL APIs, supporting <strong>50K records per batch</strong> with real-time validation</li>
                    <li>⚙️ Tuned multi-table JOIN queries for lease trigger module; cut execution time by <strong>40%</strong> on <strong>5M+ rows</strong></li>
                    <li>🌐 Deployed hiring SaaS platform handling <strong>100K+ records</strong>; integrated validation engine and shipped React frontend</li>
                </ul>
            </div>
        </section>

        <section>
            <h2>🚀 Featured Projects</h2>
            <div class="projects">
                <div class="project-card">
                    <h3>📱 KitnaBana</h3>
                    <p style="font-style: italic; color: #6c757d;">AI-Powered Financial App for Indian Gig Workers</p>
                    <div class="project-tech">
                        <span class="tech-tag">React Native</span>
                        <span class="tech-tag">Expo</span>
                        <span class="tech-tag">TypeScript</span>
                    </div>
                    <ul>
                        <li>Published Android application acting as daily financial sidekick for gig workers</li>
                        <li>Implemented <strong>multilingual UI</strong> (English, Urdu) with correct RTL layout handling</li>
                        <li>Configured <strong>Codemagic</strong> for seamless CI/CD release pipelines</li>
                    </ul>
                </div>

                <div class="project-card">
                    <h3>🎓 SmartTutor</h3>
                    <p style="font-style: italic; color: #6c757d;">RAG-Powered Learning Platform</p>
                    <div class="project-tech">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">LangChain</span>
                        <span class="tech-tag">FAISS</span>
                        <span class="tech-tag">Streamlit</span>
                    </div>
                    <ul>
                        <li>Improved PDF and URL ingestion time by <strong>90%</strong> through strategic caching</li>
                        <li>Prevented redundant reindexing in <strong>LLM-agnostic RAG pipeline</strong></li>
                        <li>Built intelligent learning assistant with vector similarity search</li>
                    </ul>
                </div>
            </div>
        </section>

        <section>
            <h2>🎓 Education & Certifications</h2>
            <div class="education">
                <h3>Aligarh Muslim University</h3>
                <p><strong>B.Tech in Computer Engineering</strong> | 2019 – 2023</p>
                <p><strong>CGPA:</strong> 9.3/10.0</p>
                
                <div style="margin-top: 20px;">
                    <h4 style="color: #667eea;">Certifications:</h4>
                    <span class="cert-badge">✅ Neo4j Certified Professional</span>
                    <p style="margin-top: 10px; color: #6c757d;">Graph Database Fundamentals & Cypher Query Language</p>
                </div>
            </div>
        </section>

        <footer>
            <h3>📬 Let's Connect!</h3>
            <p style="color: #6c757d; margin-bottom: 20px;">
                Open to collaborations in Full-Stack Development, AI/LLM Systems, and Cloud Architecture
            </p>
            <div class="cta-buttons">
                <a href="https://linkedin.com/in/mzaidali" class="cta-button" target="_blank">Connect on LinkedIn</a>
                <a href="mailto:mzaid.zhcet@gmail.com" class="cta-button secondary">Send an Email</a>
                <a href="https://github.com/Zaidtech" class="cta-button" target="_blank">View GitHub</a>
            </div>
            <p style="margin-top: 30px; color: #6c757d; font-size: 0.9em;">
                © 2024 Mohammad Zaid Ali. All rights reserved.
            </p>
        </footer>
    </div>
</body>
</html>
