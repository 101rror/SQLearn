<h2><a href="https://www.hackerrank.com/challenges/revising-the-select-query/problem">Revising the Select Query I</a></h2>
<img src="https://img.shields.io/badge/Difficulty-Easy-brightgreen" alt="Difficulty: Easy" />
<hr>

<p>
You are given a table named <code>CITY</code> with the following relevant fields:
</p>

<ul>
  <li><code>ID</code> – Integer</li>
  <li><code>NAME</code> – String</li>
  <li><code>COUNTRYCODE</code> – String</li>
  <li><code>DISTRICT</code> – String</li>
  <li><code>POPULATION</code> – Integer</li>
</ul>

<p>
Your task is to write a query that selects <strong>all columns</strong> from the <code>CITY</code> table for all cities where:
</p>

<ul>
  <li><code>COUNTRYCODE = 'USA'</code></li>
  <li><code>POPULATION &gt; 100000</code></li>
</ul>

<p>
Return the complete rows for all such cities.
</p>

<h3>Example Output (Structure Only)</h3>

<pre>
ID | NAME        | COUNTRYCODE | DISTRICT    | POPULATION
----------------------------------------------------------
... rows where country = 'USA' and population > 100000 ...
</pre>

<h3>SQL Solution</h3>

```sql
SELECT *
FROM CITY
WHERE COUNTRYCODE = 'USA'
  AND POPULATION > 100000;
