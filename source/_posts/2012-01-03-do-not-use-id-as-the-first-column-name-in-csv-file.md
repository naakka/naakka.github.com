---
layout: post
type: message
title: Remember not to use ID as the first column name of a CSV file
link: http://stackoverflow.com/questions/6032049/openoffice-calc-can-not-read-a-simple-csv-file-why 
source: stackoverflow.com
quote: ID; in the first 3 characters of a file is the signature for a SYLK file. The fourth character can be a P, N or an E which flags certain information about how the rest of the file should be processed.
---

Remember not to use ID as the first column name of a CSV file when using semicolons as field delimiters.
I spent too long debugging a problem with CSV file creation when the problem was the first
column name.