# ocr_dataset
This dataset, focused on evaluation of document layout analysis and OCR, has been created by a semi supervised approach as part of I-Assistant project funded by Microsoft's AI for Accessibility program. This contains 98 documents that have been categorized on the basis of their column structure (single column vs multi column)  and page content (figures, math, tables or plain text)  
The annotation folder contains jsons with keys
1. multicolumn - Boolean indicates if the doc has multicolumn or single column layout.
2. figures - a list of all the bounding boxes of the images present on that page, if any.
3. tables - a list of all the table list elements, where each table list element is a two-element list with the first one containing the location (bounding box) and second containing the content of that table in csv format.
4. maths - a list of all the math list elements. Each math list element is a 3 element list with the first element being the location (bounding box), second containing all the text content of that line and last element is a list which contains MathMl representation of all the math symbols of that line.
5. text - string with all the text on the page   
Bounding boxes are in relative YOLO format.
