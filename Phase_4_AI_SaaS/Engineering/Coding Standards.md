# Coding Standards.md

# Coding Standards

**Version:** 1.0 **Status:** Founding Engineering Standard **Parent
Documents:** Tech Stack.md, Architecture.md, AI Strategy.md

------------------------------------------------------------------------

# Purpose

This document defines the coding standards that every engineer and AI
coding assistant must follow. The goal is to produce software that is
readable, secure, testable, maintainable, and scalable.

------------------------------------------------------------------------

# Coding Philosophy

Code is a long-term business asset.

Write code for the next developer---not just for the compiler.

Prioritize: - Readability - Simplicity - Consistency - Reliability -
Maintainability

------------------------------------------------------------------------

# Clean Code Principles

-   One responsibility per function.
-   Small, focused modules.
-   Avoid duplication (DRY).
-   Keep logic simple (KISS).
-   Build only what is needed (YAGNI).

------------------------------------------------------------------------

# SOLID Principles

Apply SOLID where appropriate:

-   Single Responsibility
-   Open/Closed
-   Liskov Substitution
-   Interface Segregation
-   Dependency Inversion

------------------------------------------------------------------------

# Naming Conventions

Use meaningful names.

Variables: - Descriptive nouns.

Functions: - Clear verbs.

Classes: - Business concepts.

Files: - Feature-oriented and consistent.

Avoid abbreviations unless universally understood.

------------------------------------------------------------------------

# Project Structure

Organize code by feature before technical layer whenever practical.

Keep UI, business logic, and infrastructure separate.

------------------------------------------------------------------------

# Error Handling

-   Fail gracefully.
-   Never ignore exceptions.
-   Return actionable error messages.
-   Log errors with context.
-   Never expose sensitive information.

------------------------------------------------------------------------

# Logging Standards

Log:

-   Errors
-   Warnings
-   Important business events

Do not log:

-   Passwords
-   Secrets
-   Personal sensitive data

------------------------------------------------------------------------

# Security Standards

Always:

-   Validate inputs.
-   Sanitize outputs.
-   Use parameterized queries.
-   Apply least privilege.
-   Protect secrets.
-   Keep dependencies updated.

Security is everyone's responsibility.

------------------------------------------------------------------------

# Performance Guidelines

Optimize after measuring.

Avoid:

-   Premature optimization
-   N+1 database queries
-   Unnecessary re-renders
-   Blocking operations

------------------------------------------------------------------------

# Testing Standards

Every feature should include:

-   Unit tests
-   Integration tests (when applicable)
-   End-to-end tests for critical workflows

Tests should be deterministic and maintainable.

------------------------------------------------------------------------

# Documentation

Document:

-   Public APIs
-   Complex business logic
-   Architectural decisions
-   Setup instructions

Avoid comments that repeat the code.

------------------------------------------------------------------------

# Git Standards

-   Small commits
-   Descriptive commit messages
-   Feature branches
-   Pull Requests for review
-   Keep main branch deployable

------------------------------------------------------------------------

# Code Review Checklist

☐ Readable

☐ Tested

☐ Secure

☐ Performant

☐ Documented

☐ Follows architecture

☐ No unnecessary complexity

☐ Business goal achieved

------------------------------------------------------------------------

# AI-Assisted Development

AI may assist with:

-   Boilerplate
-   Refactoring
-   Documentation
-   Test generation

Every AI-generated change must be reviewed by a developer before
merging.

------------------------------------------------------------------------

# Definition of Done

A task is complete only when:

☐ Code implemented

☐ Tests pass

☐ Documentation updated

☐ Accessibility maintained

☐ Security reviewed

☐ Performance acceptable

☐ Code reviewed

☐ Ready for deployment

------------------------------------------------------------------------

# Common Mistakes

-   Large functions
-   Duplicate logic
-   Hardcoded values
-   Ignoring tests
-   Poor naming
-   Mixing UI and business logic
-   Skipping code reviews

------------------------------------------------------------------------

# Final Principle

Quality is not created during code review.

Quality is created every time we write, review, and improve code.
