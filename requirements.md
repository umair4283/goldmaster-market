# NovaFX Functional Requirements (SRS)

## 1. Public Website
- Home
- Markets
- Account types
- Trading platforms
- IB/Partner program
- FAQ
- Contact
- Risk Disclosure
- Terms & Conditions
- Privacy Policy
- AML/KYC Policy

## 2. Registration
Fields:
- Full name
- Email
- Phone
- Country
- Password
- Referral/IB code
- Terms acceptance

Referral attribution must be stored server-side and must not be editable after attribution without authorized admin workflow.

## 3. KYC
- Identity document upload
- Proof of address
- Verification status: Pending / Approved / Rejected
- Admin review
- Audit trail

## 4. Client Portal
- Profile
- KYC
- Trading accounts
- Balance/equity/margin
- Deposit requests
- Withdrawal requests
- Transaction history
- Referral link
- IB commissions
- Support tickets
- Notifications

## 5. MT5
Production version must use an authorized MT5 integration. Never fabricate live balances or trades.
Required data model:
- login/account ID
- server
- account type
- currency
- balance
- equity
- margin
- free margin
- open positions
- closed trades

## 6. Funding
Deposit:
- amount
- method
- proof/reference
- status
- timestamps

Withdrawal:
- amount
- destination
- KYC/eligibility checks
- admin approval
- processing status
- audit record

## 7. IB System
- Unique IB code
- Referral URL
- Referred clients
- Trading volume
- Commission rules
- Commission ledger
- Payout status
- Optional multi-level hierarchy, only where legally/contractually appropriate

## 8. Admin
- Client search
- KYC review
- Account management
- Deposit/withdrawal review
- IB management
- Commission rules
- Support tickets
- Audit logs
- System settings

## 9. Security
- HTTPS
- Password hashing
- MFA
- Rate limiting
- CSRF protection
- Input validation
- Secure file upload
- Role-based access
- Audit logs
- Encrypted sensitive data
- Backup and recovery

## 10. Compliance
Before accepting real client funds, obtain jurisdiction-specific legal/compliance advice and verify required authorization/licensing, KYC/AML obligations, privacy requirements, and payment rules.
