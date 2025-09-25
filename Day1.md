# 📅 Day 1 – Kickoff & Account Guardrails

## 🎓 Study (≈35 minutes)

### Exam Prep Overview: SAA-C03 (20m)
- Introduces exam structure, domains, and scoring.  
- **4 Domains**:
  1. Secure Architectures (30%)
  2. Resilient Architectures (26%)
  3. High-Performing Architectures (24%)
  4. Cost-Optimized Architectures (20%)

### Exam Prep Plan Overview: SAA-C03 (15m)
- Explains AWS’s recommended prep process.  
- Aligns with the 6-week plan.  

👉 **Tip**: Use OneNote/Notion/Markdown for notes - this becomes your interview prep portfolio.

---

## 🔐 Hands-On Lab: Guardrails & Safety Net (~60 minutes)

### Step 1 – Secure the Root Account
- Enable MFA for root user (Authenticator app).  
- Delete any root access keys.  

### Step 2 – Create an Admin Role
- Role: `AdminRole` with `AdministratorAccess`.  
- Use role instead of root going forward.  

### Step 3 – Create Admin User
- User: `you-admin` → Console sign-in enabled.  
- Group: `Admins` with AdministratorAccess.  
- Practice switching to `AdminRole`.  

### Step 4 – Budgets (Cost Tripwire)
- Create budget: **$10/month**.  
- Alerts at 80% & 100% via SNS email.  

### Step 5 – Logs Bucket
- S3 bucket: `org-logs-<yourname>-<region>`.  
- Enable:
  - Block Public Access  
  - Versioning  
  - Default Encryption (SSE-S3)  
- Add tags: `Project=Training`, `Owner=You`.  

### Step 6 – Tagging Standard
- Apply tags to all resources:
  - `Project=Training`
  - `Week=1`
  - `Owner=You`

---

## ✅ Deliverables
- Screenshot: MFA enabled on root.  
- Screenshot: Budget with alert configured.  
- Screenshot: S3 bucket with versioning + encryption enabled.  
- `README.md` with tagging standard.

---

## 🎯 End of Day 1 Outcomes
- ✅ Watched both AWS Exam Prep intros (35m).  
- ✅ MFA + budgets protecting account.  
- ✅ Secure logs bucket ready for CloudTrail.  
- ✅ Admin user/role workflow (no root usage).  
- ✅ Personal tagging standard documented.
