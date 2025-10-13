# Partle - Local Product Discovery Platform

**May 2025 - Present**

## Overview

A community-driven web application designed to solve the frustration of searching for products across multiple local stores. Partle enables users to search for specific items and instantly see availability in nearby stores, saving time and eliminating the need to visit closed or out-of-stock locations.

The platform bridges the gap between online shopping convenience and local retail, offering immediate availability information and the ability to see products before purchase. Built as an alternative to existing e-commerce platforms that don't adequately serve local discovery needs.

## Key Features

- **Smart Product Search** - Find items by name or specification (e.g., "JST 6-pin", "M8 locking nut")
- **Location-Based Discovery** - View product availability in nearby stores with map and list views
- **Community-Driven** - Users and store owners can add products, with reliability ratings
- **Passkey Authentication** - Modern, passwordless sign-in using FIDO2 standard
- **Store Management** - Multi-user store control with official/unofficial product tagging
- **Map Integration** - Interactive OpenStreetMap view for visual store location
- **AI-Optimized** - Structured data for AI search engines and API discoverability

## Technical Details

### Full-Stack Architecture

**Frontend:**
- React 18 with TypeScript for type-safe development
- Vite for fast development and optimized production builds
- Tailwind CSS for utility-first styling
- Radix UI for accessible component primitives
- Leaflet (OpenStreetMap) for interactive mapping
- react-helmet-async for SEO and structured data

**Backend:**
- FastAPI (Python 3.12+) for high-performance API
- uv for modern Python dependency management
- PostgreSQL with SQLAlchemy ORM
- Alembic for database migrations
- Passkeys (FIDO2) for passwordless authentication
- Elasticsearch for scalable product search
- Image storage in PostgreSQL (BYTEA)

**Infrastructure:**
- Frontend hosted on Hetzner Cloud
- PostgreSQL database on Hetzner (production)
- Dual environment setup (development/production)
- MCP servers for Claude Desktop integration
- Docker Compose for Elasticsearch

### Advanced Features

**Search System:**
- Elasticsearch integration for millions of products
- Advanced filtering by location, price, availability
- Database fallback for reliability
- Natural language support (planned)

**Data Architecture:**
- Product-Store relationship model
- Official/unofficial product tagging system
- Community reliability ratings (similar to X's Community Notes)
- Tag system for product categorization
- Binary image storage with MIME type support

**AI Integration:**
- robots.txt for crawler control
- ai.txt for AI training permissions
- OpenAPI schema for programmatic API discovery
- Schema.org structured data for rich search results
- sitemap.xml for efficient indexing

## Highlights

!!! success "Problem Solving"
    Addresses a real frustration: searching 30 stores for a specific item, only to find most closed or out of stock. Partle reduces this to a single search with real-time availability.

!!! info "Community-First Design"
    Built on community collaboration with reliability ratings that discourage spam while encouraging authentic contributions from users and store owners.

!!! note "Modern Tech Stack"
    Leverages cutting-edge technologies: Passkeys for authentication, Elasticsearch for scale, TypeScript for type safety, and uv for fast Python tooling.

## Use Cases

- **Finding Specialty Items** - Locate hard-to-find hardware, electronics, or specialty products
- **Price Comparison** - Sort by price and distance to find best local deals
- **Store Discovery** - Find nearby stores you didn't know existed
- **Local Business** - Help stores gain visibility for their inventory

## Monetization Strategy

- Ads and premium product positioning (similar to Wallapop)
- Store database connections via API
- AI-powered natural language search
- Location-based product recommendations

## Resources

- [Live Application](https://partle.rubenayla.xyz/) - Production deployment
- [GitHub Repository](https://github.com/rubenayla/partle) - Source code and documentation
- [API Documentation](https://partle.rubenayla.xyz/docs) - Interactive API docs

## Technical Achievements

- Built full-stack application with modern authentication (Passkeys/FIDO2)
- Implemented scalable search with Elasticsearch fallback
- Created community-driven content moderation system
- Deployed production infrastructure on Hetzner Cloud
- Integrated AI discoverability features (OpenAPI, Schema.org)
- Developed responsive map-based UI with real-time data
