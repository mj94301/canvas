How to Use GPA CALCULATOR

Upload your Canvas Grades export file (Excel or CSV) in the same environment where you run the script.
Ensure column names match:

Student (for filtering out test rows)
Section (course section identifier)
Unposted Current Grade (letter grades: A, B+, C-, etc.)


Run the script:

It automatically uses the uploaded file.
Omits rows where Student == "Student, Test".
Detects all unique sections and processes each one.


Outputs:

PNG charts: GPA_hist_<Section>.png
Summary CSV: Average_GPA_by_section_summary.csv



Notes

GPA mapping uses the standard 4.0 scale:
A=4.0, A-=3.7, B+=3.3, B=3.0, B-=2.7,
C+=2.3, C=2.0, C-=1.7, D+=1.3, D=1.0, D-=0.7, F=0.0


Modify GRADE_COL if you want to analyze a different grade column (e.g., Final Grade).
The script assumes one sheet per Excel file and consistent column headers.
