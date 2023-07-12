<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css" />
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
        <div class="section">
            <div class="container content">
                <h1 class="title">Seismic Retrofitting of Washington State Schools Would Cost Billions</h1>
                <h2 class="title">Overview</h2>
                <p> I created this project as a student in The Lede Program at Columbia University's Graduate School of Journalism. My goal was to explore the seismic readiness of Washington State public school buildings.
                </p>
                <p>
                  The <a href="https://fortress.wa.gov/dnr/geologydata/school_seismic_safety/phase2/School_Seismic_Safety_Project_2021_Final_Report_DNR.pdf">School Seismic Safety Project (SSSP) 2019–2021 Legislative Report</a> contains a 47-page chart showing the rankings of 561 school buildings that received geological and engineering assessments from 2017-2021. Since the report was published as a PDF, I experimented with several methods for scraping the data from the selected pages: PyPDF2, Camelot, and Tabula. Tabula had the best results, but the formatting had split some of the information fields in unintended ways. I wrote a formula in pandas to re-format some of the data, and then I exported the data to Excel for additional formatting work. When the data was fully cleaned, I moved it back to pandas to tally the seismic risk results and confirm the number of buildings and schools that were included in the analysis.
                </p>
                <p>To plot this information on a map, I needed school address data, which was available via the <a href="https://geo.wa.gov/datasets/23bbd746f9924c149681815cfd2a6300/explore?location=47.266088%2C-120.802250%2C7.02&showTabl">Washington Geospatial Open Data Portal</a>. I uploaded this dataset in pandas and deleted and renamed columns to reduce its size. Then I exported the data to Excel. Due to frequent variations in school name representations, I manually matched the two data sets via Excel. There were a handful of schools that could not be matched and were omitted from the data. These omissions are noted in the project.
                </p>
                <p> I made three data visualizations. The first was a symbol map in Datawrapper showing several thousand school locations, including the seismic risk rankings for the school buildings that were assessed as part of the SSSP. The second was a violin plot showing the correlation between the age of buildings and their seismic risk determinations, from a third data source. This data visualization was made using RawGraphs, and further edited using Adobe Illustrator. The third was a chart that I made with simple multiplication to show the estimated costs for retrofitting selected building types.
                </p>
                <p> 
                </p>
                <h2 class="title">Skills Learned</h2>
                <p>To create this project, I developed skills in PDF scraping using PyPDF2, Camelot, and Tabula, and data cleaning through pandas and Excel, and I experimented with RawGraphs and Adobe Illustrator. I learned about the many types of data variations that can occur when working with thousands of rows of data from more than one dataset, and the importance of documentation during data cleaning.
                </p>
                <h2 class="title">Future Work</h2>
                <p>To further develop this story, I want to explore data about tsunami risk zones, school enrollment, and prior seismic retrofitting work, in order to generate a fuller picture of the readiness of public school buildings across Washington State. I am also interested in incorporating data about private schools and daycares. I also want to learn how to conduct more data cleaning and merging work in pandas.
                </p>
                <p>https://efkodon.github.io/wa-schools-seismic/</p>
