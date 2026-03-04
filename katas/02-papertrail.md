# Kata 2: PaperTrail

**A compliance document management system for regulated industries.**

A mid-size consultancy serving pharmaceutical and financial clients needs a system to manage compliance documents. Documents go through complex approval workflows (sometimes 12+ steps), must maintain a tamper-proof audit trail, and need to support simultaneous editing by multiple reviewers with different permission levels.

**Users:** 500 internal consultants, 2,000 client users across 30 organisations. Peak usage: end of fiscal quarters.

## Requirements

- Configurable approval workflows (each client has different rules)
- Tamper-proof audit log (legally admissible)
- Role-based access control with client-level isolation
- Full-text search across all documents with permission-aware results
- Version comparison (diff) between any two versions of a document
- Offline access for consultants travelling to client sites

## Constraints

- Must comply with FDA 21 CFR Part 11 (electronic signatures) and SOX
- Documents must never leave the EU (data residency)
- Integration with existing Active Directory for client organisations
- Some clients still use Internet Explorer 11 (yes, really)

## Additional context

The current system is a SharePoint instance that everyone hates. Migration must be incremental — no big bang.

[Back to all katas](../README.md#the-katas)
