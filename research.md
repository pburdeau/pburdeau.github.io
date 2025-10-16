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

<div class="research-section" id="policy-impacts">
    <h2>Policy impacts of uncertainties in methane emissions estimates</h2>
    <span class="research-status">In Progress</span>
    
    <p class="research-intro">
    Investigating how uncertainties in methane emissions quantification affect policy decisions and mitigation strategies. This work uses statistical methods to characterize measurement uncertainties and assess their implications for climate policy and regulatory frameworks.
    </p>
</div>

<div class="research-section" id="statistical-inference">
    <h2>Statistical modeling for methane inventories</h2>
    <span class="research-status">In Progress</span>
    
    <p class="research-intro">
    Developing a statistical framework to estimate total emissions from heterogeneous measurement data. This work models emissions as a discrete-time stochastic process with intermittent activity and explicitly accounts for measurement noise, detection thresholds, and spatial aggregation across multiple sources.
    </p>
    
    <div class="research-links">
        <a href="/publications/?filter=statistical-inference" class="research-link secondary">Related Publications</a>
    </div>
</div>

<div class="research-section" id="gas-composition">
    <h2>High-resolution mapping of U.S. natural gas composition</h2>
    <span class="research-status published">Published</span>
    
    <p class="research-intro">
    Developed a spatio-temporal interpolation method combining kriging with production data to map natural gas composition across the United States at 2km resolution. This work reveals that methane loss rates have been underestimated by 7-54% in most basins due to compositional variability, and provides the first comprehensive assessment of co-emitted species beyond methane.
    </p>
    
    <div class="research-links">
        <a href="https://pburdeau.github.io/us_map_gas_composition/" class="research-link" target="_blank" rel="noopener">Interactive Map</a>
        <a href="https://github.com/pburdeau/us_gas_composition" class="research-link secondary" target="_blank" rel="noopener">Code</a>
        <a href="https://doi.org/10.5281/zenodo.17246906" class="research-link secondary" target="_blank" rel="noopener">DOI</a>
        <a href="/publications/?filter=gas-composition" class="research-link secondary">Related Publications</a>
    </div>
</div>

<div class="research-section" id="bu-model">
    <h2>Bottom-up methane emissions model</h2>
    <span class="research-status software">Software</span>
    
    <p class="research-intro">
    Modernized the Bottom-Up Analyzer for Source Emissions (BASE) model by translating it from MATLAB to Python and developing an automated pipeline to process GHGRP data. The model enables emissions analysis for any geographic region using shape-based scaling of facility-level activity data.
    </p>
    
    <div class="research-links">
        <a href="https://github.com/JSRuthe/BU_methane_model" class="research-link" target="_blank" rel="noopener">Code Repository</a>
    </div>
</div>

<div class="research-section" id="technology-evaluation">
    <h2>Methane measurement technology evaluation</h2>
    <span class="research-status published">Published</span>
    
    <p class="research-intro">
    Participated in controlled release experiments evaluating methane detection technologies across satellites, aircraft, and ground-based continuous monitoring systems. In Fall 2022, I spent one week in the field in Arizona, then led data analysis including determining wind criteria for filtering releases that could not be correctly quantified and improving the workflow and pipeline for different phases of the single-blind experiment. In 2024, I designed the complete release schedule for the TADI facility (TotalEnergies) in France and spent two weeks on-site in September 2024 managing the experimental campaign.
    </p>
    
    <div class="research-links">
        <a href="/publications/?filter=technology-evaluation" class="research-link secondary">Related Publications</a>
    </div>
</div>
