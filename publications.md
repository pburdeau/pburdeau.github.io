---
layout: default
title: "Publications"
permalink: /publications/
---

<style>
.pub-section {
    margin: 48px 0 24px;
}

.pub-section h2 {
    font-size: 22px;
    font-weight: 700;
    color: var(--ink);
    border-bottom: 2px solid var(--ink);
    display: inline-block;
    padding-bottom: 4px;
    margin-bottom: 24px;
}

.publication {
    margin: 32px 0;
    padding: 20px;
    background: #f9fafb;
    border-radius: 8px;
    border-left: 4px solid var(--ink);
}

.publication.hidden {
    display: none;
}

.pub-title {
    font-size: 18px;
    font-weight: 700;
    color: var(--ink);
    margin: 0 0 8px;
    line-height: 1.4;
}

.pub-authors {
    font-size: 15px;
    color: #444;
    margin: 8px 0;
    line-height: 1.6;
}

.pub-venue {
    font-size: 15px;
    font-style: italic;
    color: #666;
    margin: 8px 0;
}

.pub-links {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    margin-top: 12px;
}

.pub-link {
    display: inline-block;
    padding: 6px 14px;
    background: var(--ink);
    color: white;
    text-decoration: none;
    border-radius: 4px;
    font-size: 13px;
    font-weight: 600;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.pub-link:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.pub-status {
    display: inline-block;
    font-size: 12px;
    font-weight: 600;
    padding: 3px 10px;
    border-radius: 12px;
    background: #D97706;
    color: white;
    margin-left: 8px;
}

.pub-status.accepted {
    background: #059669;
}

.filter-toggle {
    display: flex;
    gap: 12px;
    margin: 24px 0;
    align-items: center;
    flex-wrap: wrap;
}

.filter-btn {
    padding: 8px 16px;
    background: transparent;
    color: var(--ink);
    border: 2px solid var(--ink);
    border-radius: 6px;
    font-size: 14px;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.2s ease;
}

.filter-btn:hover {
    background: var(--ink);
    color: white;
}

.filter-btn.active {
    background: var(--ink);
    color: white;
}

@media (max-width: 768px) {
    .publication {
        padding: 16px;
    }
    
    .pub-title {
        font-size: 16px;
    }
    
    .pub-authors, .pub-venue {
        font-size: 14px;
    }
    
    .pub-links {
        flex-direction: column;
    }
    
    .filter-toggle {
        flex-direction: column;
        align-items: flex-start;
    }
}
</style>

<h1>Publications</h1>

<div class="filter-toggle">
    <span style="font-weight: 600;">View:</span>
    <button class="filter-btn active" onclick="filterPublications('all', this)">All Publications</button>
    <button class="filter-btn" onclick="filterPublications('first', this)">First Author Only</button>
    <button class="filter-btn" onclick="filterPublications('gas-composition', this)">Gas Composition</button>
    <button class="filter-btn" onclick="filterPublications('statistical-inference', this)">Statistical Inference</button>
    <button class="filter-btn" onclick="filterPublications('technology-evaluation', this)">Technology Evaluation</button>
    <button class="filter-btn" onclick="filterPublications('bu-model', this)">Bottom-Up Model</button>
</div>

<div class="pub-section" id="gas-composition">
    <h2>Gas Composition Mapping</h2>
    
    <div class="publication" data-author-type="coauthor" data-project="gas-composition">
        <div class="pub-title">
            Carbon intensity of United States natural gas supply
            <span class="pub-status">In Review</span>
        </div>
        <div class="pub-authors">
            Zhang, Z., Rutherford, J., Littlefield, J., Ramadan, F., Ali Saafi, M., Ren, B., Y Jabbar, M., Saad, D., <strong>Burdeau, P.</strong>, Masnadi, M., Brandt, A.
        </div>
        <div class="pub-venue">
            Environmental Science & Technology (2025)
        </div>
    </div>
    
    <div class="publication" data-author-type="first" data-project="gas-composition">
        <div class="pub-title">
            High-resolution national mapping of natural gas composition substantially updates methane leakage impacts
            <span class="pub-status accepted">Accepted in Principle</span>
        </div>
        <div class="pub-authors">
            <strong>Burdeau, P.</strong>, Sherwin, E., Berman, E., Biraud, S., Brandt, A.
        </div>
        <div class="pub-venue">
            Nature Communications (2025)
        </div>
        <div class="pub-links">
            <a href="https://www.researchgate.net/publication/391799633_High-resolution_national_mapping_of_natural_gas_composition_substantially_updates_methane_leakage_impacts" class="pub-link" target="_blank" rel="noopener">Preprint</a>
        </div>
    </div>
</div>

<div class="pub-section" id="statistical-inference">
    <h2>Statistical Inference</h2>
    
    <div class="publication" data-author-type="first" data-project="statistical-inference">
        <div class="pub-title">
            Statistical inference of intermittent methane emissions from heterogeneous measurements
        </div>
        <div class="pub-authors">
            <strong>Burdeau, P.</strong>, McManemin, A., Sherwin, E., Wetherley, E., Berman, E., Brandt, A.
        </div>
        <div class="pub-venue">
            AGU Fall Meeting Abstracts, SY41C (2025)
        </div>
    </div>
</div>

<div class="pub-section" id="technology-evaluation">
    <h2>Technology Evaluation</h2>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Controlled release testing of commercially available methane emission measurement technologies at the TADI facility
            <span class="pub-status">In Review</span>
        </div>
        <div class="pub-authors">
            McManemin, A., Juéry, C., Blandin, V., France, J.L., <strong>Burdeau, P.</strong>, Brandt, A.
        </div>
        <div class="pub-venue">
            Atmospheric Measurement Techniques (2025)
        </div>
        <div class="pub-links">
            <a href="https://egusphere.copernicus.org/preprints/2025/egusphere-2025-3793/" class="pub-link" target="_blank" rel="noopener">Preprint</a>
        </div>
    </div>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Single-blind test of nine methane-sensing satellite systems from three continents
        </div>
        <div class="pub-authors">
            Sherwin, E., El Abbadi, S., <strong>Burdeau, P.</strong>, Zhang, Z., Chen, Z., Rutherford, J., Chen, Y., Brandt, A.
        </div>
        <div class="pub-venue">
            Atmospheric Measurement Techniques (2024)
        </div>
        <div class="pub-links">
            <a href="https://amt.copernicus.org/articles/17/765/2024/" class="pub-link" target="_blank" rel="noopener">Paper</a>
        </div>
    </div>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Technological maturity of aircraft-based methane sensing for greenhouse gas mitigation
        </div>
        <div class="pub-authors">
            El Abbadi, S., Chen, Z., <strong>Burdeau, P.</strong>, Rutherford, J., Chen, Y., Zhang, Z., Sherwin, E., Brandt, A.
        </div>
        <div class="pub-venue">
            Environmental Science & Technology (2024)
        </div>
        <div class="pub-links">
            <a href="https://pubs.acs.org/doi/full/10.1021/acs.est.4c02439" class="pub-link" target="_blank" rel="noopener">Paper</a>
        </div>
    </div>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Comparing continuous methane monitoring technologies for high-volume emissions: a single-blind controlled release study
        </div>
        <div class="pub-authors">
            Chen, Z., El Abbadi, S., Sherwin, E., <strong>Burdeau, P.</strong>, Rutherford, J., Chen, Y., Zhang, Z., Brandt, A.
        </div>
        <div class="pub-venue">
            ACS ES&T Air (2024)
        </div>
        <div class="pub-links">
            <a href="https://pubs.acs.org/doi/full/10.1021/acsestair.4c00015" class="pub-link" target="_blank" rel="noopener">Paper</a>
        </div>
    </div>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Comprehensive evaluation of aircraft-based methane sensing for greenhouse gas mitigation
        </div>
        <div class="pub-authors">
            El Abbadi, S., Chen, Z., <strong>Burdeau, P.</strong>, Rutherford, J., Chen, Y., Zhang, Z., Sherwin, E., Brandt, A.
        </div>
        <div class="pub-venue">
            EarthArXiv preprint (2023)
        </div>
        <div class="pub-links">
            <a href="https://www.researchgate.net/profile/Evan-Sherwin/publication/371769847_Comprehensive_evaluation_of_aircraft-based_methane_sensing_for_greenhouse_gas_mitigation/links/64dbff0e66f0e0067d99bd8d/Comprehensive-evaluation-of-aircraft-based-methane-sensing-for-greenhouse-gas-mitigation.pdf" class="pub-link" target="_blank" rel="noopener">Paper</a>
        </div>
    </div>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Creating accurate methane emission inventories through data-driven airborne survey strategies: methods and results from the Anadarko and Haynesville basins, USA
        </div>
        <div class="pub-authors">
            Yakovlev, P.V., Sherwin, E.D., <strong>Burdeau, P.</strong>, Brandt, A.R., Kruguer, J., Berman, E.S.F., Kamdar, H.
        </div>
        <div class="pub-venue">
            AGU Fall Meeting Abstracts, A13N-01 (2024)
        </div>
    </div>
    
    <div class="publication" data-author-type="coauthor" data-project="technology-evaluation">
        <div class="pub-title">
            Independent evaluation of methane sensing satellites, airplanes, and continuous monitoring ground sensors
        </div>
        <div class="pub-authors">
            El Abbadi, S., Chen, Z., <strong>Burdeau, P.</strong>, Rutherford, J., Chen, Y., Sherwin, E., Zhang, Z., Brandt, A.
        </div>
        <div class="pub-venue">
            AGU Fall Meeting Abstracts (2023)
        </div>
        <div class="pub-links">
            <a href="https://ui.adsabs.harvard.edu/abs/2023AGUFM.A53E..01E/abstract" class="pub-link" target="_blank" rel="noopener">Abstract</a>
        </div>
    </div>
</div>

<div class="pub-section" id="bu-model">
    <h2>Bottom-Up Emissions Model</h2>
    
    <div class="publication" data-author-type="first" data-project="bu-model">
        <div class="pub-title">
            Carbon emissions assessment: towards accurate control
        </div>
        <div class="pub-authors">
            <strong>Burdeau, P.</strong>, Debarre, R., Gahlot, P., Grillet, C.
        </div>
        <div class="pub-venue">
            Kearney Energy Transition Institute Report (2022)
        </div>
        <div class="pub-links">
            <a href="https://www.energy-transition-institute.com/factbooks/carbon-emissions-assessment" class="pub-link" target="_blank" rel="noopener">Report</a>
        </div>
    </div>
</div>

<script>
function filterPublications(type, button) {
    const publications = document.querySelectorAll('.publication');
    const sections = document.querySelectorAll('.pub-section');
    const buttons = document.querySelectorAll('.filter-btn');
    
    // Update button styles
    buttons.forEach(btn => btn.classList.remove('active'));
    button.classList.add('active');
    
    // Filter publications
    if (type === 'all') {
        publications.forEach(pub => pub.classList.remove('hidden'));
        sections.forEach(section => section.style.display = 'block');
    } else if (type === 'first') {
        publications.forEach(pub => {
            if (pub.getAttribute('data-author-type') === 'first') {
                pub.classList.remove('hidden');
            } else {
                pub.classList.add('hidden');
            }
        });
        sections.forEach(section => {
            const visiblePubs = section.querySelectorAll('.publication:not(.hidden)');
            section.style.display = visiblePubs.length > 0 ? 'block' : 'none';
        });
    } else {
        publications.forEach(pub => {
            if (pub.getAttribute('data-project') === type) {
                pub.classList.remove('hidden');
            } else {
                pub.classList.add('hidden');
            }
        });
        sections.forEach(section => {
            const visiblePubs = section.querySelectorAll('.publication:not(.hidden)');
            section.style.display = visiblePubs.length > 0 ? 'block' : 'none';
        });
    }
}
</script>
