# Approval State Machine

Use this to define approval workflow logic before implementation.

## States

- draft
- submitted
- under_review
- revision_requested
- approved
- rejected
- cancelled
- processed

## Transitions

| Current state | Action | Next state | Actor | Note required? |
|---|---|---|---|---|
| draft | submit | submitted | requester | no |
| submitted | approve | approved | reviewer | optional |
| submitted | reject | rejected | reviewer | yes |
| submitted | request revision | revision_requested | reviewer | yes |
| revision_requested | resubmit | submitted | requester | no |
| approved | process | processed | admin | optional |

## Audit log

Store at least:

- actor
- previous state
- next state
- timestamp
- note or reason
