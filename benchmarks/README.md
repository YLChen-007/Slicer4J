
This document describes the structure of Slicer4J's benchmarks, and how to run them.

## Table of Contents
1. [Benchmarks structure](#Benchmarks-structure)
2. [Building the Tool](#Building-the-Tool)

---
---

## Benchmarks structure
  There are 11 benchmarks: 3 borrowed from JavaSlicer, 5 we created to highlight Slicer4J's strengths, and 3 real programs from the Defects4J dataset. 


### JavaSlicer benchmarks


<table class="tg">
    <thead>
        <tr>
            <th class="tg-73oq">Benchmark</th>
            <th class="tg-73oq">Folder</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="tg-73oq">Intra-procedural</td>
            <td class="tg-73oq">bench-javaslicer-simple1</td>
        </tr>
        <tr>
            <td class="tg-73oq">Inter-procedural</td>
            <td class="tg-73oq">bench-javaslicer-method1</td>
        </tr>
        <tr>
            <td class="tg-73oq">Exceptions</td>
            <td class="tg-73oq">bench-javaslicer-exception1</td>
        </tr>
    </tbody>
</table>

---

### Slicer4J benchmarks

<table>
    <thead>
        <tr>
            <th class="tg-73oq">Benchmark</th>
            <th class="tg-73oq">Folder</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="tg-73oq">Multiple threads</td>
            <td class="tg-73oq">bench3-threads</td>
        </tr>
        <tr>
            <td class="tg-73oq">Native methods</td>
            <td class="tg-73oq">bench2-nativeframework</td>
        </tr>
        <tr>
            <td class="tg-73oq">Java 9 constructs</td>
            <td class="tg-73oq">bench1-lambda</td>
        </tr>
        <tr>
            <td class="tg-73oq">Instrumentation classes</td>
            <td class="tg-73oq">bench4-tracerclasses</td>
        </tr>
        <tr>
            <td class="tg-73oq">Static Constructor</td>
            <td class="tg-73oq">bench5-staticconstructor</td>
        </tr>
    </tbody>
</table>

---

### Defects4J Programs

<table class="tg">
<thead>
    <tr>
        <th class="tg-73oq">Benchmark</th>
        <th class="tg-73oq">Folder</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td class="tg-73oq">JacksonCore: bug #4</td>
        <td class="tg-73oq">JacksonCore_4b</td>
    </tr>
    <tr>
        <td class="tg-73oq">JacksonDatabind: bug #3</td>
        <td class="tg-73oq">JacksonDatabind_3b</td>
    </tr>
    <tr>
        <td class="tg-73oq">Gson: bug #4</td>
        <td class="tg-73oq">Gson_4b</td>
    </tr>
</tbody>
</table>

---
---

## Running the Benchmarks

Run the script <code>run_benchmarks.py</code> using python3: <code>python3 run_benchmarks.py</code> <br>
The script creates a results folder, runs all benchmarks, and places the traces and slices in the results folder.