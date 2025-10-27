# F1R3FLY.io Improvement Proposals (FIP) Repository

## Project Context
- This is the **F1R3FLY.io Improvement Proposals (FIP) repository** for documenting and tracking proposed changes to F1R3FLY.io projects
- F1R3FLY.io specializes in **high throughput transaction servers** with a focus on distributed systems and blockchain technologies
- The organization maintains multiple projects including RNode, Rholang implementations, and hyper-dimensional computing research
- This repository follows industry-standard improvement proposal processes modeled after EIP (Ethereum Improvement Proposals) and BIP (Bitcoin Improvement Proposals)
- Follow F1R3FLY.io's **documentation-first development methodology** for all proposals
- If the user does not provide enough information with their prompts, ask the user to clarify before executing the task
- DO NOT use emoticons in documentation or synthesized code. Keep it to text, tables, and hierarchical structures. Prefer use of `.yaml` to document hierarchies

## Repository Architecture

### Technology Stack
- **GitHub** - Version control and collaboration platform
- **Markdown** - Proposal documentation format
- **Git** - Version control system
- **GitHub Pages** - Proposal hosting and navigation (when applicable)

### Content Structure
```
fflip/
├── FIPS/                     # F1R3FLY.io Improvement Proposals
│   ├── fip-1.md             # Meta: FIP Purpose and Guidelines
│   ├── fip-2.md             # Subsequent proposals
│   └── ...
├── templates/               # Proposal templates
│   ├── fip-template.md     # Standard FIP template
│   └── ...
├── assets/                  # Supporting materials
│   ├── fip-N/              # Assets for specific FIPs
│   └── ...
├── CLAUDE.md               # This file - AI assistant context
├── README.md               # Repository overview and index
└── LICENSE                 # Repository license
```

## F1R3FLY.io Organization Overview

### Core Focus Areas
- **High Throughput Transaction Servers** - Scalable distributed systems
- **Blockchain Infrastructure** - RNode platform with multi-consensus mechanisms
- **Rholang Programming Language** - Process calculus based concurrent programming
- **Hyper-Dimensional Computing** - rhoHDC encoding research
- **Developer Tools** - Language servers, parsers, and development environments

### Key Projects
1. **RNode** - Decentralized blockchain platform with four consensus mechanisms
2. **Rholang** - Concurrent programming language with formal verification
3. **rhoHDC** - Encoding of rho-calculus into hyper-dimensional computing
4. **Embers** - F1R3Sky wallets and agents
5. **Developer Tools** - Language servers, parsers, and Rust implementations

## FIP Standards and Process

### Proposal Lifecycle
All F1R3FLY.io Improvement Proposals must follow this process:
1. **Idea Discussion** - Vet concepts through community forums and channels
2. **Draft Proposal** - Create FIP using the standard template
3. **Community Review** - Gather feedback and iterate on the proposal
4. **Final Call** - Last opportunity for community input before acceptance
5. **Acceptance** - Proposal is accepted and marked as Final
6. **Implementation** - Execute based on approved FIP specification
7. **Deployment** - Changes are deployed to production systems

### FIP Categories
```
FIP Types:
├── Core              # Consensus-affecting changes to RNode, protocols
├── Networking        # Network protocol improvements
├── Interface         # Language-level standards (Rholang, APIs)
├── Application       # Application-level standards and conventions
├── Meta              # Process proposals and governance changes
└── Informational     # Guidelines and design documentation
```

### FIP Naming Conventions
- **Files**: `fip-[number].md` (e.g., fip-1.md, fip-42.md)
- **Numbers**: Sequential integers assigned by FIP editors
- **Assets**: `assets/fip-[number]/` for supporting files
- **Templates**: `fip-template.md` for standard proposal structure

## Development Environment

### Local Repository Setup
```bash
# Clone the repository
git clone https://github.com/F1R3FLY-io/fflip.git

# Navigate to FIP directory
cd fflip

# View FIP structure
tree FIPS/

# Create a new FIP from template
cp templates/fip-template.md FIPS/fip-[number].md

# Edit FIP with your preferred editor
code FIPS/fip-[number].md
```

### GitHub Integration
- **Version Control**: All FIPs tracked in Git with full history
- **Collaboration**: Pull requests for new FIPs and revisions
- **Discussion**: GitHub Issues and Discussions for FIP feedback
- **Templates**: Standard templates in `templates/` directory
- **Review Process**: FIP editors review and merge proposals

## FIP Content Management

### FIP Structure and Organization
All FIPs follow a standardized structure with required metadata and sections:

#### FIP Header (Preamble)
```yaml
---
fip: [number]
title: [Brief descriptive title]
author: [Name <email>]
discussions-to: [URL or issue number]
status: Draft | Review | Last Call | Final | Withdrawn | Superseded
type: Core | Networking | Interface | Application | Meta | Informational
category: [Only for Standards Track]
created: [YYYY-MM-DD]
requires: [FIP numbers if applicable]
replaces: [FIP numbers if applicable]
superseded-by: [FIP numbers if applicable]
---
```

#### Required FIP Sections
```
1. Simple Summary        # One-paragraph explanation
2. Abstract             # Technical summary (200 words max)
3. Motivation           # Why this FIP is necessary
4. Specification        # Detailed technical specification
5. Rationale            # Design decisions and alternatives considered
6. Backwards Compatibility  # Impact on existing systems
7. Test Cases           # Required for Core FIPs
8. Reference Implementation  # Code or proof-of-concept
9. Security Considerations  # Security analysis
10. Copyright          # License information
```

### FIP Status Definitions
- **Draft**: Initial FIP submission, open for changes
- **Review**: Ready for peer review and feedback
- **Last Call**: Final review period before acceptance
- **Final**: Accepted standard, implementation complete
- **Withdrawn**: Author has withdrawn the proposal
- **Superseded**: Replaced by another FIP

## Repository Sections

### FIP Directory
- **[FIPS/](FIPS/)** - All F1R3FLY.io Improvement Proposals
- Organized sequentially by FIP number
- Each FIP is a standalone markdown document
- Includes fip-1.md as the meta-proposal defining the FIP process

### Templates Directory
- **[templates/](templates/)** - FIP templates and examples
- **fip-template.md** - Standard template for new proposals
- Example FIPs demonstrating best practices
- Style guides and formatting standards

### Assets Directory
- **[assets/](assets/)** - Supporting materials for FIPs
- Organized by FIP number (e.g., assets/fip-42/)
- Contains diagrams, images, code samples, data files
- Referenced from FIP markdown using relative paths

## FIP Best Practices

### Markdown Standards for FIPs
- **Headers**: Use proper hierarchy (H1 for title, H2 for major sections)
- **Links**: Use descriptive link text and relative paths for assets
- **Code Blocks**: Specify language for syntax highlighting (Rholang, Scala, etc.)
- **Images**: Store in assets/fip-[number]/, include alt text, optimize file sizes
- **Tables**: Use for structured data presentation
- **Math**: Use LaTeX notation for mathematical expressions when needed
- **Citations**: Link to academic papers, RFCs, and other FIPs appropriately

### FIP Authoring Guidelines
- **Clarity**: Write for technical audience but ensure accessibility
- **Completeness**: Include all required sections with thorough detail
- **Precision**: Be specific about technical requirements and specifications
- **Examples**: Provide concrete examples and test cases
- **Impact Analysis**: Clearly document backwards compatibility and security implications
- **Reference Implementation**: Include working code when possible

### Version Control for FIPs
- **Commit Messages**: Use conventional commits format (feat: add FIP-42)
- **Branching**: Create feature branch for each new FIP
- **Reviews**: Require FIP editor review before merging
- **History**: Never modify merged FIPs except for status updates
- **Status Updates**: Update status field via separate commits with clear messages

## Common Tasks

### Creating a New FIP
1. **Vet the Idea**: Discuss in community forums and GitHub Discussions
2. **Draft the FIP**:
   - Copy `templates/fip-template.md` to `FIPS/fip-[number].md`
   - Get FIP number assignment from FIP editors
   - Fill in all required sections
   - Add preamble metadata
3. **Create Supporting Assets**:
   - Create `assets/fip-[number]/` directory if needed
   - Add diagrams, code samples, or other materials
4. **Submit for Review**:
   - Create feature branch (e.g., `fip/42-description`)
   - Commit FIP with clear message
   - Open pull request with FIP summary
   - Link to discussion threads
5. **Iterate**: Incorporate feedback and update status as appropriate

### Updating an Existing FIP
1. **Status Updates Only** (for merged FIPs):
   - Edit only the status field in preamble
   - Commit with message like "Update FIP-42 status to Final"
   - Create pull request for FIP editor review
2. **Draft FIPs** (not yet merged):
   - Make necessary changes to content
   - Update metadata if needed
   - Push to existing PR branch

### Adding FIP Assets
1. Create directory `assets/fip-[number]/` if it doesn't exist
2. Add files with descriptive names (e.g., `architecture-diagram.png`)
3. Reference from FIP using relative paths: `../assets/fip-42/diagram.png`
4. Optimize images for web (compress, reasonable dimensions)
5. Include all assets in the same PR as the FIP

### Managing FIP Templates
1. Update templates in `templates/` directory
2. Ensure backward compatibility with existing FIPs
3. Version control template changes
4. Announce template updates in community channels
5. Document template version in template file itself

## Testing and Validation

### FIP Review Checklist
- [ ] All required sections are present and complete
- [ ] Preamble metadata is correctly formatted
- [ ] FIP number is properly assigned and unique
- [ ] Links work correctly and point to valid resources
- [ ] Markdown renders properly on GitHub
- [ ] Code examples are accurate and tested
- [ ] Images display correctly with appropriate alt text
- [ ] Technical specifications are clear and implementable
- [ ] Backwards compatibility impact is documented
- [ ] Security considerations are addressed
- [ ] Reference implementation is provided (if applicable)
- [ ] Follows FIP style guidelines and conventions

### FIP Quality Standards
- **Technical Accuracy**: Specifications are precise and implementable
- **Clarity**: Written for technical audience with clear explanations
- **Completeness**: All required sections thoroughly documented
- **Consistency**: Follows established FIP patterns and conventions
- **Security**: Security implications thoroughly analyzed
- **Testing**: Test cases provided for verification
- **Implementation**: Reference code demonstrates feasibility

## Git Workflow

### Branching Strategy
- **main**: Production branch containing all accepted FIPs
- **fip/[number]-[short-description]**: Branch for each new FIP
- **status/[number]**: Branch for FIP status updates
- **template**: Branch for template updates

### Commit Guidelines
- Use conventional commits format:
  - `feat: add FIP-42 for new consensus mechanism`
  - `docs: update FIP-1 with editorial changes`
  - `status: update FIP-42 status to Final`
- Reference GitHub issues and discussions when applicable
- Keep commits focused and atomic (one FIP per commit typically)
- Never amend merged FIP content (only status updates)

### Pull Request Process
1. **New FIP**: Create PR from `fip/[number]-description` branch
2. **Title Format**: "FIP-[number]: [Brief Title]"
3. **Description**: Include motivation, summary, and discussion links
4. **Labels**: Apply appropriate labels (Draft, Core, Meta, etc.)
5. **Review**: Wait for FIP editor review and approval
6. **Merge**: Squash commits when merging to main

### File Management
- **DO NOT** commit sensitive data or credentials
- **DO NOT** commit large binary files (>1MB) without optimization
- **DO NOT** modify merged FIPs except status field
- **DO** use .gitignore for temporary and local files
- **DO** optimize images before committing (use PNG, WebP, or SVG)
- **DO** keep FIP assets in dedicated `assets/fip-[number]/` directories

## Security Considerations

### FIP Security Best Practices
- Never commit API keys, secrets, or credentials in FIPs or assets
- Review all FIP content for sensitive information before submission
- Every FIP must include a "Security Considerations" section
- Analyze potential attack vectors introduced by proposals
- Document threat models for Core and Networking FIPs
- Consider cryptographic implications for security-related changes
- Review third-party dependencies and libraries referenced

### FIP Security Review Process
- All Core and Networking FIPs require security review
- Security implications must be explicitly documented
- Threat modeling required for consensus-affecting changes
- Cryptographic proposals need expert review
- Coordinate with security team for high-risk FIPs
- Public security disclosures follow responsible disclosure practices

## Troubleshooting

### Common FIP Issues

#### FIP Number Conflicts
```bash
# Check existing FIP numbers
ls FIPS/ | grep -E 'fip-[0-9]+\.md' | sort -V

# Verify your FIP number is unique
grep -r "^fip: [number]" FIPS/
```

#### Markdown Rendering Issues
```bash
# Preview locally using your editor's markdown preview
# Test YAML frontmatter validity
grep -A 10 "^---" FIPS/fip-[number].md

# Validate on GitHub preview:
# - Push to branch and view on GitHub
# - Use online tools like markdownlivepreview.com
```

#### Asset and Link Issues
```bash
# Verify asset directory exists
ls -la assets/fip-[number]/

# Test relative paths from FIP to assets
# From FIPS/fip-42.md to assets/fip-42/diagram.png
# Use: ../assets/fip-42/diagram.png
```

#### Status Update Problems
- Only update the `status:` field in preamble for merged FIPs
- Create separate PR for status changes
- Never modify content of merged FIPs
- Coordinate with FIP editors for status transitions

## Resources

### F1R3FLY.io Links
- **Website**: [f1r3fly.io](https://f1r3fly.io)
- **GitHub Organization**: [github.com/F1R3FLY-io](https://github.com/F1R3FLY-io)
- **FIP Repository**: [github.com/F1R3FLY-io/fflip](https://github.com/F1R3FLY-io/fflip)
- **Contact**: f1r3fly.ceo@gmail.com

### Related Improvement Proposal Standards
- **EIP (Ethereum)**: [eips.ethereum.org](https://eips.ethereum.org)
- **BIP (Bitcoin)**: [github.com/bitcoin/bips](https://github.com/bitcoin/bips)
- **PEP (Python)**: [peps.python.org](https://peps.python.org)
- **RFC (IETF)**: [www.rfc-editor.org](https://www.rfc-editor.org)

### Documentation and Tools
- [GitHub Markdown Guide](https://docs.github.com/en/get-started/writing-on-github)
- [Git Documentation](https://git-scm.com/doc)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [YAML Specification](https://yaml.org/spec/)
- [Mermaid Diagrams](https://mermaid.js.org/) - For creating diagrams in markdown

## FIP Principles

### Core Values
- **Consensus-Driven**: Community input guides all decisions
- **Transparency**: Open discussion and public review process
- **Technical Excellence**: Rigorous technical standards and specifications
- **Security**: Thorough security analysis for all proposals
- **Innovation**: Advance F1R3FLY.io technologies and capabilities
- **Backwards Compatibility**: Minimize breaking changes where possible

### FIP Quality Standards
- **Technical Precision**: Clear, implementable specifications
- **Completeness**: All required sections thoroughly documented
- **Clarity**: Accessible to technical audience
- **Testability**: Concrete test cases and verification methods
- **Security**: Comprehensive security analysis
- **Implementation**: Reference code demonstrates feasibility

## FIP Editor Responsibilities
- **Number Assignment**: Assign unique FIP numbers sequentially
- **Format Review**: Ensure FIPs follow template and conventions
- **Technical Review**: Verify technical soundness (or delegate to experts)
- **Process Management**: Guide FIPs through status transitions
- **Merge Control**: Approve and merge FIP pull requests
- **Index Maintenance**: Keep README.md FIP index current

## Important Instructions
- Do what has been asked; nothing more, nothing less
- NEVER create files unless absolutely necessary
- ALWAYS prefer editing existing files
- NEVER proactively create FIPs or documentation files unless requested
- Follow F1R3FLY.io's documentation-first methodology for all FIPs
- Follow industry-standard FIP processes (modeled after EIP/BIP)
- Ensure all FIPs include required sections and metadata
- Ask for clarification when requirements are unclear
- Validate FIP structure and format before submission
