# SAFIA ERP: Shaistakhil Trading Company

> **Client project** · Built by [Rahimi Tech Solution](https://github.com/AbdulRahmanRahimi) · The source code is private to the client.

A complete business management ERP for **Shaistakhil Trading Company (SAFIA brand)**, a buyer, processor and exporter of Afghan saffron and dry fruits. It runs the whole chain, from buying from farmers to exporting to customers abroad, with double-entry accounting in **AFN, USD and INR**.

## What it does

- **Buying**: farmer registration, purchases in Man or KG, cash and instalment plans, receipts and vouchers (A4 and 80 mm) with QR codes
- **Stock and processing**: stock by warehouse and batch, transfers between branches, approved adjustments, processing orders with quality control, yield, waste and cost per KG; every batch can be traced back to its farmers
- **Selling and export**: customers with credit limits, sales invoices from stock batches, export shipments with commercial invoice, packing list and certificate of origin
- **Money**: cash and bank accounts per branch and currency, expenses with approval and bill photos, currency exchange with gain/loss, bank reconciliation
- **Reports**: profit and loss, balance sheet, cash flow, trial balance, general ledger, aged payables and receivables, stock valuation, with Excel export and print/PDF
- **Tools**: product labels with barcodes and QR codes, WhatsApp Business API notifications, audit trail, role permissions editor, two-step sign-in for administrators, an in-app user guide

## Engineering highlights

- All money, stock and accounting rules live **in the database**, so every screen and any future API follows the same rules
- Posted records are never edited or deleted; corrections are cancellations and reversing entries
- The 12 acceptance tests from the software requirements specification run automatically

## Tech stack

| Layer | Tools |
|---|---|
| Frontend | Next.js 16 (App Router), React 19, TypeScript, Tailwind CSS 4 |
| Backend | Supabase: PostgreSQL 17, Auth with two-step sign-in, Row Level Security, Storage |
| Other | ExcelJS, QR code and barcode generation, WhatsApp Business API |
| Hosting | Vercel |

---

Designed, built and deployed by **Abdul Rahman Rahimi**.
