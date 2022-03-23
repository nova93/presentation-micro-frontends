# Backend for Frontend (BFF)

<br />
<br />

A BFF (Backend for Frontend) acts as a simple interface between the frontend and the micro-services that make up the Business Logic Mesh (BLM).

A BFF should generally avoid adding functionality or service to the application. Actual business logic should be in micro-services of the BLM, particularly if this logic is shared.

Each BFF is focused on a single User Experience, this helps us keep our front end User Experience as simple as possible and prevents the increasing complexity that arises when a single back end service tries to cater for the needs of many types of clients with different business needs.

<!-- ./components/SelfPromo.vue -->
<SelfPromo />
