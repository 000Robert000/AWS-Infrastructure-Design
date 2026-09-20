<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MediCare Direct | AWS Infrastructure Blueprint</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      background-color: #0d1117;
      color: #e6edf3;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 20px;
    }
    .container {
      max-width: 1000px;
      margin: 0 auto;
    }
    .header {
      background: linear-gradient(135deg, #09203f 0%, #1e4570 100%);
      border: 1px solid #30363d;
      border-radius: 12px;
      padding: 30px;
      margin-bottom: 25px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.5);
    }
    .header h1 {
      color: #ffffff;
      margin: 0 0 10px 0;
      font-size: 2.2em;
      display: flex;
      align-items: center;
      gap: 12px;
    }
    .subtitle {
      color: #38bdf8;
      font-weight: 600;
      margin-bottom: 15px;
      font-size: 1.1em;
    }
    .meta-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      margin-top: 20px;
      background: rgba(0,0,0,0.3);
      padding: 15px;
      border-radius: 8px;
      border: 1px solid rgba(255,255,255,0.1);
    }
    .meta-item {
      font-size: 0.95em;
      color: #93c5fd;
    }
    .meta-item strong {
      color: #ffffff;
      display: block;
      font-size: 1em;
    }
    .card {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 10px;
      padding: 24px;
      margin-bottom: 25px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    .card h2 {
      color: #38bdf8;
      margin-top: 0;
      border-bottom: 1px solid #30363d;
      padding-bottom: 10px;
      font-size: 1.4em;
    }
    .video-container {
      border-radius: 8px;
      overflow: hidden;
      border: 1px solid #30363d;
      background: #000;
    }
    video {
      width: 100%;
      display: block;
    }
    .pdf-table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
    }
    .pdf-table th {
      background-color: #21262d;
      color: #ffffff;
      text-align: left;
      padding: 14px;
      border: 1px solid #30363d;
      font-size: 1em;
    }
    .pdf-table td {
      padding: 14px;
      border: 1px solid #30363d;
      color: #e6edf3;
      background-color: #161b22;
      font-size: 0.95em;
    }
    .pdf-table td strong {
      color: #ffffff;
    }
    .btn-download {
      display: inline-block;
      background: #0284c7;
      color: #ffffff !important;
      font-weight: bold;
      padding: 10px 18px;
      border-radius: 6px;
      text-decoration: none !important;
      transition: background 0.2s;
    }
    .btn-download:hover {
      background: #0369a1;
    }
    .badge-container {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
      margin-top: 12px;
    }
    .badge {
      background: #21262d;
      border: 1px solid #38bdf8;
      color: #38bdf8;
      padding: 6px 12px;
      border-radius: 20px;
      font-size: 0.85em;
      font-family: monospace;
    }
    ul li {
      margin-bottom: 8px;
    }
  </style>
</head>
<body>

<div class="container">

  <div class="header">
    <h1>🏥 MediCare Direct</h1>
    <div class="subtitle">AWS 3-Tier Enterprise Healthcare Cloud Infrastructure</div>
    <p style="margin: 0; color: #cbd5e1; font-size: 1em;">
      An enterprise outpatient clinic management system digitizing patient scheduling, clinical queues, and EHR access within an isolated Virtual Private Cloud[cite: 8].
    </p>
    
    <div class="meta-grid">
      <div class="meta-item">
        <strong>Student Name</strong>
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
            <a href="SAM10_System_Proposal_Santiago.pdf" class="btn-download" target="_blank">📄 View PDF</a>[cite: 10]
          </td>
        </tr>
        <tr>
          <td><strong>Deliverable 2: AWS Architecture Diagram</strong>[cite: 9]</td>
          <td>Visual 3-tier VPC architecture diagram, subnet boundaries, and security group chaining[cite: 9].</td>
          <td style="text-align: center;">
            <a href="SAM10_AWS_Architecture_Diagram_Santiago.pdf" class="btn-download" target="_blank">📄 View PDF</a>[cite: 9]
          </td>
        </tr>
        <tr>
          <td><strong>Deliverable 3: Infrastructure Document</strong>[cite: 8]</td>
          <td>Comprehensive 4-page blueprint covering compute sizing, storage lifecycle, and cost analysis[cite: 8].</td>
          <td style="text-align: center;">
            <a href="SAM10_Infrastructure_Design_Document_Santiago.pdf" class="btn-download" target="_blank">📄 View PDF</a>[cite: 8]
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
    <ul style="margin-top: 18px; padding-left: 20px;">
      <li><strong>Subnet Isolation:</strong> Web proxy tier (`t3.micro`)[cite: 8], Application API tier (`t3.small`)[cite: 8], and PostgreSQL DB tier (`t3.small`)[cite: 8] isolated into distinct subnets[cite: 8].</li>
      <li><strong>Security Group Chaining:</strong> Strictly controls traffic flows (`sg-WebTier` ➔ `sg-AppTier` ➔ `sg-DBTier`)[cite: 8].</li>
      <li><strong>Zero Open SSH:</strong> Closed Port 22; administration enforced via AWS SSM Session Manager with hardware MFA[cite: 8].</li>
    </ul>
  </div>

</div>

</body>
</html>
