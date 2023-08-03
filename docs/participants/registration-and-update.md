# Registration & Update

Each athlete must be registered and licensed before they are eligible to compete in IBSA competitions. From this menu, users are able to complete all
steps in the registration part of the process, as well as search for and update already registered athletes. Data access is restricted by NF and sport
affiliation in order to provide more relevant data for the users and to protect personal data of the athletes.

## Details

Users must navigate the **Athlete Registration** search screen before they can modify any participant details. By clicking on a row in the grid or on
the *Add Athlete* button, users reach the details tab with fields described in the following table. Certain fields are mandatory to fill out on
creation or update of an athlete.

| **Field**                                                                                           | **Format**                                               | **Searchable** | **Comments**                                                                                                                                                                                   |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span class="table-header">Basic Information</span>                                                 |                                                          |                |                                                                                                                                                                                                |
| **Athlete ID**                                                                                      | number                                                   | Yes            | automatically assigned on participant creation                                                                                                                                                 |
| **Career Status**                                                                                   | *Active*, *Historical* or *Retired*                      | Yes            | always set to active on creation, must be changed at *Career Status* tab                                                                                                                       |
| <span class="table-header">Personal Data</span>                                                     |                                                          |                |                                                                                                                                                                                                |
| **Member Federation**                                                                               | drop down [member]                                       | Yes            | obligatory, loaded from member basic table; the drop-down is limited to the list of IBSA (see [Application Settings](application-settings/regional-data.md#international-federations))         |
| **no Family Name**                                                                                  | checkbox                                                 | No             | in some cultures, only the given name is used in the passport. This box may be ticked to allow entries of such athletes; if not ticked, then both family and given names are obligatory fields |
| **Family Name (passport)**                                                                          | text (30)                                                | Yes            | family name exactly as written in the passport (except for non-English characters).                                                                                                            |
| **Given Name (passport)**                                                                           | text (30)                                                | Yes            | given name exactly as written in the passport. This is culturally dependent, but usually the name that appears second in the passport                                                          |
| **Family name (preferred)**                                                                         | text (30)                                                | Yes            | the version of the family name that will be used in all ISAS output. May be left blank on entry, will then be identical to passport name                                                       |
| **Given name (preferred)**                                                                          | text (30)                                                | Yes            | as above but with given name                                                                                                                                                                   |
| **Gender**                                                                                          | radio buttons                                            | Yes            | obligatory                                                                                                                                                                                     |
| **Date of Birth**                                                                                   | date (yyyy-mm-dd)                                        | No             |                                                                                                                                                                                                |
| **Photo**                                                                                           | picture file                                             | No             | set by system or by the user under nationality validation, see [File Attachments](layout-and-functionalities/file-attachments.md)                                                              |
| <span class="table-header">Nationality Information</span>                                           |                                                          |                |                                                                                                                                                                                                |
| **Nationality**                                                                                     | drop down [country demonym]                              | Yes            |                                                                                                                                                                                                |
| **Nationality Status**                                                                              | read-only                                                |                |                                                                                                                                                                                                |
| **Validation Document**                                                                             | drop down [*Passport*, *ID Card* or *Birth Certificate*] | No             | type of referenced document                                                                                                                                                                    |
| **Date of Expiration**                                                                              | date (yyyy-mm-dd)                                        | No             | date this document stops being valid, as determined by the issuing authority. A checkbox may be ticked if the referenced document never expires                                                |
| **Passport/ID Card No**                                                                             | text (30)                                                | Yes            | ID number of the referenced document                                                                                                                                                           |
| **Copy of Passport/ID Card**                                                                        | PDF file                                                 | No             | to upload a scan of the referenced document from user’s hard drive or local network. Once uploaded, the document can be downloaded or replaced.                                                |
| **Previous Member Representation**                                                                  | drop down [NPCs]                                         | No             | only applicable for athletes who have previously competed for other NPCs                                                                                                                       |
| **Confirmation Document**                                                                           | PDF file                                                 | No             | uploaded by IBSA after a nationality issue has been reviewed and confirmed                                                                                                                     |
| <span class="table-header">Sport and Sport Class Registration</span><span class="asterisk">*</span> |                                                          |                |                                                                                                                                                                                                |
| **Sport Class**                                                                                     | drop down [class]                                        | No             | populated upon selection of a sport                                                                                                                                                            |
| <span class="table-header">Comments</span>                                                          |                                                          |                |                                                                                                                                                                                                |
| **Member Comments**                                                                                 | text                                                     | No             | further free text information that can be provided by the member federation                                                                                                                    |
| **IBSA Comments**                                                                                   | text                                                     | No             | further free text information that can be provided by the IF; the member federation can only read but not change its content.                                                                  |

<p class="footnote">
    <small><span class="asterisk">*</span>Only available and displayed at registration of a new athlete. Any further modification must be done at the **Sports & Classes** tab or through the classification section of ISAS.</small>
</p>

The *searchable* column indicates whether this field is offered as a criterion on the search form.
The *family name* and *given name* fields of the search form will match in either the passport or
preferred name fields, but only display the preferred name, which may sometimes lead to unexpected
search results.

> [!DANGER]
> <img src="_img/inline/button-delete.png" alt="Delete Button" class="inline-button">
>
> **Caution:** The **‘delete’** button is accessible from the participant detail menu. An athlete may be completely deleted from the system once the
> user confirms a security question. **On deletion, all related classification data and files are irrevocably removed from the system.**
> In case, you want to remove just a duplicate, it is highly recommended to use the merging tool in the duplicate control section,
> see [Duplicate Control](participants/duplicate-control.md). If the athlete is not active in this sport any more, the status shall be changed
> to **‘Retired’**.

### How To: Register a new Athlete

<img src="_img/inline/button-add-athlete.png" alt="New Athlete/Guide Button" class="center inline-button">

1. Obtain a blank athlete detail form (see Figure 4.1) by clicking the **Add Athlete** button (from the search form) or the **New** button (from the
   details page).
2. Referring to the athlete details table, complete all fields to the best of your knowledge. Yellow fields are mandatory. Cross-check spelling and
   information with the uploaded documents. For example, the spelling of the passport name should be identical to that of the uploaded ID document, as
   far as the English alphabet allows.
3. Select the sport of the athlete or guide in from the drop down box Sport. For athletes, then enter the classification in the drop down box
   _1st Class_, and possibly further classifications.
4. Click **Save** to create an Athlete ID for the athlete. Note that the athlete or guide status of the participant can no longer be changed.
5. Upload a photo of the participant by clicking Choose File… and choosing a file from your local hard drive or network. The requirements for photos
   are described in [File Uploads](layout-and-functionalities/file-uploads).
6. Obtain a valid copy of the IBSA Eligibility Agreement Form with a signature from the athlete and/or, if the athlete is younger than 18 years old,
   their parent or legal guardian. Scan this document, save it as a PDF file, and upload the PDF file under the IBSA Eligibility Agreement field, in
   the **Eligibility Information** section of the athlete's profile.
7. If all documents have been uploaded correctly, IBSA will be notified and then review the registration for correctness. To view the result of this
   review, go to the [License Overview & Application](licence-management/licence-overview-and-application) screen. If there are documentation issues
   or other problems with the registration, IBSA notifies the NF by adding comments to the licence status; if everything is correct, the athlete will
   appear In the License Overview screen with status _New_.

<figure>
    <img src="_img/figures/4.1-athlete-registration-create.png" alt="A blank athlete registration form including file upload information" class="screenshot" >
    <figcaption>Figure 4.1 - A blank athlete registration form including file upload information</figcaption>
</figure>

After an athlete has been registered, there may be reason to change the details, for example because of errors or omissions in the data entry process,
name changes due to change in marital status, etc.

### How To: Change Athlete Details

1. Search for the athlete in question from the **Athlete Registration** search form and click the
   row
   in the search grid corresponding to the athlete to enter the athlete details’ page.
2. The data stored about the athlete will appear in the form. Edit the incorrect or missing details
   and click **Save**.
3. If you change passport name and/or the member federation of the athlete, a dialogue box (see
   Figure 4.2) appears
   to ask you to confirm the reason for the name change. Choose one of the three supplied reasons (
   error, marriage or nationality change)
   and, if applicable, enter the date from which the change should be effective.
4. If you change the name of the athlete, please bear in mind that changes only apply to the field you enter, i.e., a change of passport name will not
   change the preferred name, which is how the athlete will be named in publications. Hence, in case of a name change, please change both fields
   unless there is a specific reason not to; e.g. the athlete wishes to be known under the old name but the passport issuing body will only recognise
   the new name.

<figure>
    <img src="_img/figures/4.2-name-change-dialogue-box.png" alt="Name change dialogue box" class="inline-screenshot center" >
    <figcaption>Figure 4.2 - Name change dialogue box</figcaption>
</figure>

## Sports & Classes

This section is designed for non-classifier users who wish to have a quick overview of the classes the athlete is eligible for, as well as entering
and removing the class of athletes which have not yet been classified by international panels (**New** class status). More detailed manipulation is
possible from the [Classification](participants/classification) section.

All current classifications, with sport and class, of the athlete are displayed on this menu, along with the status of the athlete within the class.
The last row of the table allows for entering of a new sport and/or class; again, this will only be accepted if the athlete is not already classified
by international panels. If the registering user does not know which class the athlete will compete in, they may enter the pseudo-class N/A and leave
further classification to other users with competence in that field, alternatively enter the sport class B3 which accepts athletes with highest
visual function.

For any further classification specific issues, please refer to IBSA rules for that sport.

<figure>
    <img src="_img/figures/4.3-summary-of-athletes-classes.png" alt="Summary of athlete's classes" class="inline-screenshot center" >
    <figcaption>Figure 4.3 - Summary of athlete's classes</figcaption>
</figure>

## Career & Name Changes

The content of this tab is separated into three parts.

The upper part allows the user changing the career status of the athlete. To change the
status, enter a reason for the career status change, select the new status and **Save**. Retired
and historic athletes can be or are automatically excluded from search grids and reports.
Historic athletes can be excluded from user’s view by removing the operation *find historic
athletes*
from the user’s roles (see [Role Functions](account-manager/management-of-groups-roles-and-permissions.md#role-functions)).

The second part reflects all the career status changes including the provided reason and
timestamps.

The lower part reflects the changes of the athlete’s name and NF association. Each
(passport) name change is registered in the database to ensure that the identification of the
individual for an athlete ID never changes. The table here only shows the changes due to
marriage (M) or nationality (N) changes, but all error (E) related changes are still registered in
the backend and can be requested by the IPC SDMS administrator.

> [!WARNING]
> If an athlete is set to the career status Historical, they will disappear to all NF users from all outputs (such as classification data and
> licensing data).

## Biography

This tab is designed for adding, modifying and removing data about the athlete’s life to date.
This is particularly designed for media and fan interaction with the athletes, allowing them to
get to know the athletes’ personality beyond a statement of their results.

The biography tab is designed to be easily modifiable in case fields need to be added or removed
and should hopefully be self-explanatory. Fields are labelled in the left-hand column and a more
detailed explanation, if necessary, is given in the right-hand column.

## Data Sheet

Core information about an athlete is summarised in the data sheet report, including personal
information, the photo, registration statuses and the classification history.
This sheet appears as PDF inside the tab. If your browser does not support the PDF plugin,
you can click the link to generate and download the PDF to your local storage.

| Section                 | Included                                                                                                                                                                | User Guide Description                                                                                                                   |
|-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| **Personal Data**       | Photo, passport name, preferred name, gender, date of birth, NF, nationality, passport/id card number with expiry date.                                                 | [Registration & Update](participants/registration-and-update) (specifically, [Details](participants/registration-and-update?id=details)) |
| **Registration Status** | All fields relevant to a complete registration: Nationality status, eligibility status, career status and photo status.                                                 | [Registration & Update](participants/registration-and-update) (specifically, [Details](participants/registration-and-update?id=details)) |
| **Registered Sports**   | All sports where the athlete is registered, along with their historic and current classifications, with class, status and date. Current classifications are in **bold** | [Classification](participants/classification)                                                                                            |
| **Licenses**            | All historic and current licenses tabulated. Columns: Season, Sport code, License number, Invoice or Package, Status, Validity date                                     | [License Management](licence-management/licence-application-process)                                                                     |
