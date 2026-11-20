# Vessel image registry migration

Base: container-libs image/v5.42.1, commit b84f98e (upstream tag).

Registry error and API types migrate from Distribution v2 to v3 in production
and tests. Authentication, credentials, transport, TLS and image handling stay
upstream implementations. Docker/reference, credential configuration, registry
configuration and TLS suites pass under race detection with the portable
containers_image_openpgp build tag.

The Vessel backend graph carries the complete, explicitly pinned fork set.
Local absolute module replacements are validation-only and must not be shipped.
