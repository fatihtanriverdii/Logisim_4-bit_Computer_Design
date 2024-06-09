<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h1>Logisim 4-bit Computer Design</h1>

<p>This repository contains the design and implementation of a basic 4-bit computer using Logisim. The project demonstrates the fundamental principles of computer architecture through the use of a small, but functional, instruction set.</p>

<h2>Project Details</h2>

<h3>Memory and Registers</h3>
<ul>
    <li><strong>Memory:</strong> 16x8 bit</li>
    <li><strong>Registers:</strong> 
        <ul>
            <li>AR, PC, DR, AC, INPR, OUTR: 4 bit</li>
            <li>IR: 8 bit</li>
        </ul>
    </li>
</ul>

<h3>Instruction Set</h3>
<p>The project includes the implementation of the following instructions:</p>

<h4>Memory Reference Instructions</h4>
<ul>
    <li><strong>AND:</strong> Logical AND with the accumulator</li>
    <li><strong>ADD:</strong> Add to the accumulator</li>
    <li><strong>LDA:</strong> Load into the accumulator</li>
    <li><strong>STA:</strong> Store the accumulator</li>
    <li><strong>BUN:</strong> Branch unconditionally</li>
    <li><strong>BSA:</strong> Branch and save return address</li>
    <li><strong>RET:</strong> Return from subroutine</li>
</ul>

<h4>Register Reference Instructions</h4>
<ul>
    <li><strong>CLA:</strong> Clear accumulator</li>
    <li><strong>CLE:</strong> Clear E</li>
    <li><strong>CMA:</strong> Complement accumulator</li>
    <li><strong>INC:</strong> Increment accumulator</li>
    <li><strong>CIR:</strong> Circulate right accumulator</li>
    <li><strong>CIL:</strong> Circulate left accumulator</li>
    <li><strong>INP:</strong> Input</li>
    <li><strong>OUT:</strong> Output</li>
    <li><strong>HLT:</strong> Halt</li>
</ul>

<h3>Fetch-Decode-Execute Cycle</h3>
<p>The design follows the typical fetch-decode-execute cycle to process instructions.</p>

<h4>Fetch</h4>
<ul>
    <li><strong>T0:</strong> AR ← PC</li>
    <li><strong>T1:</strong> IR ← M[AR], PC ← PC + 1</li>
</ul>

<h4>Decode</h4>
<ul>
    <li><strong>T2:</strong> Decode IR(4-7), AR ← IR(0-3)</li>
</ul>

<h4>Execute</h4>
<p>Execution depends on the decoded instruction, involving data transfers, arithmetic operations, and control instructions.</p>

<h2>Getting Started</h2>
<p>To get started with this project:</p>
<ol>
    <li><strong>Clone the repository:</strong>
        <pre><code>git clone https://github.com/fatihtanriverdii/Logisim-4-bit-Computer-Design.git</code></pre>
    </li>
    <li><strong>Open the Logisim project file:</strong>
        <ul>
            <li>Launch Logisim.</li>
            <li>Open the <code>labproje.circ</code> file included in the repository.</li>
        </ul>
    </li>
    <li><strong>Run the simulation:</strong>
        <ul>
            <li>Use the simulation features of Logisim to observe the fetch-decode-execute cycle and the execution of various instructions.</li>
        </ul>
    </li>
</ol>

<h2>Contributing</h2>
<p>If you wish to contribute to this project, please fork the repository and create a pull request with your changes.</p>

<h2>License</h2>
<p>This project is licensed under the MIT License. See the <code>LICENSE</code> file for details.</p>

<h2>Contact</h2>
<p>For any questions or feedback, please contact <a href="mailto:f_tanriverdii@hotmail.com">f_tanriverdii@hotmail.com</a>.</p>

</body>
</html>
