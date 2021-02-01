# ocr_dataset
This dataset has been created with a focus on layout evaluation of an OCR system.  
Containing close to a hundred documents that have been categorized on the basis of the column structure (single column vs multi column)  and page content (figures , math, tables or plain text )  
The annotation folder contains jsons with keys
1. multicolumn - Boolean indicates if the doc has multicolumn or single col layout.
2. figures - a list of all the bounding boxes of the images present on that page, if any.
3. tables - a list of all the table list elements, table list element is a two element list with the first one containg the location (bounding box) and second containg the content of that table in csv format.
4. maths - a list of all the math list elements. Each math list element is a 3 element list with the first element being the location (bounding box), second contating all the text content of that line and last element is a list which contains MathMl representation of all the math symbols of that line.
5. text - string with all the text contentof that page   
Bounding boxes are in relative YOLO format.
