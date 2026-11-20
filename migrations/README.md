# Database migrations

Use Alembic for schema changes. Keep tenant-scoped foreign keys, uniqueness constraints, and row-level security with the tables they protect. Separate table ownership and migration privileges from runtime roles. Test the effective privileges with each actual identity.

P01 adds the first executable migration and its configuration. Later tickets own migrations for their records. Coordinate concurrent changes to the Alembic revision chain.
