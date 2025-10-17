# Open Source Software Usage Guidelines

## Purpose

Simple guidelines for using open source software (OSS) in Avonova projects while ensuring legal compliance and security.

---

## License Risk Categories and Approval Requirements

### Category A: Permissive Licenses (Low Risk)

**Examples:** MIT, Apache 2.0, BSD-2-Clause, BSD-3-Clause, ISC

- **Approval Required:** None (auto-approved)
- **Documentation:** Must be recorded in dependency inventory
- **Usage:** Allowed for any purpose

### Category B: Weak Copyleft Licenses (Moderate Risk)

**Examples:** LGPL-2.1, LGPL-3.0, MPL-2.0, EPL-1.0, EPL-2.0

- **Approval Required:** Chapter lead approval
- **Documentation:** Detailed usage documentation required
- **Usage:** Allowed with proper compliance measures

### Category C: Strong Copyleft Licenses (High Risk)

**Examples:** GPL-2.0, GPL-3.0, AGPL-3.0

- **Approval Required:** Chapter lead + Legal Team approval
- **Documentation:** Comprehensive risk assessment required
- **Usage:** Generally prohibited unless exception granted

### Category D: Restricted Licenses (Very High Risk)

**Examples:** SSPL, Custom licenses with restrictions

- **Approval Required:** Executive approval
- **Documentation:** Full legal review required
- **Usage:** Prohibited unless special circumstances

---

## Quick Decision Guide

### ✅ Auto-Approved Licenses (Use freely)

**Category A** - Just document what you use

- **Examples:** Most npm packages, common Java libraries
- **Action:** Add to your project's dependency list

### ⚠️ Requires Approval (Ask Chapter Leader first)

**Category B/C** - Moderate risk licenses

- **Action:** Get Chapter Leader approval before using

### ❌ Generally Prohibited (Avoid unless special case)

**Category D** - High risk licenses that may require sharing source code

- **Action:** Only use with Chapter Leader + Legal approval

---

## Simple Process

### For Auto-Approved Licenses:

1. Use the OSS component
2. Keep it updated for security

### For Approval-Required Licenses:

1. Ask Chapter Leader before using
2. Explain why you need it
3. Get written approval
4. Document the approval

---

## What You Must Do

### ✅ Always:

- Keep OSS components updated (use GitHub Dependabot)
- Document what OSS you use in your project
- Report security vulnerabilities immediately
- Follow license terms (attribution, notices)

### ❌ Never:

- Use GPL/AGPL without approval
- Ignore security updates
- Remove license notices from OSS code
- Use OSS without documenting it

---

## Documentation Requirements

For each OSS component, document:

- **Name and version** (e.g., "express 4.18.2")
- **License type** (e.g., "MIT")
- **Why you're using it** (e.g., "HTTP server framework")
- **Approval** (if required)

---

## Security & Updates

- Use GitHub Dependabot (already enabled)
- Apply security patches within 30 days
- Test updates before deploying
- Have rollback plan for critical components

---

## Tools We Use

- **GitHub Dependabot** - Automatic vulnerability scanning
- **Maven/NPM/NuGet** - Dependency management
- **Parent POMs** - Centralized dependency control

---

## Quick Checklist

Before using new OSS:

- [ ] Check the license type
- [ ] Is it auto-approved? → Use it
- [ ] Needs approval? → Ask Chapter Leader
- [ ] Document what you use
- [ ] Keep it updated

