<!--# Automotive_Diagnostic_System
The objective of this project is to design an on-board diagnostic (OBD) system 
for an electric vehicle, using a PIC16F877A microcontroller and MPLAB X IDE development software. 
The system allows key sensors to be monitored and 
fault codes to be generated based on predefined thresholds. 
-->
<h1>Automotive Diagnostics System</h1>
<h3>Microcontroller-Based Automotive Monitoring Project</h3>
<p align="center">
  <img src="https://media.licdn.com/dms/image/v2/D4E22AQGUkbiPB5o0kw/feedshare-shrink_2048_1536/B4EZgD_5G.H4Ao-/0/1752413740365?e=1763596800&v=beta&t=m21eGXsMlsW3qeueEwfvP8HMRR8DIhSkiyGXPw_dv2U" height="80%" width="80%" alt="Automotive Diagnostics System"/>
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

<p align="center">
  <img src="https://media.licdn.com/dms/image/v2/D4E22AQH2989_HQXfVQ/feedshare-shrink_2048_1536/B4EZgD_5HSGYAo-/0/1752413744792?e=1763596800&v=beta&t=t8XCu5Y7N4815bG8pzbo_qDYBfk0-xCBatqT4Cmbno0" height="80%" width="80%" alt="Automotive Diagnostics System"/>
</p>
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
