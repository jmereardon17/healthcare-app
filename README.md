# Healthcare App

A healthcare platform that streamlines patient registration, appointment scheduling, and medical records. A built in admin dashboard that securely uses a passkey for authentication, admins can manage day to day appointments by re-scheduling or cancelling.

Built with: JavaScript, TypeScript, React, Next.JS 14, Appwrite, Tailwind CSS

[Demo](https://healthcare-app-wheat.vercel.app)

## Setup

create an `.env.local` file in the root directory using the example `.env.example` template for the variables the app uses. Setup a project within Appwrite then copy the relevant data to the corresponding environment variable.

For the database setup within Appwrite, create a database containing two collections:

| appointment                                                    | patient                                         |
| -------------------------------------------------------------- | ----------------------------------------------- |
| `patient` Many to one Relationship with `patient` from patient | `email` (Email) - Required                      |
| `schedule` (Datetime) - Required                               | `phone` (String) - Required                     |
| `reason` (String) - Required                                   | `userId` (String) - Required                    |
| `note` (String)                                                | `name` (String) - Required                      |
| `primaryPhysician` (String) - Required                         | `privacyConsent` (Boolean) - Required           |
| `status` (Enum) - Required                                     | `gender` (Enum)                                 |
| `userId` (String) - Required                                   | `birthDate` (String)                            |
| `cancellationReason` (String)                                  | `address` (String)                              |
|                                                                | `occupation` (String)                           |
|                                                                | `emergencyContactName` (String)                 |
|                                                                | `emergencyContactNumber` (String)               |
|                                                                | `insuranceProvider` (String)                    |
|                                                                | `insurancePolicyNumber` (String)                |
|                                                                | `allergies` (String)                            |
|                                                                | `currentMedication` (String)                    |
|                                                                | `familyMedicalHistory` (String)                 |
|                                                                | `pastMedicalHistory` (String)                   |
|                                                                | `identificationType` (String)                   |
|                                                                | `identificationNumber` (String)                 |
|                                                                | `identificationDocumentId` (String)             |
|                                                                | `identificationDocumentUrl` (String) - Required |
|                                                                | `primaryPhysician` (String)                     |
|                                                                | `treatmentConsent` (Boolean)                    |
|                                                                | `disclosureConsent` (Boolean)                   |
