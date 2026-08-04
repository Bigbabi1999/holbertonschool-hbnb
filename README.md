# HBnB Technical Documentation

## Introduction

This document describes the architecture and design of the HBnB application. It contains a high-level package diagram, a detailed class diagram, and sequence diagrams that illustrate how the application's components interact. These diagrams serve as a blueprint for implementing the project.

## High-Level Architecture

The application follows a three-layer architecture:

- Presentation Layer: Handles API requests and user interactions.
- Business Logic Layer: Contains the application's core business logic and entities.
- Persistence Layer: Manages data storage and retrieval.

The Presentation Layer communicates with the Business Logic Layer through a Facade, which simplifies interactions between components.

## Business Logic Layer

The Business Logic Layer contains the following entities:

- User
- Place
- Review
- Amenity

Each class defines its own attributes and methods.

Relationships:

- A User can own multiple Places.
- A User can write multiple Reviews.
- A Place can have multiple Reviews.
- A Place can have multiple Amenities.

## API Interaction Flow

The sequence diagrams demonstrate how different API requests move through the system.

The following API calls are included:

1. User Registration
2. Place Creation
3. Review Submission
4. Fetch List of Places

Each request follows the same flow:

User
→ API
→ Business Logic
→ Database
→ Business Logic
→ API
→ User

## Explanatory Notes

### High-Level Package Diagram

This diagram provides an overview of the application's layered architecture.

### Detailed Class Diagram

This diagram defines the main entities, their attributes, methods, and relationships.

### Sequence Diagrams

These diagrams illustrate how requests travel through the system during different API operations.

Together, these diagrams provide a complete overview of the HBnB application's structure and behavior.
