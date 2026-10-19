# SIM Object Listing

## Entity objects (data)

| Object | Attributes | Operations | Relationships |
| --- | --- | --- | --- |
| User | user_id, full_name, email, phone, role, password_hash, status | register(), login(), logout(), changeRole() | 1 User to many Report; 1 User to many AuditLog |
| Report | report_id, reference_id, category, incident_datetime, latitude, longitude, location_text, description, is_anonymous, reporter_id, status, urgency, created_at | submit(), validate(), setStatus(), setUrgency(), markSpam() | 1 Report to many Evidence; 1 Report to many StatusHistory |
| Evidence | evidence_id, report_id, file_path, file_type, size_bytes | store(), stripMetadata() | Belongs to one Report |
| StatusHistory | history_id, report_id, old_status, new_status, changed_by, note, changed_at | record() | Belongs to one Report |
| AuditLog | log_id, actor_id, action, target, timestamp | write() | Belongs to one User |
| Category | category_id, name, is_active | list(), toggleActive() | Classifies many Report |

## Control and service objects (logic)

| Object | Attributes | Operations | Relationships |
| --- | --- | --- | --- |
| ReportService | rateLimitPerHour = 5 | validateReport(), generateReferenceId(), saveReport() | Uses Report, Evidence, NotificationService |
| AuthService | none | register(), login(), hashPassword(), checkRole() | Uses User |
| TriageService | none | verify(), markDuplicate(), markSpam(), setUrgency() | Uses Report, AuditLog |
| TrackingService | none | findByReference(), getHistory() | Uses Report, StatusHistory |
| NotificationService | gateway settings | sendEmail(), sendSMS() | Used by TriageService and ReportService |
| StatisticsService | none | countByCategory(period), exportCSV() | Uses Report, Category |

## Boundary and interface objects (screens)

| Object | Attributes | Operations | Relationships |
| --- | --- | --- | --- |
| ReportForm | category, role, date, time, location, description, anonymous, contact, consent | fillIn(), attachFiles(), submit() | Calls ReportService |
| TrackingPage | referenceId | lookup() | Calls TrackingService |
| CrimeMapView | period filter, markers | render(), filter() | Calls StatisticsService and Report data |
| OfficerDashboard | report queue, filters | openReport(), triage(), updateStatus() | Calls TriageService, StatisticsService |
| AdminPanel | user list, roles | createUser(), deactivate(), assignRole() | Calls AuthService |
