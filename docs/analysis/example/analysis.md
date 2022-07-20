---
title: Analysis Template
---
<!---
The Analysis overview document is intended to be the gateway to the analytics documents and reporting of the project.

File name: /documentation/analysis/index.md
--->

{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

####<span style="color:coral">The price of a Big Mac in Argentina dramatically increased in 2018.<br>This continued through 2020.</span>
> Big Mac  
> **Cost** in ARS vs. EUR  
> Jan 2000..Jan 2020  

```vegalite
{
    "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
    "data": {
      "url": "https://cdn.jsdelivr.net/gh/koaning/justcharts/bigmac.csv", 
      "format": {
        "type": "csv"
      }
    },
    "mark": "line",
    "encoding": {
      "x": {"field": "date", "type": "temporal"},
      "y": {"field": "local_price", "type": "quantitative"},
      "color": {"field": "name", "type": "nominal"}
    }
}
```

### Discussion
**Q1:** { question }  
**A1:** { answer }  
**D1:** { discussion }  

**Q1:** { question }  
**A1:** { answer }  
**D1:** { discussion }  

----

???- example "Data Profile"
	=== "Field descriptions"
		|row|Field Name|Description|
		|:---|:---|:---|
		|1|rowid|row id|
		|2|date|Date (YYYY-MM-DD)|
		|3|currency_code|Currency code|
		|4|name|Country name|
		|5|local_price|Price in local currency|
		|6|dollar_ex|Unknown|
		|7|dollar_price|Unknown|

	=== "Raw Data Profile"
		```text
		1. "rowid"

			Type of data:          Number
			Contains null values:  False
			Unique values:         832
			Smallest value:        1
			Largest value:         17,250
			Sum:                   7,135,856
			Mean:                  8,576.75
			Median:                8,563
			StDev:                 4,993.93
			Most common values:    1 (1x)
								10 (1x)
								29 (1x)
								38 (1x)
								57 (1x)

		2. "date"

			Type of data:          Date
			Contains null values:  False
			Unique values:         32
			Smallest value:        2000-04-01
			Largest value:         2020-01-14
			Most common values:    2000-04-01 (26x)
								2001-04-01 (26x)
								2002-04-01 (26x)
								2003-04-01 (26x)
								2004-05-01 (26x)

		3. "currency_code"

			Type of data:          Text
			Contains null values:  False
			Unique values:         2
			Longest value:         3 characters
			Most common values:    ARS (416x)
								EUR (416x)

		4. "name"

			Type of data:          Text
			Contains null values:  False
			Unique values:         2
			Longest value:         9 characters
			Most common values:    Argentina (416x)
								Euro area (416x)

		5. "local_price"

			Type of data:          Number
			Contains null values:  False
			Unique values:         52
			Smallest value:        2.5
			Largest value:         171
			Sum:                   14,597.897
			Mean:                  17.546
			Median:                4.045
			StDev:                 30.098
			Most common values:    2.5 (39x)
								21 (39x)
								75 (39x)
								4.75 (26x)
								7 (26x)

		6. "dollar_ex"

			Type of data:          Number
			Contains null values:  False
			Unique values:         63
			Smallest value:        0.63
			Largest value:         60.066
			Sum:                   4,828.539
			Mean:                  5.804
			Median:                1.099
			StDev:                 10.626
			Most common values:    1 (26x)
								1.075 (13x)
								1.136 (13x)
								3.13 (13x)
								1.124 (13x)

		7. "dollar_price"

			Type of data:          Number
			Contains null values:  False
			Unique values:         63
			Smallest value:        0.799
			Largest value:         5.343
			Sum:                   2,930.106
			Mean:                  3.522
			Median:                3.705
			StDev:                 1.079
			Most common values:    2.5 (26x)
								2.381 (13x)
								2.262 (13x)
								0.799 (13x)
								2.376 (13x)

		Row count: 832
		```

	=== "Error Reporting"
		No errors.

#### Sample rows
{{ read_table('docs/analysis/example/data/bigmac.csv', sep = ',', nrows=10) }}

----

[Reproducible Reports with MkDocs](https://timvink.nl/reproducible-reports-with-mkdocs/)  
[IBSC Standards](https://www.ibcs.com/ibcs-standards-1-2/)