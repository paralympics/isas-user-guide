# Reports

When administrating large numbers of athlete data, it is often a good idea to print database
extracts as PDF or Excel files in a report. These reports can be generated as **Grid Export**
from each search table, but the specifically designed report section of ISAS combines data
from various tables for more comprehensive reporting.

The Report section is available to both IBSA and NF users. NF users can only download data
relating to their country’s own athletes.

## Classification Master List <!-- {docsify-ignore} -->

The _Classification Master List_ is the main report produced by ISAS, and the one with the most
customisable options. It can be used to prepare classification schedules for competitions, get
an overview of all athletes from a national federation, club, and/or sport. It can also be used
to review the registration and licence status, if this is necessary. For example, it may be
desirable to only include already licensed athletes when entering athletes for the schedule,
or if one would like an overview of all information an NF has entered about an athlete.

A classification report can only be produced for one sport at a time; therefore, the _Sport_
drop-down box is compulsory. The user must be aware that athletes with pseudo-class **‘N/A’**
are excluded from all reports.

The PDF reports generated in ISAS are generic across all sports. They only include the athlete
data and some basic information like class, class status, year of review, date of classification
and classification level (national/ international) for each athlete.

## Competition Search

It is possible to specify the competition/ classification event code for the search
([Competitions](calendar/competitions.md)). This produces a report for all athletes registered
to that event through the sport-specific assignment page
([Assigning Athletes and Classifiers](calendar/competitions.md#assigning-athletes-and-classifiers)),
particularly useful for the preparation of classification schedules. If the competition code is not
set, all athletes from the database are considered based on the other criteria.

## Other Options

A comprehensive table of all search options follows.

[//]: # (TODO: Fix this table)

| **Field**                                                                    | **Format**                                                  | **Comments**                                                                                                                                |
|------------------------------------------------------------------------------|-------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| <span class="table-header">Core Parameters</span>                            |                                                             |                                                                                                                                             |
| **Sport**                                                                    | drop-down [sport]                                           |                                                                                                                                             |
| **Region**                                                                   | drop-down [region]                                          | select by region (1 or all)                                                                                                                 |
| **National Federation**                                                      | drop-down [federation]                                      | select by responsible NF (1 or all)                                                                                                         |
| **License Status**                                                           | drop-down box                                               | <span class="asterisk">*</span>                                                                                                             |
| **active athletes only**                                                     | checkbox                                                    | If checked, only athletes with career status Active are included in the report                                                              |
| **load personal status**                                                     | checkbox                                                    | If checked, nationality status, career status and yes/no flag for an uploaded photo are included                                            |
| <span class="table-header">Competition Parameters</span>                     |                                                             |                                                                                                                                             |
| **Competition Module**                                                       | Calendar                                                    |                                                                                                                                             |
| **Competition Code**                                                         | text (6)                                                    | Enter the six-digit competition code from the calendar to limit the list of athletes to those assigned to this event in the selected sport. |
| <span class="table-header">Sorting</span>                                    |                                                             |                                                                                                                                             |
| **Sort Order**                                                               | by Athlete Name or Athlete ID                               |                                                                                                                                             |
| <span class="table-header">Additional Columns (only for Excel report)</span> |                                                             |                                                                                                                                             |
| **General Profile Fields**                                                   | checkboxes                                                  | <span class="asterisk">1</span>                                                                                                             |
| **Sport-Specific Profile Fields**                                            | checkboxes (automatically adjusted based on selected sport) | <span class="asterisk">2</span>                                                                                                             |
| **General Classification File Containers**                                   | checkboxes                                                  | <span class="asterisk">3</span>                                                                                                             |
| **Sport-Specific Classification File Containers**                            | checkboxes (automatically adjusted based on selected sport) | <span class="asterisk">4</span>                                                                                                             |

<p class="footnote" style="text-align: justify">
  <small>
  <span class="asterisk">*License Status</span><br>
The final compulsory field is the License Status drop-down box. This controls the license status of the included athletes. By default, the report 
only includes athletes who are (were, for past seasons) licensed for the selected season.To change this, there are five options:<br>
<b>Licensed:</b> shows only athletes with an active license for the selected season<br>
<b>Licensed & Pending:</b> also include athletes with Pending status (payment pending, only for winter sports)<br>
<b>Registered:</b> shows all athletes who do not have a cancelled license status, i.e., those whose registrations have been reviewed and approved in the License Renewal section<br>
<b>Registered & Cancelled:</b> shows all athletes in the license database for that particular season<br>
<b>Complete Database:</b> shows all athletes with an ISAS ID. Choose this option if you do not want to restrict the search to a particular season.<br>
  </small>
</p>

<span class="asterisk">1. / 2. </span>Lists all classification profile fields that are globally registered for all sports (

see [Classification Profile](participants/classification.md#classification-profile)). Each field checked includes a column with the classification

profile information currently stored for all athletes.

<span class="asterisk">3. / 4. </span>Lists all classification file containers that are globally registered for all sports (

see [Documentation](participants/classification.md#documentation)). Each field checked includes a column indicating whether and when a file for this

category has been uploaded.

## PDF Export

PDF reports are printed in landscape format, with a set number of columns varying from
sport to sport when you click the *Open as PDF* button. The report is also timestamped
and verified with the official logos of IBSA.

From the left, each row includes personal data – Athlete ID, family name, given name,
gender, date of birth – the athlete’s current class, the class status, and the year of
review. If the athlete has different classes for different events and/or disciplines,
this is also shown next to the class name.

The classification master list report tries to find any inconsistencies in the classification
of athletes, e.g. an athlete in a single-class sport like alpine skiing has two classes currently
registered. Such inconsistencies are indicated as red message underneath the respective athlete
and should be immediately fixed.

## Excel Export

The Excel export is similar to the PDF but meant for internal use and analysis. The athletes
are listed in rows by the sorting order specified; as there is no restriction on horizontal space
in a spreadsheet, all classification data (profile and file upload information) is displayed in a
single row.

This also allows enough space to include the additional columns with registration status and
uploaded form data; see [Classification Master List](reports/classification-master-list.md#other-options)
how to include specific information. In Excel, you may manipulate the report with your own search filters,
sorts, etc., but this is spreadsheet-specific and outside the scope of this manual.

## Classification Master List Widget

For ISAS, a publicly accessible widget is available that can be accessed on

<p class="text-center">
  <a href="https://isas.ibsasport.org/web" target="_blank">https://isas.ibsasport.org/web</a>
</p>

<figure>
    <img src="_img/figures/6.1-classification-master-list-widget.png" alt="Classification Master List Widget" class="screenshot" >
    <figcaption>Figure 6.1 - Classification Master List Widget</figcaption>
</figure>

The widget has a maximum width of 720px and is intended to be included via an HTML `<iframe>`
into any webpage. The public visitor selects the sport and decides on the format as they are
a browser version in HTML, a PDF version, an Excel sheet, and the underlying XML as possible
outputs.

It is also possible to publish links to these reports on any webpage which might be useful to
give the public a direct insight into the current classification master lists of IBSA
as all data are directly extracted live from ISAS. The format of the link is

<p class="text-center"><b>https://isas.ibsasport.org/web/cml/format/[:format]</b></p>

with

[:format] as desired output format of the report. Allowed values are:

- *html* - the HTML version of the master list
- *pdf* - the PDF version
- *excel* - an Excel version (xlsx extension, Excel 2007+)
- *xml* - a proper data exchange format based on the standard of the Olympic Data Feed
  (ODF) but with several application specific adjustments and codes

In comparison to the PDF reports of the password-protected ISAS environment
(see [PDF Export](reports/classification-master-list.md#other-options)), the
reports generated by this widget are designed for public use. Date of birth is
removed and replaced by the year of birth, some basic error indicators like
duplicated classes for single-class sports are removed and some specific
classification profile fields, like the extensions in swimming are included
upon request of the responsible federation.