---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

<style>
.software-container {
  max-width: 1000px;
  margin: 0 auto;
}

.project-card {
  background: #fff;
  border: 1px solid rgba(150,150,150,0.2);
  border-radius: 8px;
  padding: 2.5em;
  margin: 2em 0;
  transition: box-shadow 0.3s ease;
}

.project-card:hover {
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
}

.project-header {
  margin-bottom: 1.5em;
}

.project-title {
  font-size: 2em;
  font-weight: 700;
  margin: 0 0 0.3em 0;
  color: #2c3e50;
}

.project-subtitle {
  font-size: 1.1em;
  color: #8C1515;
  font-weight: 500;
  margin: 0 0 1em 0;
}

.project-summary {
  font-size: 1.05em;
  line-height: 1.7;
  color: #555;
  margin-bottom: 2em;
}

.project-image {
  margin: 2em 0;
  text-align: center;
}

.project-image img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  border: 1px solid rgba(150,150,150,0.15);
}

.features-section {
  margin: 2em 0;
}

.features-section h3 {
  font-size: 1.2em;
  font-weight: 600;
  margin-bottom: 0.8em;
  color: #333;
}

.features-list {
  list-style: none;
  padding: 0;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 0.6em;
}

.features-list li {
  padding-left: 1.5em;
  position: relative;
  color: #555;
  line-height: 1.6;
}

.features-list li:before {
  content: "▸";
  position: absolute;
  left: 0;
  color: #8C1515;
  font-weight: bold;
}

.tech-section {
  margin: 2em 0;
}

.tech-section h3 {
  font-size: 1.2em;
  font-weight: 600;
  margin-bottom: 0.8em;
  color: #333;
}

.tech-pills {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6em;
}

.tech-pill {
  display: inline-block;
  padding: 6px 14px;
  background: #f5f5f5;
  border: 1px solid rgba(150,150,150,0.2);
  border-radius: 20px;
  font-size: 0.9em;
  font-weight: 500;
  color: #555;
}

.project-links {
  margin-top: 2em;
  display: flex;
  flex-wrap: wrap;
  gap: 1em;
}

.project-link {
  display: inline-block;
  padding: 10px 24px;
  background: #8C1515;
  color: white !important;
  text-decoration: none !important;
  border-radius: 6px;
  font-weight: 600;
  font-size: 0.95em;
  transition: background 0.3s ease;
}

.project-link:hover {
  background: #6d0f11;
}

.project-link.secondary {
  background: #f5f5f5;
  color: #333 !important;
  border: 1px solid rgba(150,150,150,0.3);
}

.project-link.secondary:hover {
  background: #e8e8e8;
}

.github-badges {
  margin: 1.5em 0;
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em;
  align-items: center;
}

@media (prefers-color-scheme: dark) {
  .project-card {
    background: #1a1a1a;
    border-color: rgba(255,255,255,0.1);
  }
  
  .project-title {
    color: #e0e0e0;
  }
  
  .project-subtitle {
    color: #d45555;
  }
  
  .project-summary {
    color: #aaa;
  }
  
  .features-section h3,
  .tech-section h3 {
    color: #ddd;
  }
  
  .features-list li {
    color: #aaa;
  }
  
  .tech-pill {
    background: #2a2a2a;
    border-color: rgba(255,255,255,0.1);
    color: #aaa;
  }
  
  .project-link.secondary {
    background: #2a2a2a;
    color: #ddd !important;
    border-color: rgba(255,255,255,0.1);
  }
  
  .project-link.secondary:hover {
    background: #333;
  }
}

@media (max-width: 768px) {
  .project-card {
    padding: 1.5em;
  }
  
  .project-title {
    font-size: 1.6em;
  }
  
  .features-list {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="software-container">

<div class="project-card">
  <div class="project-header">
    <h2 class="project-title">SCALPEL</h2>
    <p class="project-subtitle">Single-Cell Alternative PoLyadenylation and Isoform ExpLoration</p>
  </div>
  
  <p class="project-summary">
    SCALPEL is a scalable computational framework for transcript isoform quantification and alternative polyadenylation analysis at single-cell resolution. Built with Nextflow, it provides a robust pipeline for characterizing post-transcriptional regulation in complex biological systems using 3'-tagged scRNA-seq data.
  </p>
  
  <div class="github-badges">
    <img src="https://img.shields.io/github/stars/plasslab/SCALPEL?style=social" alt="GitHub stars">
    <img src="https://img.shields.io/github/license/plasslab/SCALPEL" alt="License">
    <img src="https://img.shields.io/github/last-commit/plasslab/SCALPEL" alt="Last commit">
  </div>
  
  <div class="project-image">
    <img src="https://raw.githubusercontent.com/plasslab/SCALPEL/main/docs/SCALPEL_diagram.png" alt="SCALPEL Pipeline Workflow">
  </div>
  
  <div class="features-section">
    <h3>Key Features</h3>
    <ul class="features-list">
      <li>Isoform quantification at single-cell resolution</li>
      <li>Alternative polyadenylation site identification and analysis</li>
      <li>Differential isoform usage analysis across cell types</li>
      <li>Reproducible Nextflow workflows with full containerization</li>
      <li>Scalable execution on HPC clusters and cloud platforms</li>
      <li>Integration with 10x Chromium and Drop-seq platforms</li>
      <li>Comprehensive quality control and visualization modules</li>
      <li>nf-core-oriented design principles</li>
    </ul>
  </div>
  
  <div class="tech-section">
    <h3>Technologies</h3>
    <div class="tech-pills">
      <span class="tech-pill">Nextflow</span>
      <span class="tech-pill">Python</span>
      <span class="tech-pill">R</span>
      <span class="tech-pill">Docker</span>
      <span class="tech-pill">Singularity</span>
      <span class="tech-pill">scRNA-seq</span>
      <span class="tech-pill">Bioconductor</span>
      <span class="tech-pill">HPC/Cloud</span>
    </div>
  </div>
  
  <div class="project-links">
    <a href="https://github.com/plasslab/SCALPEL" class="project-link" target="_blank">
      <svg width="16" height="16" viewBox="0 0 16 16" fill="currentColor" style="vertical-align: text-bottom; margin-right: 6px;">
        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/>
      </svg>
      GitHub Repository
    </a>
    <a href="https://doi.org/10.1038/s41467-025-06402-w" class="project-link secondary" target="_blank">📄 Nature Communications Paper</a>
    <a href="https://zenodo.org/records/15717636" class="project-link secondary" target="_blank">📦 Zenodo Container</a>
  </div>
</div>

<div style="margin-top: 3em; padding-top: 2em; border-top: 1px solid rgba(150,150,150,0.2);">
  <h3 style="font-size: 1.1em; font-weight: 600; color: #555; margin-bottom: 0.5em;">Additional Contributions</h3>
  <p style="color: #666; line-height: 1.7;">
    As a <strong>Nextflow Ambassador</strong> and active member of the nf-core community, I contribute to pipeline development, best practices documentation, and community training. All code is open-source and available on <a href="https://github.com/franzake" style="color: #8C1515;">GitHub</a>.
  </p>
</div>

</div>
