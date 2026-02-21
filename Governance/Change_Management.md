# Change Management Policy: Nexus Health AI

## 1. Purpose
To ensure that all changes to the Nexus-Core AI environment are performed in a controlled manner to maintain **99.9% Service Availability** and data integrity.

## 2. Change Categories
* **Standard:** Routine, low-risk changes (e.g., UI text updates).
* **Normal:** Non-emergency changes requiring full review (e.g., AI model updates).
* **Emergency:** Critical fixes for system outages (requires retroactive review).

## 3. The "Safety Net" Process
All "Normal" changes must follow the **R.R.T.R.** workflow:
1. **Request:** Document the change in the ticketing system.
2. **Review:** A senior engineer (not the author) must perform a **Peer Review** of the code.
3. **Test:** Changes must be verified in the 'Staging' sandbox environment.
4. **Rollback:** Every change must have a pre-defined "Undo" plan if the system fails.

## 4. Approval Authority
No code shall be deployed to the production environment without a signed approval from the **Change Advisory Board (CAB)** or the designated Security Lead.
