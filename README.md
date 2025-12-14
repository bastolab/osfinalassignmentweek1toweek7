CMPN202 Operating Systems Coursework Repository
A comprehensive GitHub repository solution for the CMPN202 Operating Systems coursework assessment, providing an integrated documentation framework and automated tooling for security auditing and system monitoring in accordance with Assessment Brief CMPN202 Operating Systems Coursework_v010.pdf.
Repository Architecture
Documentation Framework (docs/)

Production-ready GitHub Pages static site with Jekyll integration
Structured homepage with project overview and navigation architecture
Dedicated documentation pages for weekly deliverables (Weeks 1–7)
Pre-configured site metadata and styling templates

Automation Toolkit (scripts/)

security-baseline.sh – Automated security baseline verification script for server-side deployment (Phases 4–5 compliance)
monitor-server.sh – Remote monitoring utility for SSH-based metric collection and aggregation

Data Management (data/)

Structured templates for performance metric collection
Designated storage for audit trails and empirical testing results

Reference Documentation

Complete coursework assessment brief (PDF format)

Deployment Instructions
GitHub Pages Configuration

Initialize repository in your GitHub account
Access repository Settings → Pages configuration panel
Configure deployment source: main branch, /docs directory
Retrieve and verify the auto-generated GitHub Pages URL

Script Execution Procedures
Server-Side Security Audit:
bashchmod +x scripts/security-baseline.sh
./scripts/security-baseline.sh | tee security-baseline-report.txt
Workstation-Based Remote Monitoring:
bashchmod +x scripts/monitor-server.sh
./scripts/monitor-server.sh user@server-ip data/perf-sample.csv 30
Customisation Requirements
To adapt this repository for your specific implementation:

Replace all placeholder identifiers (YOUR_STUDENT_ID, temporal references, network addresses, distribution specifications)
Integrate visual documentation by placing screenshots in docs/assets/ with appropriate markdown references
Populate data/performance-template.csv with empirical data from your system benchmarking activities
Adapt automation scripts to accommodate distribution-specific package managers, service nomenclature, and system utilities

Assessment Deliverables
As specified in the coursework brief, your submission must include:

 Functional GitHub Pages site comprising homepage and seven weekly documentation sections
 StudentID_GitHub_URL.txt containing your published documentation site URL
 StudentID_OSCoursework_Demonstration.mp4 video demonstration (not exceeding 8 minutes duration)
 Comprehensive evidence demonstrating security control implementation, monitoring infrastructure deployment, performance analysis methodology, system optimisation procedures, and critical reflective analysis
