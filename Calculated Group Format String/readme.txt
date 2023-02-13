Calculation Item

Value & % 

Expression:
SELECTEDMEASURE()

Format String Expression:
VAR AllData = CALCULATE(SELECTEDMEASURE(),ALLSELECTED('financials'))
VAR CalPro =  FORMAT( DIVIDE( SELECTEDMEASURE(), AllData )*100 ,"#,0")

RETURN
"#,0" & " (\"  & CalPro & " \% )"   

// FIRST THE FORMAT FOR THE 'SELECTED MEASURE' AND THEN THE '% CALCULATION' AND A '%'

