# Prototype---project
graph TD
    A[Beneficiary] --> B[Submits Aadhaar & Account Details to Bank];
    B --> C[Beneficiary Signs Consent Form for DBT];
    C --> D[Bank Seeds Account Details into Core Banking System (CBS)];
    D --> E[Bank Updates NPCI's Aadhaar Mapper with Beneficiary's Aadhaar & Account Info];
    E --> F[Government Scheme Ministry Sends Payment Request with Aadhaar Numbers to PFMS];
    F --> G[PFMS Sends Payment Instruction to NPCI (via APB)];
    G --> H[NPCI Routes Payment Using Aadhaar Mapper to Correct Bank];
    H --> I[Bank Credits DBT Payment to Beneficiary's Account];
    I --> J[Beneficiary Receives SMS Confirmation of Credit];