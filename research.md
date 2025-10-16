---
layout: default
title: "Research"
permalink: /research/
---

<style>
.research-section {
    margin: 48px 0;
    padding-bottom: 32px;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
}

.research-section:last-child {
    border-bottom: none;
}

.research-section h2 {
    font-size: 24px;
    font-weight: 700;
    margin: 0 0 8px;
    color: var(--ink);
}

.research-status {
    display: inline-block;
    font-size: 13px;
    font-weight: 600;
    padding: 4px 12px;
    border-radius: 16px;
    background: #D97706;
    color: white;
    margin-bottom: 12px;
}

.research-status.published {
    background: #059669;
}

.research-status.software {
    background: #7C3AED;
}

.research-intro {
    font-size: 18px;
    line-height: 1.7;
    margin: 16px 0;
    color: #333;
}

.research-links {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
    margin: 16px 0;
}

.research-link {
    display: inline-block;
    padding: 8px 16px;
    background: var(--ink);
    color: white;
    text-decoration: none;
    border-radius: 6px;
    font-size: 14px;
    font-weight: 600;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.research-link:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.research-link.secondary {
    background: transparent;
    color: var(--ink);
    border: 2px solid var(--ink);
}

.research-link.secondary:hover {
    background: var(--ink);
    color: white;
}

@media (max-width: 768px) {
    .research-section h2 {
        font-size: 20px;
    }
    
    .research-intro {
        font-size: 16px;
    }
    
    .research-links {
        flex-direction: column;
    }
    
    .research-link {
        text-align: center;
    }
}
</style>

<h1>Research</h1>

<p style="font-size: 20px; line-height: 1.7; margin: 24px 0 48px; color: #333;">
My research focuses on developing statistical methods and computational tools to better quantify and understand methane emissions from the oil and gas sector.
</p>

<div class="research-section">
    <h2>Policy impacts of uncertainties in methane emissions estimates</h2>
    <span class="research-status">In Progress</span>
    
    <p class="research-intro">
    Investigating how uncertainties in methane emissions quantification affect policy decisions and mitigation strategies. This work uses statistical methods to characterize measurement uncertainties and assess their implications for climate policy and regulatory frameworks.
    </p>
</div>

<div class="research-section">
    <h2>Statistical inference of intermittent methane emissions</h2>
    <span class="research-status">In Progress</span>
    
    <p class="research-intro">
    Developing advanced statistical methods for quantifying methane emissions from heterogeneous measurement data. This work combines geostatistics, Bayesian inference, and emission inventory reconciliation to better understand intermittent emission events from oil and gas infrastructure.
    </p>
</div>

<div class="research-section">
    <h2>High-resolution mapping of U.S. natural gas composition</h2>
    <span class="research-status published">Published</span>
    
    <p class="research-intro">
    Created the first comprehensive, high-resolution national map of natural gas composition across the United States. This work reveals substantial regional variations in greenhouse gas intensity and provides new estimates of methane leakage impacts.
    </p>
    
    <div class="research-links">
        <a href="https://pburdeau.github.io/us_map_gas_composition/" class="research-link" target="_blank" rel="noopener">Interactive Map</a>
        <a href="https://github.com/pburdeau/us_gas_composition" class="research-link secondary" target="_blank" rel="noopener">Code</a>
        <a href="https://doi.org/10.5281/zenodo.17246906" class="research-link secondary" target="_blank" rel="noopener">DOI</a>
        <a href="/publications/" class="research-link secondary">Publication</a>
    </div>
</div>

<div class="research-section">
    <h2>Bottom-up methane emissions model</h2>
    <span class="research-status software">Software</span>
    
    <p class="research-intro">
    Modernized the Bottom-Up Analyzer for Source Emissions (BASE) model by translating it from MATLAB to Python and developing an automated pipeline to process GHGRP data. The model now supports shape-based analysis for any geographic region and integrates comprehensive activity data from oil and gas operations.
    </p>
    
    <div class="research-links">
        <a href="https://github.com/JSRuthe/BU_methane_model" class="research-link" target="_blank" rel="noopener">Code Repository</a>
    </div>
</div>

<div class="research-section">
    <h2>Methane measurement technology evaluation</h2>
    <span class="research-status published">Published</span>
    
    <p class="research-intro">
    Contributed to multiple controlled release experiments evaluating methane detection technologies across satellites, aircraft, and ground-based continuous monitoring systems. These studies provide critical performance benchmarks for emerging measurement technologies.
    </p>
    
    <div class="research-links">
        <a href="/publications/" class="research-link">View Publications</a>
    </div>
</div>
