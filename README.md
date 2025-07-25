# NetVizOps
This is a simple project I am making to use multiple new networking tools I have not used yet. The main focus is to get familiar with these concepts and manage a server hosted by my computer and a couple VMs I also have running. This project completes all the requirements for the job posting posted by Charter Specturm for an intro level software engineer.


## Roadmap:
I plan to handle each step in about a week or two depending on how difficult they become. My estimate for project completion is about 6 weeks maybe more. I hope to be done by some time in november. 
### Step 0:Environment Setup:
- Instal VirtualBox and set up 3 Ubuntu VMs to simulate traffic with
- Instal Docker + Docker compose
- Create Github repo
- Create VSCode workspace on local machiene
- Set up Kuberneties (research pending)

### Step 1: Core Backend
- Create Python database abd queue
- Build python service to collect and normallize SNMP metrics
- Store Real-time + historical data in PostgreSQL and Redis
- Use MongoDB for ustructured logs
- Connect services using Kafkka or RabbitMQ
- Write unit tests for integration and storage logic

### Step 2: API Layer
- Expose REST APIs for data queries, thresholds and admin actions
- Protect endpoints with simple auth
- Create test suite for all endpoints usings TDD

### Step 3: Front End Web App:
- Create a react dashboard for
  - System Status
  - Threshold allerts
  - Graphs (From REST APIs)
- Use Docker to package and server frontend
  
### Step 4: Admin Panel in PHP
- Create a simple PHP admin interface
- Handle User management
- Handle Cnfiguration updates
- handle Log viewer

### Step 5: Monitoring and Metrics
- Set up SNMP agents in VMs to simulate routers/devices
- SNMP poller sends data to Kafka → DB
- Grafana for live metrics dashboards
- Export CSVs to simulate Tableau dashboards
- Route logs to syslog → forward to Splunk for analysis

### Step 6: DevOps and Automation
- Containerize all services (Python, frontend, PHP admin, databases)
- Define k8s manifests (pods, services, volumes)
- Set up GitHub Actions for CI (build + tests)
- Simulate Agile with a public Kanban board (Jir

## End Goals:
The project...
1. Monitors virtualized network activity
2. Collects and displayes real-time metrics and logs
3. Supports RESTful APIs for metrics and querying control
4. Includes user/admin web interface
5. Implements message queues, persistant storage, and role-based alerts
   
## Tools Used and Learned in this project:
- Languanges: *Python, PHP, JavaScript*
- Databases: *MySQL, PostgreSQL*
- Queues: *RabbitMQ/Kafka*
- Frontend: *React, PHP, REST APIs*
- Infastructure: *Docker, Kuberneties, VMs (VirtualBox), Linux*
- Montoring: *Grafana, Tableu, SNMP*
- Logging: *Splunk, Syslog*
- DevPractices: *GitHub, VSCode, Test-Driven Development, Agile Development*
- Other Tools: *jira (issue tracking), remedy (optional simulation), SNMP agents*
