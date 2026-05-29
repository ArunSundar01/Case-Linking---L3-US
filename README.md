# Case-Linking---L3-US

This repository contains the L3 user stories for Case Linking.

## L2 User Stories (Reference)

### L2-US-01: Identify related cases
**As a** case handling user  
**I want to** identify cases that are related to each other  
**So that** I can avoid duplicate work and improve resolution quality.

### L2-US-02: Establish case relationships
**As a** case handling user  
**I want to** create and manage links between related cases  
**So that** dependencies and relationships are clearly tracked.

### L2-US-03: View linked case context
**As a** case handling user  
**I want to** view all linked cases and their statuses from a case record  
**So that** I can quickly understand the full case context.

### L2-US-04: Maintain link quality
**As a** case handling user  
**I want the system to** prevent invalid or duplicate links  
**So that** case relationships remain accurate over time.

### L2-US-05: Control and audit link changes
**As a** case handling user  
**I want to** restrict link updates to authorized roles and track changes  
**So that** case-linking actions are secure and auditable.

## L3 User Stories

### US-01: Search and identify related cases
**As a** case manager  
**I want to** search for existing cases using case ID, customer details, and keywords  
**So that** I can identify cases that may need to be linked.

**Acceptance Criteria**
- The user can search by case ID, customer name, email, phone number, and keyword.
- Search results show key case details such as case ID, title, status, priority, and owner.
- The user can open a case from the results to review its details before linking.

### US-02: View case context before linking
**As a** case manager  
**I want to** review the summary and current state of two cases before linking them  
**So that** I can confirm that the relationship is valid.

**Acceptance Criteria**
- The user can view case summaries, status, category, and recent activity for each selected case.
- The user can compare the selected cases side by side before confirming the link.
- The system highlights if the selected cases are already linked.

### US-03: Link two or more related cases
**As a** case manager  
**I want to** link related cases and define the relationship type  
**So that** all connected work items can be managed together.

**Acceptance Criteria**
- The user can select one primary case and link one or more related cases to it.
- The user can choose a relationship type such as duplicate, parent-child, or related.
- The system saves the link and updates all linked cases with the relationship details.

### US-04: Prevent invalid or duplicate case links
**As a** case manager  
**I want the system to** prevent duplicate or invalid links  
**So that** case relationships remain accurate and trustworthy.

**Acceptance Criteria**
- The system blocks attempts to create the same link more than once.
- The system prevents a case from being linked to itself.
- The system shows a clear validation message when the requested link is not allowed.

### US-05: View linked cases from the case record
**As a** case manager  
**I want to** see all linked cases from a case record  
**So that** I can quickly understand the relationship history and navigate between them.

**Acceptance Criteria**
- A linked cases section is visible on the case details page.
- The section lists each linked case with its relationship type and current status.
- The user can navigate directly to any linked case from the list.

### US-06: Remove a case link with traceability
**As a** case manager  
**I want to** unlink cases when the relationship is no longer valid  
**So that** case data stays correct while preserving an audit trail.

**Acceptance Criteria**
- The user can remove an existing link between cases.
- The system requires a reason before the unlink action is completed.
- The system records who removed the link and when it was removed.

### US-07: Restrict linking actions by role
**As a** system administrator  
**I want to** control which roles can create or remove case links  
**So that** only authorized users can manage case relationships.

**Acceptance Criteria**
- Only users with the required permission can create or remove links.
- Unauthorized users can still view linked cases if they have case access.
- The system shows an access error when a user without permission attempts to modify links.
