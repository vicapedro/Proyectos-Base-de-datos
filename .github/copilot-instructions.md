# Database Projects - AI Agent Instructions

## Project Overview
This is an educational repository containing **database design case studies** for Systems Engineering courses. Each directory represents a complete business domain with real-world requirements written in domain-specific language rather than typical textbook database jargon.

## Architecture & Organization

### Project Structure
- **Each directory = One complete business case** (e.g., `Conquistadores/`, `TrumpetWare/`, `Salud y Vida/`)
- **Main specification file**: `{ProjectName}.md` contains the full business requirements
- **Query files**: `Consultas.md` contains SQL queries organized by difficulty (Básico/Intermedio/Avanzado)
- **Supporting files**: `README.md`, `Requisitos.md`, and domain-specific documents

### Documentation Patterns
- **Business domain language**: Requirements are written from stakeholder perspective, not technical database terms
- **Real-world scenarios**: Examples include specific names, locations, and business flows
- **Progressive complexity**: Queries advance from simple SELECT to complex CTEs and analytics

## Key Business Domains

### Conquistadores (Scout Club Management)
- **Core entities**: Clubs, Members, Classes, Specialties, Requirements
- **Complex relationships**: Multi-generational family tracking, skill progression, volunteer management
- **Business rules**: Age-based class progression, specialty prerequisites, investment ceremonies

### TrumpetWare (MLM/Catalog Sales)
- **Core entities**: Products, Ambassadors, Campaigns, Clients, Orders, CEDIS (Distribution Centers)
- **Complex workflows**: Multi-level sales structure, seasonal campaigns, inventory logistics
- **Business rules**: Ambassador level progression, regional distribution, production planning

### Salud y Vida (Healthcare Clinic)
- **Core entities**: Patients, Doctors, Appointments, Medical Records, Pharmacy, Lab Results
- **Integration points**: Electronic medical records, lab systems, pharmacy inventory
- **Compliance**: Medical data privacy, prescription controls, insurance processing

## Development Conventions

### Query Design Patterns
- **Básico**: Simple SELECT, WHERE, ORDER BY, basic GROUP BY
- **Intermedio**: JOINs, subqueries, except, intersect, union, window functions, aggregations with HAVING
- **Avanzado**: CTEs, recursive queries, pivot

### Naming Conventions
- Directory names use Spanish terms as domain language
- File names are descriptive: `Conquistadores.md` (main spec), `Consultas.md` (queries)
- Business entities use domain-specific terminology (e.g., "Conquistadores" not "members")

### Business Logic Complexity
- **Family relationships**: Multi-generational tracking in Conquistadores
- **Temporal data**: Historical tracking of roles, memberships, transactions
- **Geographic distribution**: Regional management in TrumpetWare, Agroquímicos
- **Regulatory compliance**: Medical records in Salud y Vida, chemical handling in Agroquímicos

## Build & Publishing

### Quarto Integration
- **Main config**: `_quarto.yml` defines book structure
- **Output formats**: HTML and PDF book generation
- **Chapter organization**: Each business case becomes a book chapter
- **Build command**: Standard Quarto book build process

### Content Management
- Markdown-based documentation with Spanish domain terminology
- Image assets stored within project directories
- Modular structure allows independent case study development

## Critical Development Workflows

### Adding New Business Cases
1. Create directory with descriptive Spanish name
2. Add main specification file: `{ProjectName}.md`
3. Include in `_quarto.yml` chapters list
4. Follow established query complexity progression in `Consultas.md`

### Query Development
- Start with business requirement in natural language
- Progress through complexity levels systematically
- Include real business scenarios and constraints
- Test queries against realistic data volumes

### Documentation Standards
- Write from stakeholder perspective first
- Include specific examples with names and scenarios
- Document business rules and edge cases
- Maintain consistency in domain terminology

## Integration Points

### Cross-Project Patterns
- **Inventory management**: Common across TrumpetWare, Agroquímicos, Salud y Vida
- **Geographic organization**: Regional structures in multiple domains
- **User role hierarchies**: Different permission levels across all projects
- **Temporal tracking**: Historical data requirements in most cases

### Common Database Challenges
- **Many-to-many relationships**: Specialties-Requirements, Products-Categories
- **Hierarchical data**: Organizational structures, product categorization
- **Audit trails**: Transaction history, status changes
- **Business rule enforcement**: Complex validation logic

This repository serves as a comprehensive database design learning platform with real-world complexity and domain-specific requirements that mirror actual business environments.
