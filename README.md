# Documents related to DC statehood constitution

Download constitutions:

    wget -O dc-home-rule-act.html http://dccode.org/home-rule-act/
    wget -O 1982-dc-constitution.pdf http://statehood.dc.gov/sites/default/files/dc/sites/statehood/page_content/attachments/1982%20Constitution%20for%20the%20State%20of%20New%20Columbia.pdf
    wget -O 1987-dc-constitution.html http://www.verfassungen.net/us/dc/verf87.htm
    wget -O 2016-draft-dc-constitution.pdf http://statehood.dc.gov/sites/default/files/dc/sites/statehood/publication/attachments/DRAFT%20CONSTITUTION%20PACKAGE%20FINAL.pdf

The 1987 constitution on the statehood.dc.gov site is a PDF of scanned images, with no text. The best text version
I could find is from a German site that collects constitutions.

Convert to text:

    pdftotext 1982-dc-constitution.pdf
    pdftotext 2016-draft-dc-constitution.pdf
    html-to-text < dc-home-rule-act.html > dc-home-rule-act.txt
    html-to-text < 1987-dc-constitution.html > 1987-dc-constitution.txt

If you have node.js installed, you can install html-to-text with `npm install -g html-to-text`.
