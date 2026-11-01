# Royal Flight Club Department Billing
Release: credits-only billing and optional color printing (1 November 2026).
App Created By: Micha Christine Dotimas

Upload the exported ledger, enter department account number and month, review debit/credit totals, complete billing details and issue a numbered service bill. Current month only is the default; opening balance is displayed separately. Print in A4 portrait with browser headers/footers off.

The source export can be XLS/XLSX, CSV or tab-separated text named .xls. Required columns: VoucherNo, Date, VoucherType, Member, MemberNo, Debit, Credit, Balance. The upload is parsed by the bundled SheetJS Community Edition locally. No ledger data, customer records, PDFs or backups belong in this repository.

New bills request the selected month's total Credit only. Debit entries and payments remain visible for reconciliation but are not deducted from the payment request. Opening balances are excluded. Previously issued snapshots keep their original amounts and billing basis. Always review the bill before issuing. No tax is computed or added. Missing or conflicting source values are flagged rather than invented. Card numbers are not imported.

The browser keeps an invoice register in localStorage. Once issued, snapshots and bill numbers remain unchanged. Duplicate account/month issuance is blocked within that browser. New bill numbers use PREFIX-YEAR-SEQUENCE, for example RFC-2026-00001. Previously issued numbers remain unchanged; no central invoice-number registry exists. Use one designated billing computer and export backups. Restoring a backup copies its register and browser identifier; do not issue in parallel from cloned backups. Clearing browser data can lose the register. Private customer data is not uploaded by the application, but people with access to the same unlocked browser can read it.

Third-party reader: SheetJS CE 0.20.3, Apache-2.0, https://sheetjs.com/ . No external scripts, analytics or network submissions are used.

Print appearance defaults to black and white, with an optional Color setting for the original club logo and maroon headings. The choice is remembered on this browser. Select Color in the printer dialog too; background graphics may be enabled for shaded headings. Neither print option includes creator attribution. The creator credit remains visible in the app.
