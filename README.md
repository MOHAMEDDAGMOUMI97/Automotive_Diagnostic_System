<!--# Automotive_Diagnostic_System
The objective of this project is to design an on-board diagnostic (OBD) system 
for an electric vehicle, using a PIC16F877A microcontroller and MPLAB X IDE development software. 
The system allows key sensors to be monitored and 
fault codes to be generated based on predefined thresholds. 
-->
<h1>Automotive Diagnostics System</h1>
<h3>Microcontroller-Based Automotive Monitoring Project</h3>
<p align="center">
  <img src="https://ci3.googleusercontent.com/mail-img-att/AGAZnRrRhdik6HSew95Mi-z6FlDgfpCq7A1Funz0HFPoHpxjvm6CPOaRvqKe_Ojw9VD8rUHkH3pZWyj0E5wirGJ6hHdXGgwx_rSTFsTTEskHo7XZ9stN_Sx1ED19t2h-Cy7_fQiDl3mZNwwFrmjOXDlc9brqClyfuiuNbM3INylc4MoEwkxTSSm3nJy32iTVuB0S61WNpns9ZnTQz3PHRWSSn5SgQsqgrcIZxwSsIX1_1rzAm1hLegHDaZoTNfjEpeuwd6qEVtEofR3dL8EoUhAbegPgFXcoSSybZLGFspYagMnf_zjE1ET8p2X-fXc0N0Iq80PWRFlGK5ZYuvWE2YjwgDZTBDJ7ZWpGu40a2hq_eKi7umi7QHNok-AG5WTZJQfykQ6sSiMfOOO7YXq3OptQ-RjYO6zKq9WirlNfaUlvWYbDLxzil6x3s4B_S_vZnipYxI8kXairGDva9MoFif1pkDq7WiMP1IIN4tPavQOmK66No6ixY0yvdRV_sK37FKaZhdYaSpFY8xCvarnZRhzRaq7NtBdS0kHwCsL7wftTK9BhGjZ8LQozelVhV8_RCVmbM_DwITK01OGcCiB-Z9C_ck3wNq-mq-yGGdY7fibGThvX58tdLmWsHSQxTPM1hyfJJgU4cbFiMokfRyRFZ9yNHuu3IYTg2YZ99lHglPN7ua9bxRhBmxMnU9fMGcQxBeGnEy0VhzhKYdapEhtRifAOMXXySBZlJrVZE1eEX8RJ54cE9CsRAaMQsUxkpVVD4g78pZqCCX30FMyS4Dy7Q7wNjfyGs8IIGTiQF62ed9-brEBjs0p0eSmCICA-iGhTGrFHINW0h5Y0iRSNZcl8sO1scWKLda-x6gNOavE4Q1f0UQu3APmM9ltE_97OiX_dZ3ogoixIPRAr-libY1PDcM7e96XXwFMd9Avzjnv8WqydBrt2ojHxZzXR7lzpTW4kIkHGMjXonRQv5wva3glwnZEtRep1gIGmlepI80k2XlZgcMVJ0sCNaGMleYyB7Ykncq5f2t4Qz-qnFh1MZ_fiy-Dsj0HQIgVcGWMa0W0on82yLNK7nE1VT28w6aSXwInbc6yBFJaQiKq5N5Qizesl5fx19w=s0-l75-ft" height="80%" width="80%" alt="Automotive Diagnostics System"/>
</p>

<h2>Overview</h2>
<p>
This project aims to design and simulate an <b>On-Board Diagnostic (OBD)</b> system for an <b>electric vehicle</b> 
using the <b>PIC16F877A microcontroller</b>. Developed under <b>MPLAB X IDE</b> and simulated in <b>Proteus</b>, 
the system monitors key physical parameters — <b>temperature</b>, <b>voltage</b>, and <b>speed</b> — 
and transmits the data in real time to a serial terminal.
</p>

<h2>Objectives</h2>
<ul>
  <li>Develop an embedded diagnostic system capable of:</li>
  <ul>
    <li>Measuring <b>temperature</b> via the LM35 sensor.</li>
    <li>Monitoring <b>battery voltage</b> using an analog potentiometer.</li>
    <li>Calculating <b>vehicle speed</b> from a simulated sensor signal.</li>
  </ul>
  <li>Generate diagnostic codes when predefined thresholds are exceeded.</li>
  <li>Enable <b>real-time data visualization</b> through serial communication.</li>
</ul>

<h2>System Design</h2>
<ul>
  <li><b>Microcontroller:</b> PIC16F877A</li>
  <li><b>Software Tools:</b> MPLAB X IDE, Proteus</li>
  <li><b>Programming Language:</b> C</li>
  <li><b>Sensors Simulated:</b></li>
  <ul>
    <li>LM35 (temperature)</li>
    <li>Potentiometer (voltage)</li>
    <li>Signal generator (speed sensor)</li>
  </ul>
</ul>

<h2>Working Principle</h2>
<ol>
  <li>The LM35 and voltage sensors provide analog signals to the microcontroller’s ADC inputs.</li>
  <li>The Timer1 and CCP1 modules capture the period of an incoming square wave from the simulated speed sensor.</li>
  <li>The measured period is converted to frequency, then to linear speed (km/h) based on:
    <ul>
      <li>A wheel radius of <b>30 cm</b></li>
      <li><b>48 teeth</b> per revolution</li>
    </ul>
  </li>
  <li>The system sends real-time data (temperature, voltage, and speed) to a serial terminal for live monitoring.</li>
</ol>

<h2> Simulation Results</h2>
<ul>
  <li>Real-time monitoring of three key parameters.</li>
  <li>Stable and accurate readings from ADC and timer modules.</li>
  <li>Smooth serial data transmission with precise numerical output.</li>
  <li>Demonstrated the reliability of microcontroller-based diagnostics for EVs.</li>
</ul>

<h2>Key Learnings</h2>
<ul>
  <li>Hands-on experience with <b>embedded C programming</b> for PIC microcontrollers.</li>
  <li>Practical understanding of <b>sensor interfacing</b>, <b>signal processing</b>, and <b>serial communication</b>.</li>
  <li>Strengthened skills in <b>system simulation</b> and <b>data acquisition</b> for automotive applications.</li>
</ul>

<h2>Technologies Used</h2>
<p>
<code>PIC16F877A</code> • <code>MPLAB X IDE</code> • <code>Proteus</code> • <code>C Programming</code> • <code>USART Communication</code>
</p>

<h2>Conclusion</h2>
<p>
The project successfully demonstrated an embedded diagnostic system capable of monitoring essential vehicle parameters 
in real time. It represents a foundational step toward <b>smart automotive systems</b> and 
<b>IoT-based vehicle health monitoring</b>.
</p>
