---
title: "Skills"
permalink: /skills/
layout: default
author_profile: false
classes: wide
---

<div class="wrap" markdown="1">

<style>
/* ===== Layout ===== */
.page-grid{
  display:grid;
  grid-template-columns:260px 1fr;
  gap:28px;
  align-items:start;
}
@media(max-width:900px){
  .page-grid{grid-template-columns:1fr;}
}

/* ===== Author card ===== */
.author-card{
  position:sticky;
  top:90px;
  border:1px solid #e5e7eb;
  border-radius:14px;
  padding:16px;
  background:#fff;
}
@media(max-width:900px){
  .author-card{position:static;}
}
.author-avatar{
  width:110px;height:110px;border-radius:999px;
  object-fit:cover;display:block;margin:0 auto 10px;
}
.author-name{text-align:center;font-weight:800;margin:0;}
.author-bio{text-align:center;color:#6b7280;margin:6px 0 12px;font-size:.95rem;}
.author-links{list-style:none;padding:0;margin:0;}
.author-links li{margin:8px 0;}
.author-links a{display:inline-flex;gap:8px;align-items:center;text-decoration:none;}

/* ===== Skills table ===== */
.skills-table{
  width:100%;
  border:1px solid #e5e7eb;
  border-radius:16px;
  overflow:hidden;
  background:#fff;
}

.skill-row{
  display:grid;
  grid-template-columns: 130px 260px 1fr;
  gap:18px;
  padding:16px;
  border-bottom:1px solid #f1f5f9;
  align-items:center;
}
.skill-row:last-child{border-bottom:none;}

@media(max-width:900px){
  .skill-row{
    grid-template-columns: 1fr;
    gap:12px;
  }
}

/* ===== Logo ===== */
.skill-logo{
  width:120px;height:90px;
  border:1px solid #e5e7eb;
  border-radius:14px;
  display:flex;align-items:center;justify-content:center;
  padding:12px;background:#fff;
}
.skill-logo img{
  max-width:100%;
  max-height:100%;
  object-fit:contain;
}

/* ===== Bar ===== */
.skill-bar{
  height:14px;
  border-radius:999px;
  background:#eef2f7;
  overflow:hidden;
  border:1px solid #e5e7eb;
}
.skill-fill{
  height:100%;
  border-radius:999px;
  background:linear-gradient(90deg,#2563eb,#22c55e);
}

/* ===== Text ===== */
.skill-title{
  font-weight:800;
  margin:0 0 6px 0;
}
.skill-desc{
  margin:0;
  color:#6b7280;
  line-height:1.4;
}
</style>

<div class="page-grid">

<!-- LEFT -->
<aside class="author-card">
  <img class="author-avatar" src="/assets/images/profile.jpg">
  <p class="author-name">Abu Bakkar Siddiq</p>
  <p class="author-bio">MS Student, UT Dallas</p>
  <ul class="author-links">
    <li><a href="mailto:piashsiddiq@gmail.com"><i class="fas fa-envelope"></i>Email</a></li>
    <li><a href="https://github.com/piashsiddiq" target="_blank"><i class="fab fa-github"></i>GitHub</a></li>
    <li><a href="https://www.linkedin.com/in/abu-siddiq-bakkar/" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a></li>
  </ul>
</aside>

<!-- RIGHT -->
<main>

<div class="skills-table">

<!-- SAP S/4HANA -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/sap-s4hana-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:95%"></div></div>
  <div>
    <p class="skill-title">SAP S/4HANA</p>
    <p class="skill-desc">
      End-to-end financial transaction processing, general & adjusting journal entries,
      financial statement generation (Income Statement, Balance Sheet), and ERP implementation support.
    </p>
  </div>
</div>

<!-- Oracle ERP -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/oracle-erp-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:75%"></div></div>
  <div>
    <p class="skill-title">Oracle ERP</p>
    <p class="skill-desc">
      General ledger operations and financial transaction processing within
      enterprise ERP environments.
    </p>
  </div>
</div>

<!-- QuickBooks -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/quickbooks-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>
  <div>
    <p class="skill-title">QuickBooks</p>
    <p class="skill-desc">
      Full-cycle Accounts Receivable and Accounts Payable management, journal entries,
      payment processing, and bank/vendor reconciliations.
    </p>
  </div>
</div>

<!-- Tally -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/tally-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:80%"></div></div>
  <div>
    <p class="skill-title">Tally</p>
    <p class="skill-desc">
      Bookkeeping, ledger maintenance, and day-to-day accounting entries.
    </p>
  </div>
</div>

<div class="skill-row">
  <!-- Logo -->
  <div class="skill-logo">
    <img src="/assets/images/logos/excel-logo.png" alt="Microsoft Excel">
  </div>

  <!-- Skill level -->
  <div class="skill-barwrap">
    <div class="skill-bar">
      <div class="skill-fill" style="width:95%;"></div>
    </div>
  </div>

  <!-- Description -->
  <div class="skill-meta">
    <p class="skill-title">Advanced Microsoft Excel</p>
    <p class="skill-desc">
      Advanced financial modeling and reporting using Pivot Tables, Power Query, Power Pivot,
      VLOOKUP/XLOOKUP, SUMIFS, and INDEX-MATCH for variance analysis and dashboard automation.
    </p>
  </div>
</div>

<!-- Power BI -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/power-bi-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>
  <div>
    <p class="skill-title">Power BI</p>
    <p class="skill-desc">
      Interactive dashboard development for sales-vs-target tracking, Accounts Receivable
      aging analysis, and management reporting.
    </p>
  </div>
</div>

<!-- Tableau -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/tableau-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:80%"></div></div>
  <div>
    <p class="skill-title">Tableau</p>
    <p class="skill-desc">
      Data visualization and business analytics dashboards to support performance
      monitoring and decision-making.
    </p>
  </div>
</div>

<!-- SQL -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/sql-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:80%"></div></div>
  <div>
    <p class="skill-title">SQL</p>
    <p class="skill-desc">
      Querying and structuring business data for reporting, analysis,
      and business intelligence workflows.
    </p>
  </div>
</div>

<!-- Python -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/Python-logo-notext.svg.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:75%"></div></div>
  <div>
    <p class="skill-title">Python</p>
    <p class="skill-desc">
      Data cleaning, validation, and AI/ML-assisted report automation, including
      classification modeling for fraud detection.
    </p>
  </div>
</div>

<!-- R -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/r-logo.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:75%"></div></div>
  <div>
    <p class="skill-title">R</p>
    <p class="skill-desc">
      Statistical and machine learning analysis, including classification modeling
      (Logistic Regression, Decision Tree, k-NN) using caret, ggplot2, and dplyr.
    </p>
  </div>
</div>

<!-- Financial Reporting -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/financial-reporting-icon.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:95%"></div></div>
  <div>
    <p class="skill-title">Financial Reporting &amp; Statement Analysis</p>
    <p class="skill-desc">
      Preparation and analysis of Income Statements, Balance Sheets, and Cash Flow
      Statements to support senior management decision-making.
    </p>
  </div>
</div>

<!-- General Ledger -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/general-ledger-icon.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>
  <div>
    <p class="skill-title">General Ledger &amp; Bank Reconciliation</p>
    <p class="skill-desc">
      General ledger maintenance, chart of accounts management, and bank reconciliations
      across ERP and accounting platforms.
    </p>
  </div>
</div>

<!-- AR/AP -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/ar-ap-icon.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>
  <div>
    <p class="skill-title">Accounts Receivable / Payable &amp; Aging Analysis</p>
    <p class="skill-desc">
      Accounts Receivable/Payable management, vendor reconciliations, and aging report
      analysis to strengthen collections and cash flow.
    </p>
  </div>
</div>

<!-- Budgeting & Variance -->
<div class="skill-row">
  <div class="skill-logo"><img src="/assets/images/logos/budgeting-icon.png"></div>
  <div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div>
  <div>
    <p class="skill-title">Budgeting &amp; Variance Analysis</p>
    <p class="skill-desc">
      Budget-to-actual variance analysis, overhead cost analysis, and profitability
      analysis to optimize contribution margins and control costs.
    </p>
  </div>
</div>

</div>

</main>

</div>
</div>
