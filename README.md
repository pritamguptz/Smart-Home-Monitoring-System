<div align="center">
<h1><b><i>🚀 Smart Home Monitoring System</b></i></h1></div>


<h2>Overview</h2>
Smart Home Monitoring and Fire Alert System Using Arduino UNO<br>
This project is a Smart Home Monitoring and Fire Alert System developed using Arduino UNO. It monitors temperature, humidity, light intensity, and fire conditions in real time. The system provides automatic lighting control and emergency response during fire detection.
<hr>
<h2>Features</h2>

* Real-time temperature and humidity monitoring using DHT11
* Automatic light control using LDR sensor
* Real-time clock display using DS1307 RTC module
* Fire detection using Flame Sensor
* Automatic emergency light and fan activation during fire
* OLED display for live system monitoring
* Virtual Terminal output in Proteus
* Smart home safety and automation functions

<hr>
<h2>Components Used</h2>

* Arduino UNO
* OLED SSD1306 (128×64)
* DHT11 Sensor
* LDR Sensor
* Flame Sensor
* DS1307 RTC Module
* LED Bulb 1 (Automatic Lighting)
* LED Bulb 2 (Emergency Alert)
* DC Fan
* Proteus Design Suite

<hr><h2>Working Principle</h2>

The LDR sensor continuously monitors ambient light intensity. When the light level falls below a predefined threshold, Bulb 1 automatically turns ON. The DHT11 sensor measures temperature and humidity, while the DS1307 RTC provides real-time clock information.

A flame sensor continuously checks for fire hazards. When a flame is detected, the system immediately activates the emergency bulb and fan while changing the system status from SAFE to ALERT. All information is displayed on the OLED display and Virtual Terminal.
<hr>
<image src="Screenshot%202026-06-22%20at%2009.02.34.png">
<h2>Pin Configuration</h2>

<table>
  <tr>
    <th>Component</th>
    <th>Arduino UNO Pin</th>
  </tr>
  <tr>
    <td>DHT11 Sensor</td>
    <td>D7</td>
  </tr>
  <tr>
    <td>Fan</td>
    <td>D8</td>
  </tr>
  <tr>
    <td>Emergency Bulb (Bulb 2)</td>
    <td>D9</td>
  </tr>
  <tr>
    <td>Automatic Light (Bulb 1)</td>
    <td>D10</td>
  </tr>
  <tr>
    <td>Flame Sensor</td>
    <td>D11</td>
  </tr>
  <tr>
    <td>LDR Sensor (AO)</td>
    <td>A0</td>
  </tr>
  <tr>
    <td>DS1307 RTC SDA</td>
    <td>A4</td>
  </tr>
  <tr>
    <td>DS1307 RTC SCL</td>
    <td>A5</td>
  </tr>
  <tr>
    <td>OLED SDA</td>
    <td>A4</td>
  </tr>
  <tr>
    <td>OLED SCL</td>
    <td>A5</td>
  </tr>
</table>

<h2>System Logic</h2>

<table>
  <tr>
    <th>Condition</th>
    <th>Action</th>
  </tr>
  <tr>
    <td>LDR Value &lt; 300</td>
    <td>Bulb 1 (D10) Turns ON</td>
  </tr>
  <tr>
    <td>LDR Value ≥ 300</td>
    <td>Bulb 1 (D10) Turns OFF</td>
  </tr>
  <tr>
    <td>Flame Detected</td>
    <td>Fan (D8) ON + Emergency Bulb (D9) ON</td>
  </tr>
  <tr>
    <td>Flame Not Detected</td>
    <td>Fan (D8) OFF + Emergency Bulb (D9) OFF</td>
  </tr>
</table>

<h2>OLED Display Information</h2>

<table>
  <tr>
    <th>Display Item</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Time</td>
    <td>Current Time from DS1307 RTC Module</td>
  </tr>
  <tr>
    <td>Temperature</td>
    <td>Temperature from DHT11 Sensor</td>
  </tr>
  <tr>
    <td>Humidity</td>
    <td>Humidity from DHT11 Sensor</td>
  </tr>
  <tr>
    <td>LDR Value</td>
    <td>Light Intensity Reading</td>
  </tr>
  <tr>
    <td>Light Status</td>
    <td>ON/OFF Status of Bulb 1</td>
  </tr>
  <tr>
    <td>Flame Status</td>
    <td>DETECTED / NOT DETECTED</td>
  </tr>
  <tr>
    <td>System Status</td>
    <td>SAFE / ALERT</td>
  </tr>
</table>

<h2>OLED Output Example</h2>

<pre>
Time:14:35:22
Temp:27C
Hum:80%
LDR:245
Light:ON
Flame:NOT DET
Status:SAFE
</pre>



<hr><h2>Applications</h2>

* Smart Home Monitoring
* Fire Safety Systems
* Home Automation
* Environmental Monitoring
* Embedded Systems Projects

Developed By
<div align="center">
<h1 style="color:#0A66C2;">Pritam Kumar Gupta</h1>  
</div>
<br>
