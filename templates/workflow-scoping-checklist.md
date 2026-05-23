# Workflow Scoping Checklist

Use this before writing a feature list.

## 1. Trigger

- What starts the workflow?
- Is the trigger manual, scheduled, customer-driven, or system-driven?
- What information is known at the beginning?

## 2. Actor

- Who performs the first action?
- Who reviews the result?
- Who only needs read access?
- Are there roles that can be merged in version one?

## 3. Data

- What fields are required?
- Which fields are optional?
- Which fields are calculated?
- Which fields should be locked after approval?

## 4. State

- What statuses are needed?
- Which transitions are allowed?
- Which transitions are forbidden?
- Does every change need an audit log?

## 5. Decision

- Who can approve, reject, cancel, or request revision?
- What note or reason is required?
- What happens after approval?

## 6. Output

- What should the owner, admin, customer, or field team see?
- Is a dashboard needed now or later?
- Is an export actually needed in version one?

## 7. Not Now

List what should not be built in the first release.

- 
- 
- 
