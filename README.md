# Word Editor

***Word Editor with this plug-in can be read and modify the docx file header, footer, table, and paragraph.***


## Word Editor
| Item         |          Value           |
|--------------|:------------------------:|
| Icon         | ![Word Editor](icon.png) |
| Display Name |     **Word Editor**      |

### Arun Kumar (arunk@argos-labs.com)

Arun Kumar
* [email](mailto:arunk@argos-labs.com) 
 
## Version Control 
* [4.728.1004](setup.yaml)
* Release Date: `July 30, 2022`

## Input (Required)
| OP Type            | Parameters      | Output                         |
|--------------------|-----------------|--------------------------------|
| Read Header        |                 | p_id,paragraph                 |
| <br>               |                 |                                |
| Read Header        | Run             | p_id,r_id,paragraph            |
| <br>               |                 |                                |
| Update Header      | Paragraph Index | Updated file path              |
|                    | Paragraph Value |                                |
| Update Header      | Paragraph Index | Updated file path              |
|                    | Paragraph Value |                                |
|                    | Output Path     |                                |
| Update Header      | Paragraph Index | Updated file path              |
|                    | Run Index       |                                |
|                    | Paragraph Value |                                |
| Update Header      | Paragraph Index | Updated file path              |
|                    | Run Index       |                                |
|                    | Paragraph Value |                                |
|                    | Output Path     |                                |
| Read Paragraphs    |                 | p_id,paragraph                 |
| <br>               |                 |                                |
| Read Paragraphs    | Run             | p_id,r_id,paragraph            |
| <br>               |                 |                                |
| Update Paragraphs  | Paragraph Index | Updated file path              |
|                    | Paragraph Value |                                |
| Update Paragraphs  | Paragraph Index | Updated file path              |
|                    | Paragraph Value |                                |
|                    | Output Path     |                                |
| Update Paragraphs  | Paragraph Index | Updated file path              |
|                    | Run Index       |                                |
|                    | Paragraph Value |                                |
| Update Paragraphs  | Paragraph Index | Updated file path              |
|                    | Run Index       |                                |
|                    | Paragraph Value |                                |
|                    | Output Path     |                                |
| Read Table         | Table Index     | row_id,cell_id,value           |
| <br>               |                 |                                |
| Read Table         | Table Index     | row_id,cell_id,value           |
|                    | Row Index       |                                |
| Read Table         | Table Index     | row_id,cell_id,value           |
|                    | Row Index       |                                |
|                    | Cell Index      |                                |
| Read Table         | Table Index     | row_id,cell_id,p_id,r_id,value |
|                    | Row Index       |                                |
|                    | Cell Index      |                                |
|                    | Run             |                                |
| Update Table Rows  | Table Index     | Updated file path              |
|                    | Row Index       |                                |
|                    | Cell Index      |                                |
|                    | Row Cell Value  |                                |
| Update Table Rows  | Table Index     | Updated file path              |
|                    | Row Index       |                                |
|                    | Cell Index      |                                |
|                    | Row Cell Value  |                                |
|                    | Output Path     |                                |
| Update Table Rows  | Table Index     | Updated file path              |
|                    | Row Index       |                                |
|                    | Cell Index      |                                |
|                    | Paragraph Index |                                |
|                    | Run Index       |                                |
|                    | Row Cell Value  |                                |
| Update  Table Rows | Table Index     | Updated file path              |
|                    | Row Index       |                                |
|                    | Cell Index      |                                |
|                    | Paragraph Index |                                |
|                    | Run Index       |                                |
|                    | Row Cell Value  |                                |
|                    | Output Path     |                                |
| Read Footer        |                 | p_id,paragraph                 |
| <br>               |                 |                                |
| Read Footer        | Run             | p_id,r_id,paragraph            |
| <br>               |                 |                                |
| Update Footer      | Paragraph Index | Updated file path              |
|                    | Paragraph Value |                                |
| Update Footer      | Paragraph Index | Updated file path              |
|                    | Paragraph Value |                                |
|                    | Output Path     |                                |
| Update Footer      | Paragraph Index | Updated file path              |
|                    | Run Index       |                                |
|                    | Paragraph Value |                                |
| Update Footer      | Paragraph Index | Updated file path              |
|                    | Run Index       |                                |
|                    | Paragraph Value |                                |
|                    | Output Path     |                                |

### Notes:-
<ul>
    <li>p_id has information about Paragraph Index.</li>
    <li>r_id has information about Run Index.</li>
    <li>Run Index treated as sub-paragraph.</li>
    <li>row_id has information about Row Index.</li>
    <li>cell_id has information about Cell Index.</li>
    <li>Cell Index treated as sub-row.</li>
    <li>Output Path is an optional parameter to store an updated file, in case of no not being selected default updated file will store in the same location as the docx file.</li>
    <li>In case of empty Run Index put it as None. </li>
</ul>

## Return Value

### Normal Case
Description of the output result

## Return Code
| Code | Meaning                      |
|------|------------------------------|
| 0    | Success                      |
| 1    | Failure (Invalid Input Type) |
| 99   | Exceptional case             |

## Output Format
You may choose one of 3 output formats below,

<ul>
  <li>String (default)</li>
  <li>CSV</li>
  <li>File</li>
</ul>  


## Parameter setting examples (diagrams)

## Operations

### Sample Docx File:

[Word Editor Input Data](sample.docx)

### Read Header:

![Word Editor Input Data](WE_1.png)

### Read Header with Run:

![Word Editor Input Data](WE_2.png)

### Read Paragraphs:

![Word Editor Input Data](WE_3.png)

### Read Paragraphs with Run:

![Word Editor Input Data](WE_4.png)

### Read Table:

![Word Editor Input Data](WE_5.png)

### Update Paragraphs:

![Word Editor Input Data](WE_7.png)

### Update Table:

![Word Editor Input Data](WE_8.png)

### Update Table with Run:

![Word Editor Input Data](WE_9.png)
