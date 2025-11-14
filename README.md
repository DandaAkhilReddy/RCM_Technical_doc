# RCM Technical Documentation

Comprehensive Revenue Cycle Management (RCM) System Analysis & Implementation Guide for Page Management Associates.

## Overview

This documentation provides a complete technical analysis of the current RCM infrastructure, including system architecture, software inventory, integration methods, and strategic recommendations for 2025.

## Contents

### Main
- **Dashboard** ([index.html](index.html)) - Overview and key metrics
- **Executive Overview** ([overview.html](overview.html)) - High-level summary and stakeholder information

### Technical Documentation
- **System Architecture** ([architecture.html](architecture.html)) - Platform architecture and data flows
- **Software Inventory** ([inventory.html](inventory.html)) - Complete application inventory
- **Integration Methods** ([integrations.html](integrations.html)) - Detailed integration specifications
- **Data Flow Analysis** ([data-flow.html](data-flow.html)) - End-to-end data journey visualization

### Operations
- **Reconciliation Process** ([reconciliation.html](reconciliation.html)) - Payment posting and reconciliation workflows
- **Pain Points & Gaps** ([pain-points.html](pain-points.html)) - Critical operational issues and impact analysis
- **Data Governance** ([governance.html](governance.html)) - Policies, standards, and compliance

### Implementation
- **2025 Recommendations** ([recommendations.html](recommendations.html)) - Priority implementation recommendations
- **Implementation Roadmap** ([roadmap.html](roadmap.html)) - Quarterly 2025 implementation timeline
- **ROI Analysis** ([roi.html](roi.html)) - Detailed financial projections and cost-benefit analysis

## Key Findings

- **95% Manual Processes** - Current operations heavily dependent on manual work
- **24-Hour ADT Sync Delay** - Significant lag between clinical and billing systems
- **Zero Bank Integration** - No automated payment reconciliation
- **$2.5M Potential Recovery** - Estimated annual revenue recovery opportunity

## Technology Stack

- **Clinical**: Meditech (On-Premise)
- **Charge Capture**: IngeniousMed (Cloud SaaS)
- **Billing**: AdvancedMD (Cloud SaaS)
- **Clearinghouse**: McKesson RelayHealth
- **AR Management**: EnableComp (External Service)

## Critical Limitations

- AdvancedMD does NOT support HL7 integration
- No automated bank reconciliation
- Manual Excel-based tracking and reporting
- Limited real-time data synchronization

## 2025 Priority Recommendations

1. **Bank Integration & Payment Automation** - Deploy API or RPA for automated payment matching
2. **RPA for Insurance Follow-up** - Automate tracking and follow-up workflows
3. **HL7-Compatible System Migration** - Replace AdvancedMD for better integration
4. **AI-Powered Denial Management** - Predictive analytics and automated appeals

## Expected Impact

- **65%** reduction in manual work
- **$2.5M** annual revenue recovery
- **18 days** reduction in AR
- **90%** first-pass resolution rate

## Deployment

This is a static HTML website that can be:
- Hosted on GitHub Pages
- Deployed to Netlify
- Deployed to any web server
- Opened directly in a browser

### Live Deployments

**GitHub Pages**: https://dandaakhilreddy.github.io/RCM_Technical_doc/

**Netlify**: Coming soon (after initial deployment)

### Deploy to Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/DandaAkhilReddy/RCM_Technical_doc)

**Manual Deployment:**
1. Install Netlify CLI: `npm install -g netlify-cli`
2. Login: `netlify login`
3. Deploy: `netlify deploy --prod`

The `netlify.toml` configuration file is included with:
- Automated deployment settings
- Security headers
- Cache control optimization
- Lighthouse performance plugin

## Quality Assurance

This project uses automated testing and code review tools:

### CodeRabbit Integration
- AI-powered code reviews on every pull request
- Automated HTML validation and accessibility checks
- Configuration: `.coderabbit.yaml`

### GitHub Actions Workflows
- **HTML Validation**: Validates all HTML files using HTMLHint
- **Link Checker**: Verifies all internal navigation links are working
- **Accessibility Testing**: WCAG 2.0 AA compliance checks using Pa11y
- **Mobile Responsiveness**: Ensures proper viewport configuration

All tests run automatically on push and pull requests to ensure code quality.

## Development

### Running Locally
Simply open any HTML file in a modern web browser. All pages are standalone and don't require a build process.

### Contributing
1. Create a feature branch
2. Make your changes
3. Ensure all HTML files have proper navigation structure
4. Push and create a pull request
5. CodeRabbit will automatically review your code
6. GitHub Actions will run quality checks

## License

© 2025 Page Management Associates. All rights reserved.

---

**Last Updated**: January 2025
**Contact**: RCM Technical Team
**Version**: 1.0.0
