# ChangeLog

## [1.5.1] - 2025-05-07

### Fixed

- Fixed issues in GetReservationResponseDTO to ensure correct reservation data handling and serialization (042a2818).
- Fixed UpdateReservationByWaiterService by adding reservation status checks to prevent incorrect updates (6d8d1125).

### Notes

- This release focuses on bug fixes from development snapshots.
- No new features or breaking changes were introduced.
- Merged branches (develop, feature/20734, main) to incorporate fixes (8204ee50, 891530b1, 5e01fdd1).

## [1.5.0] - 2025-05-07

### Added

- Implemented global CORS configuration to support cross-origin requests (099ae7b4, ee57f7c2).
- Configured the pom.xml to have required dependencies for Spring Boot 3 (4e779a25).
- Changed

- Migrated the codebase from AWS Java (Dagger) to Spring Boot 3, adopting a modern framework for improved maintainability and performance.
- Upgraded to Java 17 to meet Spring Boot 3 requirements.

- Refactored internal architecture to leverage Spring Boot conventions, including dependency injection and configuration management, while preserving backward-compatible API behavior.
- Updated project dependencies to align with Spring Boot 3 (e.g., Spring Framework 6, Jakarta EE).

- Revised application.properties to support Spring Boot configuration requirements (196ea461).
- Updated deployment.yaml by removing extra spaces for cleaner configuration (6edebd19).
- Updated ingress configuration to optimize AWS deployment (80d4b864).

### Fixed

- Resolved multiple bugs introduced during the Spring Boot 3 migration, including:
- Fixed dependency injection issues transitioning from Dagger to Spring’s dependency management.

- Corrected configuration errors in application properties to ensure proper environment setup.
- Addressed runtime exceptions and compatibility issues from Java 17 and Jakarta EE updates.

- Stabilized API responses to match pre-migration behavior.
- Fixed a bug in ProfileService to ensure proper functionality (449c361e).
- Fixed issues in develop branch post-migration, stabilizing the codebase (baffc13a).

### Notes

- No new features were added in this release.
- The migration and changes introduce no breaking changes to the public API or external integrations.
- Incorporated changes from development snapshots into this stable release.

### Previous Releases

## [1.4.0] - 2025-04-23

- Final AWS project release before migration to Spring Boot 3.