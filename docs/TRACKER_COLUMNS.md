# Finance Master Tracker columns

Create an Excel table (Insert → Table) with these headers. `Request ID` is the key the flow uses to update a row.

## Written when the request is submitted

| Column | Source |
| --- | --- |
| Request ID | `PAY-yyyyMMdd-HHmmss-XXXX` (generated) |
| Month, Year, Date of Request, Time of Request | Submission time in IST |
| Current Status | `Pending Level 1 Approval` |
| Department, Requested By, Requester Email | Form |
| Vendor Type, Vendor Name | Form |
| PAN Number, GST Number | Form |
| Amount Without GST, GST Amount, Total Amount | Form |
| Payment Reason, Expected Payment Date | Form |
| Account Holder Name, Account Number, IFSC Code | Form |
| Invoice Link, PAN Link | Link of the first uploaded file |
| Cancelled Cheque Link | Form |
| Level 1 Approval, Level 2 Approval, Payment Status | `Pending` |

## Written by the approval steps

| Column | Written at |
| --- | --- |
| Level 1 Approval, Level 1 Approval Date, Level 1 Remarks | Level 1 decision |
| Level 2 Approval, Level 2 Approval Date, Level 2 Remarks, Level 2 Approval Raw | Level 2 decision |
| Payment Status, Finance Remarks | Payment step (UTR or ETA and reason) |
| Current Status, Last Updated At | Every step |

Bank and PAN details are sensitive. Keep the workbook in a restricted finance folder.
