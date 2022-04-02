+++
title = "000 BIPIN KUMAR JHA"

+++
[[BIPIN KUMAR JHA	2014-04-28, 06:19:36 [Source](https://groups.google.com/g/bvparishat/c/hRRGKjl9v48)]]



Dear scholars Namonamh,

  

1\. I am facing a problem while creating Sanskrit search engine with php my admin 3.5. I am able to search desired word from single row. I want to search from whole table (of that word isavailableanywherein that table).

  

Please help me with editing the codegivenbelow.

  

  

  

?>

\<form action="search.php" method="GET">

  

\<font color=green>\<b>Using 'iTrans' Please Enter Search Term :\</b>

  

\<input type="text" name="term" size="60" AUTOCOMPLETE = "off">

Results:

  

\<select name="results">

\<option value="10">Ten\</option>

\<option value="20">select\</option>

\<option value="50">select\</option>

  

\<td>\<input style="vertical-align:top; padding: 0px 0px;" id="button2" type="image" src="search.png" height="40" width="40" border="0" title="Search"/>\</select>

\</form>

\</center>

\<hr>

  

\<?php mysql_connect("localhost", "Tatsama_word", ""); mysql_select_db("test");

$sql=mysql_query("SELECT \* FROM searchengine WHERE Tatsama_word LIKE '$\_GET\[term\]%' LIMIT 50");

  

while($ser = mysql_fetch_array($sql)) {

echo "\<h5>\<a href='display.php?id=$ser\[ID\]'>$ser\[Tatsama_word\]\</a>\</h5>";

  

  

  

2\. I am still facing the last Devnagari display problem which was discussed with Shri[Nityanand Misra](https://mail.google.com/mail/u/0/h/zpeway0lpr6v/?&v=c&d=u&s=q&q=devanagari&n=3&th=144aa18c5cbe4aba#m_144aa11fed6ce6a1)ji and Shridhaval patel ji.

  

With regards

Bipin Jha

