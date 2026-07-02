---
title: "Publications / Projects"
permalink: /pubs-projects/
layout: default
author_profile: false
classes: wide
---

<div class="wrap" markdown="1">

<style>
  /* ===== Page-only 2-column layout ===== */
  .page-grid{
    display: grid;
    grid-template-columns: 260px 1fr;
    gap: 28px;
    align-items: start;
  }
  @media (max-width: 900px){
    .page-grid{ grid-template-columns: 1fr; }
  }

  /* ===== Author card ===== */
  .author-card{
    position: sticky;
    top: 90px;
    border: 1px solid #e5e7eb;
    border-radius: 14px;
    padding: 16px;
    background: #fff;
  }
  @media (max-width: 900px){
    .author-card{ position: static; }
  }

  .author-avatar{
    width: 110px;
    height: 110px;
    border-radius: 999px;
    object-fit: cover;
    display: block;
    margin: 0 auto 10px auto;
  }
  .author-name{ text-align: center; font-weight: 800; margin: 0; }
  .author-bio{ text-align: center; color: #6b7280; margin: 6px 0 12px 0; font-size: 0.95rem; }
  .author-links{ list-style: none; padding: 0; margin: 0; }
  .author-links li{ margin: 8px 0; }
  .author-links a{ text-decoration: none; display: inline-flex; gap: 8px; align-items: center; }

  /* Red mark for missing info */
  .missing-note{
    display: inline-block;
    border: 1px dashed #ef4444;
    background: #fff5f5;
    color: #ef4444;
    border-radius: 8px;
    padding: 6px 10px;
    font-size: 0.85rem;
    font-weight: 600;
  }
</style>

<div class="page-grid">

  <!-- LEFT: manual author profile -->
  <aside class="author-card">
    <img class="author-avatar" src="/assets/images/profile.jpg" alt="Abu Bakkar Siddiq">
    <p class="author-name">Abu Bakkar Siddiq</p>
    <p class="author-bio">MS Student, UT Dallas</p>

    <ul class="author-links">
      <li><a href="mailto:piashsiddiq@gmail.com"><i class="fas fa-fw fa-envelope"></i><span>Email</span></a></li>
      <li><a href="https://github.com/piashsiddiq" target="_blank" rel="noopener"><i class="fab fa-fw fa-github"></i><span>GitHub</span></a></li>
      <li><a href="https://www.linkedin.com/in/abu-siddiq-bakkar/" target="_blank" rel="noopener"><i class="fab fa-fw fa-linkedin"></i><span>LinkedIn</span></a></li>
    </ul>
  </aside>

  <!-- RIGHT: your existing content -->
  <main markdown="1">

## <i class="fas fa-file-alt"></i> Publications

<div class="edu-timeline">

  <!-- Journal of Financial Crime submission -->
  <div class="edu-item">
    <div class="edu-content">
      <h3>A Business Analytics Framework for Credit Card Fraud Detection and Risk Profiling</h3>
      <div class="edu-meta">
        <span>Status: Under Review</span>
        <span>Journal of Financial Crime</span>
      </div>
      <p class="edu-inst">
        Co-authored with Dr. Rasoul Ramezani &middot; Submitted June 2026
      </p>
      <p class="edu-extra">
        A business analytics framework applying data-driven and machine-learning-based
        methods to credit card fraud detection and customer risk profiling, extending the
        classification-modeling approach developed during graduate coursework.
      </p>
    </div>
  </div>

</div>

---

## <i class="fas fa-diagram-project"></i> Projects

<div class="edu-timeline">

  <!-- Predicting Credit Card Fraud -->
  <div class="edu-item">
    <div class="edu-content">
      <h3>Predicting Credit Card Fraud</h3>
      <div class="edu-meta">
        <span>January 2025 – May 2025</span>
        <span>Course: Business Analytics with R</span>
      </div>
      <p class="edu-inst">The University of Texas at Dallas</p>

      <p class="edu-extra"><strong>Key Contributions:</strong></p>
      <ul class="edu-list">
        <li>Built and compared three ML classification models (Logistic Regression, Decision Tree, k-NN) in R on a dataset of 284,807 transactions, achieving 97%+ accuracy using SMOTE for class imbalance and ROC/AUC for model evaluation.</li>
        <li>Identified that 0.5 percent of fraudulent transactions clustered around low-dollar amounts during late-night hours in online and point-of-sale retail channels, informing actionable real-time fraud alert thresholds.</li>
      </ul>
      <p class="edu-extra"><strong>Tools:</strong> R (caret, ggplot2, dplyr, ROSE), SMOTE, CRISP-DM methodology.</p>
    </div>
  </div>

</div>

  </main>

</div>
</div>
