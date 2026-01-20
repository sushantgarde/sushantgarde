<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sushant G. - ML Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #0f0f1e 0%, #1a0033 25%, #0d0015 50%, #1a0033 75%, #0f0f1e 100%);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
            color: #e0e0e0;
            padding: 20px;
            min-height: 100vh;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: rgba(10, 10, 20, 0.8);
            backdrop-filter: blur(10px);
            border: 2px solid rgba(100, 200, 255, 0.3);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3), 0 0 50px rgba(100, 200, 255, 0.1);
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
            animation: fadeInDown 1s ease;
        }
        
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .header h1 {
            font-size: 3em;
            background: linear-gradient(45deg, #00d4ff, #0099ff, #00ff88);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
            text-shadow: 0 0 20px rgba(0, 212, 255, 0.3);
        }
        
        .badge-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin: 20px 0;
        }
        
        .badge {
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.2), rgba(0, 255, 136, 0.2));
            border: 1px solid rgba(0, 212, 255, 0.4);
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: bold;
            animation: pulse 2s ease-in-out infinite;
        }
        
        .badge:nth-child(1) { animation-delay: 0s; }
        .badge:nth-child(2) { animation-delay: 0.2s; }
        .badge:nth-child(3) { animation-delay: 0.4s; }
        .badge:nth-child(4) { animation-delay: 0.6s; }
        
        @keyframes pulse {
            0%, 100% { box-shadow: 0 0 10px rgba(0, 212, 255, 0.3); }
            50% { box-shadow: 0 0 20px rgba(0, 255, 136, 0.6); }
        }
        
        .about {
            margin: 40px 0;
            padding: 20px;
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.1), rgba(0, 255, 136, 0.1));
            border-left: 4px solid #00d4ff;
            border-radius: 10px;
            animation: fadeInLeft 1s ease 0.3s backwards;
        }
        
        @keyframes fadeInLeft {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        .about h2 {
            color: #00d4ff;
            margin-bottom: 15px;
            font-size: 1.8em;
        }
        
        .about p {
            line-height: 1.8;
            font-size: 1.1em;
            color: #b0b0b0;
        }
        
        .section {
            margin: 40px 0;
            animation: fadeInUp 1s ease backwards;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .section:nth-child(3) { animation-delay: 0.2s; }
        .section:nth-child(4) { animation-delay: 0.4s; }
        .section:nth-child(5) { animation-delay: 0.6s; }
        .section:nth-child(6) { animation-delay: 0.8s; }
        
        .section h2 {
            color: #00ff88;
            font-size: 1.8em;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid rgba(0, 255, 136, 0.3);
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            margin-bottom: 20px;
        }
        
        .tech-item {
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.1), rgba(0, 155, 255, 0.1));
            border: 1px solid rgba(0, 212, 255, 0.3);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .tech-item:hover {
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.3), rgba(0, 155, 255, 0.3));
            border-color: rgba(0, 255, 136, 0.6);
            transform: translateY(-5px);
            box-shadow: 0 0 20px rgba(0, 212, 255, 0.4);
        }
        
        .tech-item strong {
            color: #00d4ff;
            display: block;
            margin-bottom: 5px;
        }
        
        .project {
            background: linear-gradient(135deg, rgba(0, 155, 255, 0.05), rgba(0, 255, 136, 0.05));
            border: 1px solid rgba(0, 212, 255, 0.2);
            padding: 25px;
            border-radius: 15px;
            margin-bottom: 25px;
            transition: all 0.3s ease;
        }
        
        .project:hover {
            background: linear-gradient(135deg, rgba(0, 155, 255, 0.1), rgba(0, 255, 136, 0.1));
            border-color: rgba(0, 255, 136, 0.5);
            transform: translateX(5px);
            box-shadow: 0 0 25px rgba(0, 212, 255, 0.2);
        }
        
        .project-title {
            color: #00ff88;
            font-size: 1.5em;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .project-emoji {
            font-size: 1.3em;
        }
        
        .project-link {
            color: #00d4ff;
            text-decoration: none;
            font-weight: bold;
            margin: 10px 0;
            display: inline-block;
        }
        
        .project-link:hover {
            text-decoration: underline;
            color: #00ff88;
        }
        
        .project-desc {
            color: #a0a0a0;
            margin: 15px 0;
            line-height: 1.6;
        }
        
        .tech-tags {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 15px;
        }
        
        .tag {
            background: rgba(0, 212, 255, 0.2);
            color: #00d4ff;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.85em;
            border: 1px solid rgba(0, 212, 255, 0.4);
        }
        
        .learning {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        
        .learning-item {
            background: linear-gradient(135deg, rgba(255, 107, 0, 0.1), rgba(255, 200, 0, 0.1));
            border: 1px solid rgba(255, 107, 0, 0.3);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            color: #ffb300;
        }
        
        .learning-item strong {
            display: block;
            font-size: 1.1em;
        }
        
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
            text-align: center;
        }
        
        .stat-box {
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.1), rgba(0, 255, 136, 0.1));
            border: 1px solid rgba(0, 212, 255, 0.3);
            padding: 20px;
            border-radius: 10px;
        }
        
        .stat-number {
            font-size: 2.5em;
            color: #00ff88;
            font-weight: bold;
        }
        
        .stat-label {
            color: #00d4ff;
            margin-top: 10px;
        }
        
        .contact-section {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }
        
        .contact-btn {
            background: linear-gradient(135deg, #00d4ff, #0099ff);
            color: #000;
            padding: 12px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1em;
        }
        
        .contact-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(0, 212, 255, 0.4);
        }
        
        .contact-btn.secondary {
            background: linear-gradient(135deg, #00ff88, #00d4ff);
        }
        
        .footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 30px;
            border-top: 1px solid rgba(0, 212, 255, 0.2);
            color: #808080;
        }
        
        .footer p {
            margin: 10px 0;
            font-style: italic;
        }
        
        .highlight-box {
            background: linear-gradient(135deg, rgba(0, 255, 136, 0.1), rgba(0, 212, 255, 0.1));
            border-left: 4px solid #00ff88;
            padding: 20px;
            margin: 20px 0;
            border-radius: 10px;
        }
        
        .skills-showcase {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
            margin: 20px 0;
        }
        
        .skill-card {
            background: linear-gradient(135deg, rgba(0, 155, 255, 0.1), rgba(0, 255, 136, 0.1));
            border: 1px solid rgba(0, 212, 255, 0.3);
            padding: 20px;
            border-radius: 10px;
            transition: all 0.3s ease;
        }
        
        .skill-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 212, 255, 0.2);
        }
        
        .skill-card h3 {
            color: #00ff88;
            margin-bottom: 10px;
        }
        
        .skill-card p {
            color: #a0a0a0;
        }
        
        .neon-text {
            color: #00d4ff;
            text-shadow: 0 0 10px rgba(0, 212, 255, 0.8), 0 0 20px rgba(0, 255, 136, 0.4);
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- HEADER -->
        <div class="header">
            <h1>🚀 SUSHANT G.</h1>
            <p style="font-size: 1.2em; color: #00d4ff; margin-bottom: 15px;">ML/AI Engineer | Deep Learning Specialist</p>
            
            <div class="badge-container">
                <div class="badge">🎓 Prefinal Year @ Nutan Engineering</div>
                <div class="badge">🤖 ML/AI Engineer</div>
                <div class="badge">📊 Data Scientist</div>
                <div class="badge">🎯 Seeking Internships & Placements</div>
            </div>
        </div>
        
        <!-- ABOUT -->
        <div class="about">
            <h2>💡 About Me - The Vision</h2>
            <p>I'm an <span class="neon-text">ML/AI Engineer</span> building intelligent systems that solve real-world problems. My expertise lies in <strong>Deep Learning, Computer Vision, and Data Science</strong>. I transform raw data into actionable intelligence using cutting-edge AI techniques.</p>
            <p style="margin-top: 15px;"><strong>What excites me:</strong> Triplet Networks • ResNet architectures • Deepfake Detection • Image Retrieval Systems • Advanced ML algorithms • Production-grade AI solutions</p>
        </div>
        
        <!-- CORE COMPETENCIES -->
        <div class="section">
            <h2>⚡ Core Competencies</h2>
            <div class="skills-showcase">
                <div class="skill-card">
                    <h3>🐍 Python Master</h3>
                    <p>Expert-level Python programming for ML applications, data processing, and system design</p>
                </div>
                <div class="skill-card">
                    <h3>📊 Data Science</h3>
                    <p>Statistical analysis, feature engineering, exploratory data analysis, predictive modeling</p>
                </div>
                <div class="skill-card">
                    <h3>🤖 ML/AI Engineering</h3>
                    <p>Building production-ready ML models using TensorFlow, PyTorch, and scikit-learn</p>
                </div>
                <div class="skill-card">
                    <h3>📈 Data Analysis</h3>
                    <p>Extracting insights from complex datasets, visualization, and business intelligence</p>
                </div>
            </div>
        </div>
        
        <!-- TECH STACK -->
        <div class="section">
            <h2>🛠️ Tech Arsenal</h2>
            
            <p style="color: #00d4ff; font-weight: bold; margin-bottom: 15px;">Languages</p>
            <div class="tech-grid">
                <div class="tech-item">
                    <strong>🐍 Python</strong>
                    <span>Advanced</span>
                </div>
                <div class="tech-item">
                    <strong>💾 C</strong>
                    <span>Intermediate</span>
                </div>
                <div class="tech-item">
                    <strong>☕ Java</strong>
                    <span>Basic</span>
                </div>
                <div class="tech-item">
                    <strong>⚙️ C++</strong>
                    <span>Basic</span>
                </div>
            </div>
            
            <p style="color: #00d4ff; font-weight: bold; margin: 20px 0 15px 0;">ML/AI Frameworks</p>
            <div class="tech-grid">
                <div class="tech-item">
                    <strong>🔥 TensorFlow</strong>
                    <span>Advanced</span>
                </div>
                <div class="tech-item">
                    <strong>🔥 PyTorch</strong>
                    <span>Advanced</span>
                </div>
                <div class="tech-item">
                    <strong>📚 Scikit-Learn</strong>
                    <span>Advanced</span>
                </div>
                <div class="tech-item">
                    <strong>🧠 Keras</strong>
                    <span>Advanced</span>
                </div>
            </div>
            
            <p style="color: #00d4ff; font-weight: bold; margin: 20px 0 15px 0;">Tools & Platforms</p>
            <div class="tech-grid">
                <div class="tech-item"><strong>📓 Jupyter</strong></div>
                <div class="tech-item"><strong>☁️ Google Colab</strong></div>
                <div class="tech-item"><strong>🐱 GitHub</strong></div>
                <div class="tech-item"><strong>📦 Anaconda</strong></div>
                <div class="tech-item"><strong>🏆 Kaggle</strong></div>
                <div class="tech-item"><strong>💻 VS Code</strong></div>
                <div class="tech-item"><strong>🔧 Flask</strong></div>
                <div class="tech-item"><strong>🗄️ MySQL</strong></div>
            </div>
        </div>
        
        <!-- FLAGSHIP PROJECTS -->
        <div class="section">
            <h2>🏆 Flagship Projects - Proof of Expertise</h2>
            
            <!-- Project 1 -->
            <div class="project">
                <div class="project-title">
                    <span class="project-emoji">👁️</span> Image Similarity Detection
                </div>
                <a href="https://github.com/sushantgarde/image_similarity" class="project-link">📍 View Repository</a>
                <div class="project-desc">
                    <strong>Mission:</strong> Find semantic twins among millions of images using deep neural networks and triplet loss optimization.
                </div>
                <p style="color: #b0b0b0;"><strong>What Makes It Special:</strong></p>
                <p style="color: #a0a0a0; margin-left: 15px;">
                    ✓ ResNet50 backbone for powerful feature extraction<br>
                    ✓ Triplet loss learning for metric learning<br>
                    ✓ Lightning-fast similarity computation<br>
                    ✓ Handles diverse image types with high accuracy
                </p>
                <div class="tech-tags">
                    <span class="tag">Python</span>
                    <span class="tag">TensorFlow</span>
                    <span class="tag">ResNet50</span>
                    <span class="tag">Deep Learning</span>
                    <span class="tag">Computer Vision</span>
                </div>
            </div>
            
            <!-- Project 2 -->
            <div class="project">
                <div class="project-title">
                    <span class="project-emoji">🚨</span> Deepfake Detection System
                </div>
                <a href="https://github.com/sushantgarde/deepfake_detection" class="project-link">📍 View Repository</a>
                <div class="project-desc">
                    <strong>Mission:</strong> Separate fact from fiction. Identify AI-generated images vs authentic ones to combat digital fraud and misinformation.
                </div>
                <p style="color: #b0b0b0;"><strong>Superpowers:</strong></p>
                <p style="color: #a0a0a0; margin-left: 15px;">
                    ✓ Real vs Fake classification with high accuracy<br>
                    ✓ Detects synthetic media & AI-generated content<br>
                    ✓ Combat deepfakes & fraudulent media<br>
                    ✓ Trained on diverse deepfake datasets
                </p>
                <div class="tech-tags">
                    <span class="tag">Python</span>
                    <span class="tag">Deep Learning</span>
                    <span class="tag">CNN</span>
                    <span class="tag">Computer Vision</span>
                    <span class="tag">Real/Fake API</span>
                </div>
            </div>
            
            <!-- Project 3 -->
            <div class="project">
                <div class="project-title">
                    <span class="project-emoji">🔍</span> SearchAlike (Contributor)
                </div>
                <a href="https://github.com/Vedant2004X/SearchAlike" class="project-link">📍 View Repository</a>
                <div class="project-desc">
                    <strong>Mission:</strong> Google-level semantic image search powered by triplet networks and advanced deep learning architectures.
                </div>
                <p style="color: #b0b0b0;"><strong>Technical Marvel:</strong></p>
                <p style="color: #a0a0a0; margin-left: 15px;">
                    ✓ Triplet Network architecture for metric learning<br>
                    ✓ ResNet50 as backbone for deep feature extraction<br>
                    ✓ Scalable to millions of images<br>
                    ✓ Finds semantically similar images, not just pixel matches
                </p>
                <div class="tech-tags">
                    <span class="tag">Python</span>
                    <span class="tag">Triplet Loss</span>
                    <span class="tag">ResNet50</span>
                    <span class="tag">Metric Learning</span>
                    <span class="tag">Deep Learning</span>
                </div>
            </div>
        </div>
        
        <!-- CURRENTLY LEARNING -->
        <div class="section">
            <h2>🔥 Currently Learning & Exploring</h2>
            <div class="learning">
                <div class="learning-item">
                    <strong>Advanced ML</strong>
                    <p style="color: #ffaa00; margin-top: 8px;">Cutting-edge algorithms</p>
                </div>
                <div class="learning-item">
                    <strong>TensorFlow</strong>
                    <p style="color: #ffaa00; margin-top: 8px;">Production pipelines</p>
                </div>
                <div class="learning-item">
                    <strong>PyTorch</strong>
                    <p style="color: #ffaa00; margin-top: 8px;">Advanced techniques</p>
                </div>
                <div class="learning-item">
                    <strong>Transformers & NLP</strong>
                    <p style="color: #ffaa00; margin-top: 8px;">Language models</p>
                </div>
            </div>
        </div>
        
        <!-- STATS -->
        <div class="section">
            <h2>📊 GitHub Presence</h2>
            <div class="stats-container">
                <div class="stat-box">
                    <div class="stat-number">3+</div>
                    <div class="stat-label">ML Projects</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">100%</div>
                    <div class="stat-label">Python Focused</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">∞</div>
                    <div class="stat-label">Learning Drive</div>
                </div>
                <div class="stat-box">
                    <div class="stat-number">🎯</div>
                    <div class="stat-label">Goal: Make Impact</div>
                </div>
            </div>
        </div>
        
        <!-- WHY HIRE ME -->
        <div class="highlight-box">
            <h3 style="color: #00ff88; margin-bottom: 15px;">💎 Why Hire Me?</h3>
            <p style="color: #b0b0b0; line-height: 1.8;">
                ✅ <strong>Proven ML Expertise:</strong> 3 portfolio projects showcasing deep learning, computer vision, and production-ready systems<br>
                ✅ <strong>Problem Solver:</strong> Breaks down complex ML challenges into elegant, scalable solutions<br>
                ✅ <strong>Quick Learner:</strong> Rapidly masters new frameworks & cutting-edge technologies<br>
                ✅ <strong>Data-Driven:</strong> Every decision backed by experiments, metrics, and insights<br>
                ✅ <strong>Production-Focused:</strong> Not just models—scalable, deployable systems
            </p>
        </div>
        
        <!-- OPPORTUNITIES -->
        <div class="section">
            <h2>🎯 Open To</h2>
            <div class="tech-grid">
                <div class="tech-item" style="background: linear-gradient(135deg, rgba(0, 212, 255, 0.15), rgba(0, 155, 255, 0.15));">
                    <strong>💼 Internships</strong>
                    <p style="color: #00d4ff; margin-top: 5px;">ML/Data Science</p>
                </div>
                <div class="tech-item" style="background: linear-gradient(135deg, rgba(0, 212, 255, 0.15), rgba(0, 155, 255, 0.15));">
                    <strong>🏢 Full-Time Roles</strong>
                    <p style="color: #00d4ff; margin-top: 5px;">ML/AI Engineer</p>
                </div>
                <div class="tech-item" style="background: linear-gradient(135deg, rgba(0, 212, 255, 0.15), rgba(0, 155, 255, 0.15));">
                    <strong>🤝 Collaboration</strong>
                    <p style="color: #00d4ff; margin-top: 5px;">Open-Source Projects</p>
                </div>
                <div class="tech-item" style="background: linear-gradient(135deg, rgba(0, 212, 255, 0.15), rgba(0, 155, 255, 0.15));">
                    <strong>📚 Growth</strong>
                    <p style="color: #00d4ff; margin-top: 5px;">Mentorship & Learning</p>
                </div>
            </div>
        </div>
        
        <!-- CONTACT -->
        <div class="contact-section">
            <a href="mailto:gardesushant1@gmail.com" class="contact-btn">📧 Email Me</a>
            <a href="https://www.linkedin.com/in/sushant-garde" class="contact-btn">💼 LinkedIn</a>
            <a href="https://github.com/sushantgarde" class="contact-btn">🐙 GitHub</a>
        </div>
        
        <!-- FOOTER -->
        <div class="footer">
            <p>⭐ If my work inspires you, star my repositories!</p>
            <p style="color: #808080; font-size: 0.9em; margin-top: 15px;">
                "I transform data into intelligence,<br>
                algorithms into innovation,<br>
                and ideas into reality."
            </p>
            <p style="color: #606060; font-size: 0.85em; margin-top: 15px;">
                🚀 Building Tomorrow's AI, One Algorithm at a Time 🚀
            </p>
        </div>
    </div>
</body>
</html>
