# Awesome-Demand-Side-Platform

# Top Demand-Side Platform (DSP) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Programmatic Advertising, Real-Time Bidding & Audience Targeting*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Demand-Side Platforms (DSP)**. These tools help advertisers and agencies automate the buying of digital ad inventory across display, video, mobile, and connected TV through real-time bidding (RTB).

**Examples** include The Trade Desk, Google DV360, Amazon DSP, Adform, StackAdapt, Basis Technologies, Simpli.fi, Viant Technology, Yahoo DSP, and Smadex (the category leaders).

**Open-source emphasis**: The open-source DSP ecosystem is **fragmented and largely historical**. Most active projects date from the early-to-mid 2010s when RTB was emerging. **RTB4FREE** and **vanilla-rtb** remain the most significant reference implementations, providing OpenRTB-compliant bidders and DSP frameworks . **Prebid Server** (Go/Java) is actively maintained and widely deployed, but it serves the **supply-side (header bidding)** rather than the demand side . **OpenAdServer** is a newer Python-based ad serving platform with ML-powered CTR prediction, though its RTB support is on the roadmap rather than production-ready . This section documents these focused solutions honestly.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[The Trade Desk](https://www.thetradedesk.com/)**
  The leading independent demand-side platform. Provides omnichannel programmatic buying across display, video, CTV, audio, and native. Known for transparency, data partnerships, and the Kokai AI platform.

- **[Google DV360](https://displayvideo.google.com/)**
  Google's enterprise DSP integrated with the Google Marketing Platform. Provides programmatic buying across YouTube, Google Display Network, and third-party exchanges with deep audience and measurement integration.

- **[Amazon DSP](https://advertising.amazon.com/)**
  Amazon's demand-side platform with unique access to Amazon's retail and streaming TV inventory. Provides audience targeting based on shopping behavior and Fire TV/IMDb TV inventory.

- **[Adform](https://adform.com/)**
  Integrated advertising platform with DSP, DMP, and ad server capabilities. Strong in European markets with omnichannel programmatic buying.

- **[StackAdapt](https://www.stackadapt.com/)**
  Multi-channel programmatic advertising platform. Provides DSP capabilities across native, display, video, CTV, audio, and DOOH with strong self-serve capabilities.

- **[Basis Technologies](https://basis.com/)**
  Programmatic advertising platform with DSP, workflow automation, and business intelligence. Serves agencies and brands with omnichannel buying.

- **[Simpli.fi](https://simplifi/)**
  Programmatic advertising platform specializing in addressable geo-fencing and unstructured data optimization. Strong in local and regional advertising.

- **[Viant Technology](https://www.viantinc.com/)**
  People-based DSP with household ID graph for omnichannel programmatic buying. Provides CTV, display, audio, and native inventory.

- **[Yahoo DSP](https://www.yahooinc.com/)**
  Yahoo's demand-side platform (formerly Verizon Media DSP). Provides programmatic buying with Yahoo's identity graph and premium inventory.

- **[Smadex](https://smadex.com/)**
  Mobile-first DSP specializing in programmatic user acquisition and retargeting for mobile apps and games.

## Open-Source GitHub Projects

### DSP Frameworks & Bidders

- **[RTB4FREE](https://github.com/RTB4FREE/rtb4free)**  
  **The most complete open-source DSP framework.** Provides an OpenRTB 2.0 compliant bidder with campaign management UI . The **bidder** repo has 87 stars and 55 forks, written in Java . Includes **campaign-manager** (26 stars) for campaign management and **rtb4free** core repo for documentation and API explorer . **Status**: Last updated approximately 2 years ago; historical reference implementation .

- **[vanilla-rtb](https://github.com/venediktov/vanilla-rtb)**  
  **Real Time Bidding (RTB) Demand Side Platform framework written in C++.** 328 stars, 87 forks . Provides a high-performance bidder framework. **rapid-bidder** (71 stars) is a DSP application built on the vanilla-rtb stack, last updated approximately 7-8 years ago . **Status**: Historical reference; not actively maintained .

- **[OpenAdServer](https://github.com/pysean/openadserver)**  
  **Self-hosted ad serving platform with ML-powered CTR prediction.** Provides a complete pipeline: **Retrieve → Filter → Predict → Rank → Return** . **Key features**: OpenRTB compatible (roadmap); **DeepFM CTR model** with AUC 0.72; PostgreSQL + Redis; Docker Compose deployment; Prometheus metrics; Grafana dashboards . **Tech stack**: Python 3.11+, FastAPI, PyTorch. **Status**: Active development; RTB support planned .

- **[OpenDSP (javagossip)](https://github.com/javagossip/opendsp)**  
  **Open-source mobile DSP advertising platform with built-in ADX integration and out-of-the-box dashboard.** 133 stars, updated April 2025 . Chinese-language project providing a complete mobile DSP solution.

- **[RTBKit](https://github.com/rtbkit/rtbkit)**  
  **Open-source software package for creating and deploying Real Time Bidders for display advertising.** 1,068 stars . **Status**: Last updated approximately 6 years ago; historical.

### Supply-Side & Infrastructure (Adjacent)

- **[Prebid Server](https://github.com/prebid/prebid-server)**  
  **Open-source solution for server-to-server header bidding.** Go implementation with 574 stars, Apache-2.0 licensed . **Note**: This is **supply-side** (publisher) technology, not demand-side, but is the most actively maintained open-source ad tech project . Java version also available . **Prebid.js** (1,589 stars) handles client-side header bidding .

- **[OpenRTB](https://github.com/openrtb/OpenRTB)**  
  **Documentation and issue tracking for the OpenRTB Project.** 859 stars . The **OpenRTB specification** (405+ stars) defines the protocol for real-time bidding on digital media .

- **[OpenRTB Models (Go)](https://github.com/mxmCherry/openrtb)**  
  **OpenRTB protocol definitions for Go.** 288 stars, updated 2 months ago . Actively maintained library for Go-based RTB implementations.

- **[OpenRTB Models (Java)](https://github.com/openrtb/openrtb2x)**  
  **OpenRTB model for Java via protobuf with JSON serialization helpers.** 397 stars .

- **[Revive Adserver](https://github.com/revive-adserver/revive-adserver)**  
  **The most popular free open-source ad server.** Provides ad serving, targeting, and reporting. **Note**: Ad server, not a DSP; serves as the ad delivery infrastructure .

### Additional Strong Open-Source Options

- **DSP Frameworks**: **RTB4FREE** (Java, OpenRTB 2.0, historical) , **vanilla-rtb** (C++, high-performance, historical) , **OpenAdServer** (Python, ML-powered, active) .
- **Mobile DSP**: **OpenDSP** (Java, ADX integration, 2025) .
- **Infrastructure**: **Prebid Server** (Go/Java, supply-side, active) , **OpenRTB Models** (Go/Java, protocol definitions) .
- **Ad Serving**: **Revive Adserver** (ad server, not DSP) .

**Frameworks for building custom systems**: Combine **OpenAdServer** for ML-powered ad serving with CTR prediction, **RTB4FREE** or **vanilla-rtb** for reference DSP architecture, **OpenRTB Models** (Go or Java) for protocol definitions, and **Revive Adserver** for ad delivery infrastructure. Add **PostgreSQL** for data persistence, **Redis** for caching, and **Docker** for deployment.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DSP platforms handle sensitive advertising and audience data; ensure compliance with GDPR, CCPA, and applicable advertising regulations.
- **Open-source reality**: The open-source ecosystem for demand-side platforms is **fragmented and largely historical**. Most DSP frameworks (**RTB4FREE**, **vanilla-rtb**, **RTBKit**) date from the early-to-mid 2010s and are no longer actively maintained . **Prebid Server** is the most actively maintained open-source ad tech project but serves the **supply side** (header bidding), not the demand side . **OpenAdServer** represents a newer generation of ML-powered ad serving, but its RTB support is planned rather than production-ready . **Commercial platforms** (The Trade Desk, DV360, Amazon DSP) provide **global inventory access, identity graphs, brand safety controls, and managed optimization** that open-source alternatives cannot match. The open-source path is most viable for **research, education, or building specialized internal ad tech infrastructure** rather than competing with commercial DSPs.

---

**Made for ad tech engineers, programmatic advertisers, and RTB researchers.**
Let's make demand-side platforms more open, transparent, and accessible.
