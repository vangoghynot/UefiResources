Visit Site https://ubios.blogspot.com/  to get all versions

--------------------------------
# v1.0.1.4 (2025.5.17)
--------------------------------

--------------------------------
# v1.0.1.2 (2020.7.19)
--------------------------------
- Add Command Line option -noerrpause
  <br>"No Error Pause" option is added

- Add Serial Port ReadTimeOut/WriteTimeout Parameter
  <br>Add Serial Port ReadTimeOut/WriteTimeOut setting in Configuration

- Uefi Variable Dump
  <br>Add Hex view title to link to the variable name

- Acpi Table Dump
  <br>Add hex data dump

--------------------------------
# v1.0.1.1 (2020.6.26)
--------------------------------
- Add UEFI Variable Dump
   <br>Add Read UEFI Variable UI
   <br>**Need Administrator right!!!**

--------------------------------
# v1.0.1.0 (2020.5.14)
--------------------------------
- Remove the app administrator right requirment
- SUT Control improvement
  - 'Config' screen includes complete SUT control button definition and actions.
  - Invalid web request error display. 
- Console Window (VT100/ANSI)
  - Add Menu in FormConsole - 'Save ScreenAs'
  - Backspace key bug fixed
  - char background/foreground color bug fixed

--------------------------------
# v1.0.0.42
--------------------------------
 - DiskInfo
   -Show MBR information - bootable/nonbootable.
   -Show OS name in OsType field.

 - Add Command Line Mode
   - Arguments
     <br>-cli                   Command Line Mode
	   <br>-com [COM Settings]    COM port settings
	   <br>-file [FileName]       Logs will be save to this file
	   <br>-fchk [FileName]       The existence of this file will terminate the log capture  
	   <br>**Example:**
	          <br>plc -cli -com COM4:115200:None:8:ONE:None -file d:\mylog.txt -fchk stop.txt

  - Add SUT Control 
    <br>Add **"Sut Control"** field in Main Window.
    <br>The action string can be either web URL or executable file. Set the action string in "Option" window.
    <br>Below are the samples of the action string:
      <br>http://yourhost-ip/gpio/on/
      <br>d:\sut\AcPowerOn.bat      
      <br>d:\sut\PressPowerButton.exe

 - Console Window
   <br>Add "Backspace" key process.
