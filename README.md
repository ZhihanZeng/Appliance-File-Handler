# Appliance-File-Handler
This project implements an `Appliance` class in Java that models an appliance with a serial number, providing:

- **Serial number validation** using regular expressions
- **Data Structures** using Treemap and applianceComparator
- **Comparison** (`compareTo`) for sorting appliances
- **File Input** (`inputFromFile`) to parse and read textfile lines
- **Equality checks** (`equals`) for duplicate detection
- **Custom output formatting** (`toString`)

## Features
- Validates serial numbers against the format:
  - Starts with `R`, `D`, or `W`
  - Followed by 11 alphanumeric characters
- Uses `Pattern` and `Matcher` for regex-based validation
- Implements object-oriented principles and inheritance
  - Divides into 3 seperate classes each with it's unique properties
- Reads and parses serial numbers from textfiles
  - Stores data into dynamic data structures using TreeMap
- Displayed on a GUI using Swing toolkit
  - Combines both JFrame and JMenu to create an interactive GUI
   

## Example
```java
Appliance fridge = new Appliance("RA12345678901");
System.out.println(fridge); // Output: [|||RA12345678901|||]
Microwave microwave = new Microwave("MD2314567889", 38.9, 90);
System.out.println(microwave.getprice()); // Output: 38.9
System.out.println(microwave.getWatts()); // Output : 90
