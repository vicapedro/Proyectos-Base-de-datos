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

### 🎯 Purpose
When generating exercises for student projects, Copilot should provide **creative and realistic SQL problems** aligned with the course progression. Exercises must involve real-world data scenarios and encourage step-by-step mastery of T-SQL and standard SQL features.



### 🪜 Difficulty Levels & Expected Features

| Level | Description | Common Clauses | Key Functions |
|-------|-------------|---------------|---------------|
| 🟢 **Básico** | Data cleaning, simple filters, basic transformations | `SELECT`, `FROM`, `WHERE`, `ORDER BY`, `DISTINCT`, `TOP` | `LEN`, `LTRIM`, `RTRIM`, `SUBSTRING`, `UPPER`, `LOWER`, `CAST`, `ISNULL` |
| 🟡 **Intermedio** | Summaries, simple joins, conditional logic | `GROUP BY`, `HAVING`, `UNION`, `EXCEPT`, `INTERSECT`, simple subqueries | `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`, `CASE`, `IIF`, `DATEDIFF`, `YEAR`, `MONTH` |
| 🔵 **Avanzado** | Analytical calculations, complex transformations, advanced joins | `JOIN` (various), `APPLY`, `PIVOT`, correlated subqueries | `STRING_AGG`, `FORMAT`, `DATEADD`, `EOMONTH`, `POWER`, `TRY_CAST` |
| 🔴 **Experto** | Analytical SQL, complex structures, optimization | `WITH` (CTE), window functions with `OVER`, `MERGE`, `OUTPUT` | `ROW_NUMBER`, `RANK`, `LAG`, `LEAD`, `JSON_VALUE`, `STRING_SPLIT` |

---

### ✍️ Exercise Generation Guidelines

When Copilot generates SQL exercises, it should:

1. **Start with a business or real-world scenario**  
   - Example: “Una empresa quiere saber qué productos se vendieron más el último trimestre.”  
   - Keep scenarios simple and relatable (e.g. ventas, hospital, biblioteca, escuela, transporte).

2. **Specify the expected difficulty level**  
   - Use the 🟢🟡🔵🔴 classification to guide the choice of clauses and functions.  
   - Build exercises progressively when generating a sequence.

3. **Vary the type of challenges**  
   - Data cleaning  
   - Filtering & sorting  
   - Aggregation & reporting  
   - Subqueries & set operations  
   - Joins between multiple tables  
   - CTEs and window functions

4. **Include constraints or twists**  
   - Example: “Solo mostrar clientes con más de 3 compras en el último año.”  
   - Or: “Obtener el producto más vendido por región sin usar subconsultas.”

5. **Target multi-database compatibility (when possible)**  
   - Stick to ANSI SQL for Básico & Intermedio levels.  
   - Avoid vendor-specific functions unless the exercise is explicitly Avanzado/Experto.

6. **Describe expected outputs or goals**  
   - Example: “La consulta debe devolver el nombre del cliente, el total gastado y el número de pedidos.”

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
