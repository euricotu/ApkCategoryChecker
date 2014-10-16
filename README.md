# APK CATEGORY CHECKER #

Author: [Gabriele Martini](https://github.com/GabMar)

## DESCRIPTION ##

A Command-Line Program written in [Java](http://en.wikipedia.org/wiki/Java_%28programming_language%29) to decode an APK file or a directory containing APK files using ApkTool and check what Framework it's been used to build the APK.

## COMMAND LINE PARAMETERS ##


* `-p` : The Path of an APK or the Path of a directory containing APKs

* `-d` : Use current directory

* `-csv` : Export the results in a [CSV](http://it.wikipedia.org/wiki/Comma-separated_values) file

* `-o` : The destination directory of the result's file. If this parameter is missing, the result's file will be exported on the working path

* `-k` : Keep the directory of the encoded APK 

## USAGE EXAMPLE ##

* To analyze the directory containing the `ApkCategoryChecker.jar` and put the CSV result file in the same directory, open a terminal, navigate in the directory and type:

	`java -jar ApkCategoryChecker.jar -d -csv`

* To analyze a directory or an APK file and put the CSV result file in a different directory, open a terminal, navigate in the directory containing the 'ApkCategoryChecker.jar' file and type:

	`java -jar ApkCategoryChecker.jar -p /Path/of/The/Directory/or/APK/To/Analyze -csv -o /Destination/Path/for/Result/File`

* If you want to maintain the directory containing the decoded APK, add the parameter -k:

	`java -jar ApkCategoryChecker.jar -p /Path/of/The/Directory/or/APK/To/Analyze -csv -k`

## MINIMUM REQUIREMENTS ##

This software requires Java 1.7 or higher

## LICENSE ##

Copyright (C) <2014>  <Gabriele Martini>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

## 3RD-PART APPLICATIONS: ##

Apktool:   https://github.com/iBotPeaches/Apktool

Apache Commons CSV:   http://commons.apache.org/proper/commons-csv/

Apache Commons CLI:   http://commons.apache.org/proper/commons-cli/usage.html