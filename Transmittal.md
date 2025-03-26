# Transmittal Tool Manual

## Introduction

The Transmittal (TRN) tool is developed to track and manage document transmissions to clients within the Enersea EPDM environment. It helps ensure proper documentation control, revision tracking, and structured export of related project documents. The transmittal function is used to create, revise, and send grouped documents with associated metadata. For a gif see [Go to Transmittal Tool](#how-to-use-the-transmittal-tool-with-gif-demo)

---

## File references transmittal

When viewing a transmittal in SOLIDWORKS PDM, the "Contains" tab shows which files are referenced by the transmittal file. These references represent links between documents—for example, a transmittal Excel file may reference a drawing or report that is included in the submission package. In the "Contains" tab, you can see all files directly linked to the selected transmittal file. Only the **top-level references**—the files directly attached to the transmittal—will be included when exporting or sending the transmittal. These are marked with a **green check mark**(see picture below)

If a referenced file has its own references (a second layer), those nested files are **not** included in the transmittal. This is visually indicated by a **red cross**(see picture below). In other words, the transmittal includes only the files it directly "contains" and skips any files deeper in the reference tree.
![ContainsTab](/Resources/Containstab.png)

## Interface Overview

The transmittal form is divided into two main sections:

- **Left panel**: General transmittal information input and controls.
- **Right panel**: Transmittal content display and file management.

See picture below:

![TemplateTRNForm](/Resources/TRNForm.png)

---

## 1. **Project Number Selector / Search TRN**

- **Purpose**: Automatically filled with the current project number.
- **Function**: You can search other transmittals for different projects by clicking the **Search TRN** button.

---

## 2. **Select Transmittal (Dropdown)**

- **Purpose**: Choose an existing transmittal.
- **Function**:
- Selecting a released transmittal triggers a **warning dialog**. - If confirmed, it **revises the transmittal** and allows new changes to be made.  
  ⚠️ Revising the transmittal will delete all existing references of the files.

---

## 3. **NEW TRANSMITTAL Button**

![TemplateTRNForm](/Resources/TemplateTRNForm.png)

- **Purpose**: Create a **new transmittal**.
- **Function**:
  - Opens the **TemplateTrn** window (see screenshot below).
  - In this form, you can define all relevant transmittal metadata including:
    - Project info (project number, name, company, client number, client revision).
    - Document info (code, name, revision, status, creation date, flag).
    - Review & approval roles (author, checker, approver).
    - Transmittal subject and keywords.
    - MDR and deliverable options.

#### Special Fields in the TemplateTrn Window

- **(1) Template Dropdown**  
  Select the type of transmittal template you wish to use:

  - **Enersea**
  - **H2Sea**
  - **FrequenSea**

- **(2) Export Folder (Browse...)**  
  By default, the export folder is the same directory where the files were selected.  
  Use the **Browse** button to select a different location if needed.  
  This is helpful when organizing exports by client or delivery batch.

  ❗ The folder needs to be inside the pdm vault.

ℹ️ Once all information is filled out, click **OK** to proceed with the new transmittal creation.

---

## 4. **Use Client Data for Attached Files (Checkbox)**

- **Purpose**: Choose between **Enersea document numbers** or **Client numbers** for export.
- **Function**:
  - When checked, `Document Code` and `Revision` will be set to the **client values** instead of Enersea values.

---

## 5. **Delete**

- **Click to highlight rows** (documents) to select them.
- **Delete Selected Files**:
  - Removes the selected (highlighted) files from the transmittal list.

---

## 6. **\*Add Selected Items**

- Adds the selected files from another control/menu (not shown in screenshot) to the current transmittal.
- See gif for more details.

## How to Use the Transmittal Tool (with GIF Demo)

![Ii7QSIoePA](https://github.com/user-attachments/assets/017b2619-ff0e-4ae2-96a6-222ac1ca9802)

---
