# Win UI Op

***Win UI Op with this plug-in can print all controllers on the windows interface and retrieve the value needed.***


## Win UI Op
| Item         |          Value           |
|--------------|:------------------------:|
| Icon         |  ![Win UI Op](icon.png)  |
| Display Name |      **Win UI Op**       |

### Arun Kumar (arunk@argos-labs.com)

Arun Kumar
* [email](mailto:arunk@argos-labs.com) 
 
## Version Control 
* [4.829.1404](setup.yaml)
* Release Date: `August 29, 2022`

## Input (Required)
| Function type                  | Parameters              | Output                   |
|--------------------------------|-------------------------|--------------------------|
| Print Control Identifiers      | uia or win32            | Control Identifiers:     |
|                                | Title                   |                          |
| Get Control Identifiers Value  | uia or win32            | Control Identifier Value |
|                                | Title                   |                          |
|                                | Control Identifier Name |                          |
| Print Control Identifiers      | uia or win32            | Control Identifiers:     |
|                                | Title                   |                          |
|                                | CMD Line                |                          |
| Get Control Identifiers Value  | uia or win32            | Control Identifier Value |
|                                | Title                   |                          |
|                                | CMD Line                |                          |
|                                | Control Identifier Name |                          |

Note:-

1. If required window interface already running skip CMD Line option.
2. win32 (Win32 API) & uia (MS UI Automation) pick one according to Interface.

:warning: **If Control Identifier Value already has comma separated**: deal it separately!


## Return Value

### Normal Case
Description of the output result

## Return Code
| Code | Meaning                      |
|------|------------------------------|
| 0    | Success                      |
| 1    | Exceptional case             |

## Output Format
You may choose one of 3 output formats below,

<ul>
  <li>String (default)</li>
  <li>CSV</li>
  <li>File</li>
</ul>  


## Parameter setting examples (diagrams)

## Operations


###  Print Control Identifiers:

![Win UI Op Input Data](README_1.png)


### Print Control Identifiers Value:

![Win UI Op Input Data](README_2.png)


###  Print Control Identifiers already running window:

![Win UI Op Input Data](README_3.png)


### Print Control Identifiers Value already running window:

![Win UI Op Input Data](README_4.png)
