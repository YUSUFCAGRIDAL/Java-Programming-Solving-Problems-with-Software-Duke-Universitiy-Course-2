PROJECT TITLE     :Parsing Export Data
AUTHORS           :YUSUF ÇAĞRI DAL
USER INSTRUCTIONS :
The CSV file exportdata.csv has information on the export products of countries; you can download a .zip folder with this and other export data files here. In particular it has three column headers labeled Country, Exports, and Value (dollars). The Country column represents a country from the world, the Exports column is a list of export items for a country, and the Value (dollars) column is the dollar amount in millions of their exports in the format of a dollar sign, followed by an integer number with a comma separator every three digits from the right. An example of such a value might be “$400,000,000”.

The CSV file exports_small.csv is a smaller version of the file above with the same columns that you may find helpful in testing your program. We show a picture of it here.



Write the following program. Be sure to see the sample program in this lesson's videos.

Write a method named tester that will create your CSVParser and call each of the methods below in parts 2, 3, 4, and 5. You would start your code with:

12
FileResource fr = new FileResource();
CSVParser parser = fr.getCSVParser();
Each time you want to use the parser with another method, you will need to reset the             parser by calling fr.getCSVParser() again to get a new parser.

1
parser = fr.getCSVParser();
2. Write a method named countryInfo that has two parameters, parser is a CSVParser and country is a String. This method returns a string of information about the country or returns “NOT FOUND” if there is no information about the country. The format of the string returned is the country, followed by “: “, followed by a list of the countries’ exports, followed by “: “, followed by the countries export value. For example, using the file exports_small.csv and the country Germany, the program returns the string:

1
Germany: motor vehicles, machinery, chemicals: $1,547,000,000,000
3. Write a void method named listExportersTwoProducts that has three parameters, parser is a CSVParser, exportItem1 is a String and exportItem2 is a String. This method prints the names of all the countries that have both exportItem1 and exportItem2 as export items. For example, using the file exports_small.csv, this method called with the items “gold” and “diamonds” would print the countries

12
Namibia
South Africa
4. Write a method named numberOfExporters, which has two parameters, parser is a CSVParser, and exportItem is a String. This method returns the number of countries that export exportItem. For example, using the file exports_small.csv, this method called with the item “gold” would return 3.

5. Write a void method named bigExporters that has two parameters, parser is a CSVParser, and amount is a String in the format of a dollar sign, followed by an integer number with a comma separator every three digits from the right. An example of such a string might be “$400,000,000”. This method prints the names of countries and their Value amount for all countries whose Value (dollars) string is longer than the amount string. You do not need to parse either string value as an integer, just compare the lengths of the strings. For example, if bigExporters is called with the file exports_small.csv and amount with the string $999,999,999, then this method would print eight countries and their export values shown here: 

85672341