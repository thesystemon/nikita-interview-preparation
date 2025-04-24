### 🔹 **Day 1: Resume Deep Dive + General Introduction**

**1. Tell me about yourself:**  
I am a dedicated DevOps Engineer with hands-on experience in automation, cloud computing, and continuous integration. My journey started with a strong foundation in programming, which evolved into an interest in building scalable, automated infrastructures using tools like AWS, Jenkins, and Docker.

**2. Walk me through your resume:**  
- Bachelor's degree in [Your Field].  
- Internship/Job at Quorum Software – worked on EC2 automation and CI/CD.  
- Personal projects in Python, Flask, and DevOps tools.  
- Proficient in Git, JMeter, Selenium, and cloud infrastructure.

**3. Why DevOps?**  
I chose DevOps because it bridges development and operations. I enjoy automating repetitive tasks, improving deployment cycles, and solving system-level problems.

**4. What did you do at Quorum Software?**  
I worked on an EC2 automation project using AWS Lambda and Jenkins. My responsibilities included writing scripts, securing AWS resources, and ensuring seamless integration with Jenkins.

**5. Describe a challenge and solution:**  
We had an EC2 instance not triggering via Lambda. I debugged permissions, updated IAM roles, and improved monitoring using CloudWatch to ensure reliability.

**6. Biggest achievement so far:**  
Successfully built and deployed a complete CI/CD pipeline using Jenkins and Docker that reduced deployment time by 70%.

**7. Staying updated with tech:**  
I follow DevOps YouTube channels, read AWS and Docker blogs, and engage in hands-on projects.

**8. Project you’re proud of:**  
My YouTube Transcript Summarizer—it solves a real problem and combines Flask, REST APIs, and NLP.

**9. Team collaboration:**  
In my projects, I facilitated communication between backend and infrastructure teams using Slack, Git, and regular standups.

**10. What would you improve in past projects?**  
I’d focus more on modular design and error handling from the beginning.

---

### 🔹 **Day 2: AWS + EC2 Automation Project**

**1. EC2 Automation Project:**  
Created an automation pipeline where Jenkins triggers AWS Lambda, which starts EC2 instances based on cron jobs and performs health checks.

**2. EC2 Instance Types:**  
Used `t2.micro` for testing due to its cost-efficiency and `t3.medium` for production for better performance.

**3. AWS Lambda Scheduling:**  
Used CloudWatch Events (cron expression) to schedule Lambda for automatic instance control.

**4. IAM Roles in Automation:**  
Defined roles with least privilege for Lambda and EC2—ensuring only necessary permissions were granted.

**5. Benefit of AWS cron jobs:**  
Automates repetitive tasks like backups, EC2 scaling, and cleanup—saves manual effort and ensures consistency.

**6. EC2 Security:**  
Configured key pairs, used security groups, disabled SSH root login, and used IAM for access control.

**7. EC2 Stop vs Terminate:**  
Stop retains instance data and billing for EBS; terminate deletes instance and storage.

**8. Lambda fails to start EC2:**  
Monitored using CloudWatch logs; ensured EC2 start permissions and correct instance IDs.

**9. Monitor EC2:**  
Used CloudWatch for CPU/memory utilization, and custom scripts to trigger alerts.

**10. Jenkins & Lambda Integration:**  
Used Jenkins pipeline scripts with AWS CLI commands to invoke Lambda using API Gateway.

---

### 🔹 **Day 3: Docker + Jenkins + Git**

**1. Docker Image vs Container:**  
Image is a blueprint; container is a running instance of that image.

**2. Create Dockerfile:**  
Wrote a `Dockerfile` with base image, environment setup, and commands to install dependencies and expose ports.

**3. Docker in DevOps:**  
Standardizes environments, speeds up testing, ensures scalability across stages.

**4. Docker Compose:**  
Used to define and manage multi-container apps using `docker-compose.yml`.

**5. Jenkins Plugins Used:**  
Git plugin, Docker plugin, Pipeline, Blue Ocean for UI.

**6. Jenkins CI/CD Pipeline:**  
Stages: Code Pull → Build → Test → Dockerize → Deploy.

**7. Trigger Jenkins Build via GitHub:**  
Used webhooks in GitHub and configured Jenkins to poll SCM or listen to GitHub triggers.

**8. Resolve Git Conflicts:**  
Pulled the latest changes, resolved manually using VS Code or CLI, committed and pushed.

**9. Merge vs Rebase:**  
Merge retains history; rebase keeps it linear—used based on team strategy.

**10. Jenkins Build Failed:**  
Analyzed logs, fixed the Dockerfile error causing build fail, re-ran pipeline.

---

### 🔹 **Day 4: Performance Testing (JMeter & Selenium)**

**1. JMeter Test Plan Components:**  
Thread groups, samplers, listeners, assertions, config elements.

**2. Analyze JMeter Report:**  
Focused on throughput, response time, and error % using Summary Report and Graph Results.

**3. Thread Groups:**  
Used to simulate concurrent users; configured number of users, ramp-up, and loop count.

**4. CSV in JMeter:**  
Used CSV Data Set Config to parameterize test inputs (usernames, URLs).

**5. Metrics Compared:**  
Avg. response time, errors, throughput in baseline vs updated versions.

**6. Selenium for Performance:**  
Automated user interactions, monitored loading speed, DOM rendering time.

**7. Handle Dynamic Elements:**  
Used XPath, `WebDriverWait`, and custom logic to handle changing IDs.

**8. Implicit vs Explicit Wait:**  
Implicit waits globally; explicit waits for specific elements/conditions.

**9. Selenium with Python:**  
Used `selenium` package, `webdriver`, and integrated with `unittest` for testing flow.

**10. Frontend Performance with Selenium:**  
Logged timestamps at key events and calculated load/render times.

---

### 🔹 **Day 5: Python Projects + APIs + Tools**

**1. YouTube Transcript Summarizer:**  
Used `youtube-transcript-api` to fetch transcript → NLP summarization → displayed via Flask web app.

**2. Flask Use:**  
Developed REST APIs and lightweight web interfaces using Flask routes.

**3. Consume REST API:**  
Used `requests.get()` and `requests.post()` with headers and data payloads.

**4. Google Translate API:**  
Integrated via `googletrans` to auto-detect and translate text.

**5. requests.get vs post:**  
GET fetches data; POST sends data to server (used for form submissions or payloads).

**6. Error Handling:**  
Used `try-except`, `logging`, and fallback logic for API failures.

**7. JSON Parsing:**  
Used `json.loads()` and dictionary access to work with API responses.

**8. Purpose of openpyxl:**  
Read/write Excel files in automation tasks (reporting, data logging).

**9. Compare CSV with pandas:**  
Loaded CSVs into DataFrames → used `merge()` and `compare()` for differences.

**10. Python Automation Libraries:**  
Used `pandas`, `requests`, `openpyxl`, `selenium`, `schedule`.

---

### 🔹 **Day 6: Data Analytics + Visualization**

**1. Use of pandas:**  
For data cleaning, transformation, aggregation, and quick stats.

**2. Handle Missing Values:**  
Used `.fillna()`, `.dropna()`, or imputation techniques.

**3. Series vs DataFrame:**  
Series = 1D labeled array; DataFrame = 2D table of Series.

**4. Plot with matplotlib:**  
Used `pyplot.plot()`, `bar()`, `hist()`, and `show()` for visualizations.

**5. Visualization Types:**  
Line charts (trends), bar graphs (comparison), pie charts (distribution), heatmaps.

**6. Data Viz Decision Example:**  
Visualized test performance across builds—identified bottlenecks via bar graph.

**7. NumPy vs pandas:**  
NumPy is for numeric arrays and matrix operations; pandas adds tabular structure.

**8. Merge DataFrames:**  
Used `pd.merge()` on keys (inner, outer joins).

**9. groupby Use:**  
Grouped data by category and aggregated with `.sum()`, `.mean()`.

**10. Export DataFrame:**  
Used `.to_csv()` or `.to_excel()`.

---

### 🔹 **Day 7: System Knowledge + Soft Skills + HR Round**

**1. Basic Linux Commands:**  
`ls`, `cd`, `pwd`, `ps`, `top`, `chmod`, `crontab -e`.

**2. Crontab Task Scheduling:**  
`crontab -e` to set up tasks using time patterns (e.g., `0 2 * * *` for daily 2 AM).

**3. Ubuntu vs Windows:**  
Ubuntu is more CLI-based, lightweight, and suited for automation. Windows is GUI-centric.

**4. Check Running Processes:**  
`ps aux`, `top`, `htop`.

**5. Why this company?**  
Your innovative work culture, focus on DevOps, and continuous learning opportunities resonate with my passion.

**6. 2-3 Years Vision:**  
Become a senior DevOps engineer, leading automation initiatives and mentoring new talent.

**7. Strengths & Weaknesses:**  
Strength: Quick learner, good under pressure.  
Weakness: Sometimes overanalyze issues—working on trusting first instincts more.

**8. Handle Deadlines/Stress:**  
Break down tasks, use priority matrices, communicate blockers early.

**9. Prioritize Multiple Projects:**  
Use Trello/Notion, categorize by urgency/impact, schedule accordingly.

**10. Why Hire Me?**  
I bring a strong foundation, proven automation experience, problem-solving attitude, and passion for learning.

---
