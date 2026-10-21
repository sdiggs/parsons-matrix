# The Parsons Matrix

**Live site: [https://sdiggs.github.io/parsons-matrix/](https://sdiggs.github.io/parsons-matrix/)**

The Parsons Matrix maps who works where in research data stewardship. It places each organization on three axes: whose data it handles, what it does with that data, and who uses the result. The original figure was a static 3D grid that came out of network mapping work; this site plots real organizations inside it so you can see the shape each one occupies, who pays for it, and where the space is empty.

## What's on the page

- A rotatable 3D cube with a show/hide button for each organization. Isolating one organization at a time is the clearest way to read its shape.
- A "color by" switch between organization and funder type (federal, philanthropy, host institution, volunteers and small grants, unfunded).
- The three axes, with notes on how each was revised from the original figure.
- A definition of home and reach, and how the cube draws them.
- A placement table with each organization's domains, functions, users, and funding.
- Findings so far, and open questions for reviewers.

## The axes

Each axis answers one question.

- **Domain (whose data?):** Earth system, Life, Physical (outside the Earth system), Social, Health.
- **Function (what does it do?):** Produce, Preserve, Standardize, Integrate, Deliver, Coordinate, Advocate, Train.
- **Users (who is it for?):** Researchers, CBOs, Policy and decision makers, Investors, Risk analysts, Journalists.

Funders are not a user group. They pay for the work rather than use the data, so funding colors the cube instead of occupying an axis.

## Home and reach

Home is what an organization exists to serve, as named in its charter, mission, or funder's terms. Reach is what its infrastructure touches without being designed for it. The test: if the organization stopped serving it tomorrow, would its funder or board say it was failing at its job? Filled dots mark home domains; hollow rings mark reach.

## Organizations plotted

NYCE's Data Stewardship Initiative (DSI), KCF's Planetary Vital Signs Initiative (PVSI), the Data Foundation's Center for Climate and Environmental Data (CCED), the Coalition for Resilient Research Data Infrastructure (CRRDI), the AGU Data Resilience Project, the Data Rescue Project, CODAN, NIH's Generalist Repository Ecosystem Initiative (GREI), the Environmental Data and Governance Initiative (EDGI), Public Environmental Data Partners (PEDP), and the Open Environmental Data Project (OEDP).

## Status

The axis revisions and placements are a first pass by Steve Diggs, drawn from each organization's public materials and his working knowledge of the field, and they're open for review. Funding entries for EDGI, PEDP, and OEDP are marked "to confirm" on the page. Dot size is reserved for funding tier once there's a figure for every organization.

## How it's built

The site is a single static `index.html` with no build step. It loads Plotly.js 2.27.0 from cdnjs and its typefaces from Google Fonts. All placements live in one JavaScript array (`O`) near the bottom of the file, so adding an organization means adding one entry with its domains, functions, users, and funding. The page follows the viewer's light or dark setting.

GitHub Pages serves the site from `index.html` at the root of the `parsons-matrix` repository.

## Sources

- [Data Foundation](https://datafoundation.org)
- [AGU Global Data Resilience Convening](https://news.agu.org/press-release/agu-global-data-resilience-convening/)
- [Data Rescue Project](https://www.datarescueproject.org/)
- [NIH GREI](https://datascience.nih.gov/data-ecosystem/generalist-repository-ecosystem-initiative)
- [EDGI](https://envirodatagov.org/about)
- [Public Environmental Data Partners](https://www.screening-tools.com)
- [Open Environmental Data Project](https://openenvironmentaldataproject.substack.com/)

Last updated October 21, 2026.
