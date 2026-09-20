---
layout: default
title: MediCare Direct | AWS Infrastructure Blueprint
---

<style>
  :root {
    --bg-dark: #0d1117;
    --card-bg: #161b22;
    --border-color: #30363d;
    --accent-blue: #00f2fe;
    --accent-teal: #4facfe;
    --text-main: #c9d1d9;
    --text-bright: #ffffff;
    --text-muted: #8b949e;
  }

  body {
    background-color: var(--bg-dark) !important;
    color: var(--text-main) !important;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    line-height: 1.6;
  }

  .medical-header {
    background: linear-gradient(135deg, #09203f 0%, #537895 100%);
    border: 1px solid var(--border-color);
    border-radius: 12px;
    padding: 28px;
    margin-bottom: 25px;
    box-shadow: 0 8px 24px rgba(0,0,0,0.4);
  }

  .medical-header h1 {
    color: var(--text-bright);
    margin: 0 0 10px 0;
    font-size: 2em;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .subtitle {
    color: var(--accent-blue);
    font-weight: 600;
    margin-bottom: 15px;
    font-size: 1.1em;
  }

  .meta-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 12px;
    margin-top: 20px;
    background: rgba(0,0,0,0.2);
    padding: 15px;
    border-radius: 8px;
    border: 1px solid rgba(255,255,255,0.05);
  }

  .meta-item {
    font-size: 0.9em;
  }

  .meta-item strong {
    color: var(--text-bright);
    display: block;
  }

  .card {
    background: var(--card-bg);
    border: 1px solid var(--border-color);
    border-radius: 10px;
    padding: 20px;
    margin-bottom: 25px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
  }

  .card h2 {
    color: var(--accent-teal);
    margin-top: 0;
    border-bottom: 1px solid var(--border-color);
    padding-bottom: 8px;
    font-size: 1.4em;
  }

  .video-container {
    position: relative;
    border-radius: 8px;
    overflow: hidden;
    border: 1px solid var(--border-color);
  }

  video {
    width: 100%;
    display: block;
    background: #000;
  }

  .pdf-table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 10px;
  }

  .pdf-table th {
    background-color: #21262d;
    color: var(--text-bright);
    text-align: left;
    padding: 12px;
    border: 1px solid var(--border-color);
  }

  .pdf-table td {
    padding: 12px;
    border: 1px solid var(--border-color);
    color: var(--text-main);
  }

  .btn-download {
    display: inline-block;
    background: linear-gradient(135deg, #00f2fe 0%, #4facfe 100%);
    color: #000 !important;
    font-weight: bold;
    padding: 8px 14px;
    border-radius: 6px;
    text-decoration: none !important;
    transition: transform 0.2s, opacity 0.2s;
  }

  .btn-download:hover {
    opacity: 0.9;
    transform: translateY(-2px);
  }

  .badge-container {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    margin-top: 10px;
  }

  .badge {
    background: #21262d;
    border: 1px solid var(--border-color);
    color: var(--accent-blue);
    padding: 4px 10px;
    border-radius: 20px;
    font-size: 0.85em;
    font-family: monospace;
  }
</style>

<div class="medical-header">
  <h1>🏥 MediCare Direct</h1>
  <div class="subtitle">AWS 3-Tier Enterprise Healthcare Cloud Infrastructure[cite: 8]</div>
  <p style="margin: 0; color: #e1e4e8; font-size: 0.95em;">
    An enterprise outpatient clinic management system digitizing patient scheduling, clinical queues, and EHR access within an isolated, HIPAA-compliant Virtual Private Cloud[cite: 8].
  </p>
  
  <div class="meta-grid">
    <div class="meta-item">
      <strong>Student</strong>
      Robert Angel B. Santiago[cite: 8]
    </div>
    <div class="meta-item">
      <strong>Student ID</strong>
      23-1360-266[cite: 8]
    </div>
    <div class="meta-item">
      <strong>Course & Section</strong>
      BSIT-4-A (SAM10)[cite: 8]
    </div>
    <div class="meta-item">
      <strong>AWS Region</strong>
      ap-southeast-1[cite: 8]
    </div>
  </div>
</div>

<div class="card">
  <h2>📽️ Architecture Walkthrough & Video Demo</h2>
  <div class="video-container">
    <video controls poster="assets/video-thumbnail.png">
      <source src="demo-video.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

<div class="card">
  <h2>📑 Project Deliverables & Technical Blueprints</h2>
  <table class="pdf-table">
    <thead>
      <tr>
        <th>Deliverable</th>
        <th>Description</th>
        <th style="text-align: center;">Document</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Deliverable 1: System Proposal</strong>[cite: 10]</td>
        <td>System requirements mapping, service selections, and network topology justification[cite: 10].</td>
        <td style="text-align: center;">
          <a href="SAM10_System_Proposal_Santiago.pdf" class="btn-download" target="_blank">📥 View PDF</a>[cite: 10]
        </td>
      </tr>
      <tr>
        <td><strong>Deliverable 2: AWS Architecture Diagram</strong>[cite: 9]</td>
        <td>Visual 3-tier VPC architecture diagram, subnet boundaries, and security group chaining[cite: 9].</td>
        <td style="text-align: center;">
          <a href="SAM10_AWS_Architecture_Diagram_Santiago.pdf" class="btn-download" target="_blank">📥 View PDF</a>[cite: 9]
        </td>
      </tr>
      <tr>
        <td><strong>Deliverable 3: Infrastructure Document</strong>[cite: 8]</td>
        <td>Comprehensive 4-page blueprint covering compute sizing, storage lifecycle, and cost analysis[cite: 8].</td>
        <td style="text-align: center;">
          <a href="SAM10_Infrastructure_Design_Document_Santiago.pdf" class="btn-download" target="_blank">📥 View PDF</a>[cite: 8]
        </td>
      </tr>
    </tbody>
  </table>
</div>

<div class="card">
  <h2>🏗️ Core Infrastructure Highlights</h2>
  <div class="badge-container">
    <span class="badge">VPC: 10.0.0.0/16</span>[cite: 8]
    <span class="badge">Public Tier: 10.0.1.0/24</span>[cite: 8]
    <span class="badge">App Tier: 10.0.2.0/24</span>[cite: 8]
    <span class="badge">Data Tier: 10.0.3.0/24</span>[cite: 8]
    <span class="badge">Cost: $57.98/mo</span>[cite: 8]
  </div>
  <ul style="margin-top: 15px; padding-left: 20px;">
    <li><strong>Subnet Isolation:</strong> Web proxy tier (`t3.micro`)[cite: 8], Application API tier (`t3.small`)[cite: 8], and PostgreSQL DB tier (`t3.small`)[cite: 8] isolated into distinct subnets[cite: 8].</li>
    <li><strong>Security Group Chaining:</strong> Strictly controls traffic flows (`sg-WebTier` ➔ `sg-AppTier` ➔ `sg-DBTier`)[cite: 8].</li>
    <li><strong>Zero Open SSH:</strong> Closed Port 22; administration enforced via AWS SSM Session Manager with hardware MFA[cite: 8].</li>
  </ul>
</div>
