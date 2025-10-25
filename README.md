# hrishikesh-portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hrishikesh Nanda - AI Data Analyst Portfolio</title>
    <meta name="description" content="Professional portfolio of Hrishikesh Nanda - AI Data Analyst specializing in Python, SQL, Power BI, and data visualization">
    <meta name="keywords" content="AI Data Analyst, Data Science, Python, SQL, Power BI, Hrishikesh Nanda">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: #0f0f1e;
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .bg-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 0;
            background: linear-gradient(45deg, #0f0f1e, #1a1a3e, #0f0f1e);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
        }
        
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 1;
            pointer-events: none;
        }
        
        .particle {
            position: absolute;
            background: rgba(99, 102, 241, 0.5);
            border-radius: 50%;
            animation: float 20s infinite;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(0deg); opacity: 0; }
            10% { opacity: 1; }
            90% { opacity: 1; }
            100% { transform: translateY(-1000px) rotate(720deg); opacity: 0; }
        }
        
        .container {
            position: relative;
            z-index: 2;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .header {
            text-align: center;
            padding: 80px 20px;
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(10px);
            border-radius: 30px;
            margin-bottom: 40px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.5);
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
        
        .profile-image {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            margin: 0 auto 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            color: white;
            font-weight: bold;
            box-shadow: 0 10px 40px rgba(102, 126, 234, 0.5);
            animation: pulse 3s ease-in-out infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        .header h1 {
            font-size: 3.5em;
            margin-bottom: 10px;
            font-weight: 700;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: shimmer 3s ease-in-out infinite;
        }
        
        @keyframes shimmer {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        
        .header h2 {
            font-size: 1.8em;
            font-weight: 300;
            color: #a0a0ff;
            margin-bottom: 30px;
            animation: fadeIn 1.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            margin-top: 30px;
        }
        
        .contact-btn {
            background: rgba(102, 126, 234, 0.2);
            color: white;
            padding: 12px 25px;
            border-radius: 25px;
            text-decoration: none;
            transition: all 0.3s;
            border: 1px solid rgba(102, 126, 234, 0.5);
            backdrop-filter: blur(10px);
            font-weight: 500;
        }
        
        .contact-btn:hover {
            background: rgba(102, 126, 234, 0.4);
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
        }
        
        .content {
            display: grid;
            gap: 30px;
        }
        
        .section {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: fadeInUp 1s ease;
            transition: all 0.3s;
        }
        
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(102, 126, 234, 0.2);
            border-color: rgba(102, 126, 234, 0.3);
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
        
        .section h3 {
            color: #ffffff;
            font-size: 2em;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid;
            border-image: linear-gradient(90deg, #667eea, #764ba2) 1;
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .section-icon {
            font-size: 1.2em;
        }
        
        .summary {
            background: rgba(102, 126, 234, 0.1);
            padding: 30px;
            border-radius: 15px;
            border-left: 4px solid #667eea;
            font-size: 1.1em;
            line-height: 1.9;
            color: #e0e0ff;
        }
        
        .experience-item, .project-item {
            margin-bottom: 25px;
            padding: 25px;
            background: rgba(102, 126, 234, 0.05);
            border-radius: 15px;
            border-left: 4px solid #667eea;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .experience-item::before, .project-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.1), transparent);
            opacity: 0;
            transition: opacity 0.3s;
        }
        
        .experience-item:hover::before, .project-item:hover::before {
            opacity: 1;
        }
        
        .experience-item:hover, .project-item:hover {
            transform: translateX(10px);
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
        }
        
        .experience-item h4, .project-item h4 {
            color: #ffffff;
            font-size: 1.4em;
            margin-bottom: 8px;
            position: relative;
            z-index: 1;
        }
        
        .company, .project-date {
            color: #a0a0ff;
            font-weight: 600;
            margin-bottom: 5px;
            position: relative;
            z-index: 1;
        }
        
        .date-location {
            color: #8080cc;
            font-size: 0.95em;
            margin-bottom: 12px;
            position: relative;
            z-index: 1;
        }
        
        .description {
            color: #b0b0e0;
            font-style: italic;
            margin-bottom: 15px;
            position: relative;
            z-index: 1;
        }
        
        .experience-item ul, .project-item ul {
            margin-left: 20px;
            margin-top: 12px;
            position: relative;
            z-index: 1;
        }
        
        .experience-item li, .project-item li {
            margin-bottom: 10px;
            color: #d0d0f0;
            position: relative;
            padding-left: 10px;
        }
        
        .experience-item li::before, .project-item li::before {
            content: '▹';
            position: absolute;
            left: -10px;
            color: #667eea;
        }
        
        .education-item {
            margin-bottom: 20px;
            padding: 20px;
            background: rgba(102, 126, 234, 0.05);
            border-radius: 15px;
            border-left: 4px solid #764ba2;
            transition: all 0.3s;
        }
        
        .education-item:hover {
            transform: translateX(10px);
            background: rgba(102, 126, 234, 0.1);
        }
        
        .education-item h4 {
            color: #ffffff;
            font-size: 1.3em;
            margin-bottom: 5px;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        
        .skill-tag {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px 20px;
            border-radius: 15px;
            text-align: center;
            font-weight: 600;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .skill-tag::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.3) 0%, transparent 70%);
            opacity: 0;
            transition: opacity 0.3s;
        }
        
        .skill-tag:hover::before {
            opacity: 1;
        }
        
        .skill-tag:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.5);
        }
        
        .languages {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .language-item {
            padding: 25px;
            background: rgba(102, 126, 234, 0.05);
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s;
            border: 1px solid rgba(102, 126, 234, 0.2);
        }
        
        .language-item:hover {
            background: rgba(102, 126, 234, 0.15);
            transform: translateY(-5px);
        }
        
        .language-item h5 {
            color: #a0a0ff;
            margin-bottom: 8px;
            font-size: 1.2em;
        }
        
        .language-item p {
            color: #d0d0f0;
        }
        
        .achievement {
            background: rgba(102, 126, 234, 0.1);
            padding: 25px;
            border-radius: 15px;
            border-left: 4px solid #f093fb;
            transition: all 0.3s;
        }
        
        .achievement:hover {
            background: rgba(102, 126, 234, 0.15);
            transform: translateX(10px);
        }
        
        .achievement h4 {
            color: #ffffff;
            margin-bottom: 12px;
            font-size: 1.3em;
        }
        
        .achievement p {
            color: #d0d0f0;
            line-height: 1.7;
        }
        
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2.2em;
            }
            
            .header h2 {
                font-size: 1.3em;
            }
            
            .contact-info {
                flex-direction: column;
                gap: 15px;
            }
            
            .section {
                padding: 25px;
            }
            
            .skills-grid {
                grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            }
        }
    </style>
</head>
<body>
    <div class="bg-animation"></div>
    <div class="particles" id="particles"></div>
    
    <div class="container">
        <div class="header">
            <div class="profile-image">HN</div>
            <h1>HRISHIKESH NANDA</h1>
            <h2>AI Data Analyst</h2>
            <div class="contact-info">
                <a href="tel:08658584467" class="contact-btn">📞 08658584467</a>
                <a href="mailto:hrishinanda2@gmail.com" class="contact-btn">✉️ hrishinanda2@gmail.com</a>
                <a href="https://linkedin.com/in/hrishikesh-nanda-0ab371245" target="_blank" class="contact-btn">💼 LinkedIn</a>
                <span class="contact-btn">📍 Bhubaneswar, India</span>
            </div>
        </div>
        
        <div class="content">
            <div class="section">
                <h3><span class="section-icon">👨‍💼</span> Summary</h3>
                <div class="summary">
                    I am an enthusiastic and adaptable fresher with practical experience in applying artificial intelligence (AI) and automation to data analysis tasks. Skilled in Python, SQL, Power BI, and Excel, I can leverage modern AI tools and machine learning techniques to extract meaningful insights from complex datasets. I have hands-on exposure to data annotation, tagging, and conversational AI systems, and enjoy problem-solving and improving business processes. Eager to join a forward-thinking organization and contribute to impactful data-driven decisions using the latest AI technologies.
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">💼</span> Experience</h3>
                
                <div class="experience-item">
                    <h4>Data Analyst Intern</h4>
                    <div class="company">Deloitte India (Remote)</div>
                    <div class="date-location">June 2025 | Bhubaneswar, India</div>
                    <div class="description">A global leader in audit and consulting services</div>
                    <ul>
                        <li>Engaged in an internship that involved analyzing business data</li>
                        <li>Created trends and charts using Excel and SQL</li>
                        <li>Collaborated effectively with the data team and communicated findings</li>
                    </ul>
                </div>
                
                <div class="experience-item">
                    <h4>Data Science</h4>
                    <div class="company">Whizzo Infotech Pvt. Ltd</div>
                    <div class="date-location">December 2021 - April 2022 | Bhubaneswar, Odisha</div>
                    <div class="description">A technology company specializing in data solutions</div>
                    <ul>
                        <li>Hands-on experience in data analysis and visualization using Excel and Power BI</li>
                        <li>Utilized SQL for data manipulation and extraction</li>
                        <li>Contributed to projects focused on data-driven insights</li>
                    </ul>
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">🚀</span> Projects</h3>
                
                <div class="project-item">
                    <h4>Profit Margins and Trends in Sales Data</h4>
                    <div class="project-date">July 2025 - August 2025</div>
                    <div class="description">Analysis of sales data to provide insights on profitability and trends</div>
                    <ul>
                        <li>Conducted a comprehensive analysis of sales data to evaluate profit margins</li>
                        <li>Calculated profit margins for individual transactions and visualized monthly trends</li>
                        <li>Utilized Python, pandas, and matplotlib for data processing and visualization</li>
                        <li>Identified periods of high and low profitability providing insights for strategic decisions</li>
                    </ul>
                </div>
                
                <div class="project-item">
                    <h4>Project Portfolio - Sales Dashboard</h4>
                    <div class="project-date">July 2025 - August 2025</div>
                    <div class="description">Creating a dashboard to visualize sales performance metrics</div>
                    <ul>
                        <li>Built an interactive Power BI dashboard from sample sales data</li>
                        <li>Tracked KPIs like total sales, regional trends, and product contribution</li>
                        <li>Used Power Query for data cleaning and DAX for calculations</li>
                    </ul>
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">⚡</span> Skills</h3>
                <div class="skills-grid">
                    <div class="skill-tag">Python</div>
                    <div class="skill-tag">SQL</div>
                    <div class="skill-tag">Power BI</div>
                    <div class="skill-tag">Excel</div>
                    <div class="skill-tag">DAX</div>
                    <div class="skill-tag">PowerPoint</div>
                    <div class="skill-tag">Pandas</div>
                    <div class="skill-tag">Matplotlib</div>
                    <div class="skill-tag">Numerous.ai</div>
                    <div class="skill-tag">ThoughtSpot</div>
                    <div class="skill-tag">Perplexity</div>
                    <div class="skill-tag">Powerdrill</div>
                    <div class="skill-tag">Julius AI</div>
                    <div class="skill-tag">Bloom</div>
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">🎓</span> Education</h3>
                
                <div class="education-item">
                    <h4>Engineering</h4>
                    <div class="company">Kalam Institute of Technology</div>
                    <div class="date-location">July 2017 - August 2020 | Berhampur</div>
                </div>
                
                <div class="education-item">
                    <h4>Diploma</h4>
                    <div class="company">Biju Patnaik University of Technology</div>
                    <div class="date-location">November 2014 - March 2016 | Koraput, Odisha</div>
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">🏆</span> Key Achievements</h3>
                <div class="achievement">
                    <h4>Data Analysis and Visualization</h4>
                    <p>Contributed to data-driven decision making in project teams by identifying periods of high and low profitability and recommending strategic improvements.</p>
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">🌐</span> Languages</h3>
                <div class="languages">
                    <div class="language-item">
                        <h5>Odia</h5>
                        <p>Native</p>
                    </div>
                    <div class="language-item">
                        <h5>Hindi</h5>
                        <p>Proficient</p>
                    </div>
                    <div class="language-item">
                        <h5>English</h5>
                        <p>Native</p>
                    </div>
                </div>
            </div>
            
            <div class="section">
                <h3><span class="section-icon">💪</span> Interests</h3>
                <div class="achievement">
                    <h4>Weight Lifting</h4>
                    <p>Passionate about fitness and health</p>
                </div>
            </div>
        </div>
    </div>
    
    <script>
        // Create floating particles
        const particlesContainer = document.getElementById('particles');
        for (let i = 0; i < 30; i++) {
            const particle = document.createElement('div');
            particle.className = 'particle';
            const size = Math.random() * 5 + 2;
            particle.style.width = size + 'px';
            particle.style.height = size + 'px';
            particle.style.left = Math.random() * 100 + '%';
            particle.style.animationDuration = (Math.random() * 10 + 15) + 's';
            particle.style.animationDelay = Math.random() * 5 + 's';
            particlesContainer.appendChild(particle);
        }
    </script>
</body>
</html>
