| Title              | DN_0010_6_windows_sysmon_driver_loaded       |
|:-------------------|:------------------|
| **Author**         | @atc_project        |
| **Description**    | The driver loaded events provides information about a driver being loaded on  the system. The configured hashes are provided as well as signature  information |
| **Logging Policy** | <ul><li> Not existing </li></ul> |
| **References**     | <ul><li>[https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=90006](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/event.aspx?eventid=90006)</li><li>[https://github.com/Cyb3rWard0g/OSSEM/blob/master/data_dictionaries/windows/sysmon/event-6.md](https://github.com/Cyb3rWard0g/OSSEM/blob/master/data_dictionaries/windows/sysmon/event-6.md)</li></ul> |
| **Platform**       | Windows    |
| **Type**           | Applications and Services Logs        |
| **Channel**        | Microsoft-Windows-Sysmon/Operational     |
| **Provider**       | Microsoft-Windows-Sysmon    |
| **Fields**         | <ul><li>EventID</li><li>Computer</li><li>Hostname</li><li>UtcTime</li><li>ImageLoaded</li><li>Hashes</li><li>Sha256hash</li><li>Md5hash</li><li>Signed</li><li>Signature</li><li>SignatureStatus</li></ul> |


## Log Samples

### Raw Log

```
- <Event xmlns="http://schemas.microsoft.com/win/2004/08/events/event">
  - <System>
    <Provider Name="Microsoft-Windows-Sysmon" Guid="{5770385F-C22A-43E0-BF4C-06F5698FFBD9}" /> 
    <EventID>6</EventID> 
    <Version>3</Version> 
    <Level>4</Level> 
    <Task>6</Task> 
    <Opcode>0</Opcode> 
    <Keywords>0x8000000000000000</Keywords> 
    <TimeCreated SystemTime="2018-12-09T21:41:44.778524700Z" /> 
    <EventRecordID>4565</EventRecordID> 
    <Correlation /> 
    <Execution ProcessID="2996" ThreadID="3992" /> 
    <Channel>Microsoft-Windows-Sysmon/Operational</Channel> 
    <Computer>atc-win-10</Computer> 
    <Security UserID="S-1-5-18" /> 
  </System>
  - <EventData>
    <Data Name="RuleName" /> 
    <Data Name="UtcTime">2018-12-09 21:41:41.091</Data> 
    <Data Name="ImageLoaded">C:\Windows\System32\drivers\PROCEXP152.SYS</Data> 
    <Data Name="Hashes">MD5=8213C5972C91A56BE78CD02A4DE4E3FC,SHA256=95D07C3B8DF26790AC43BB4259F65D1E90B03EA31D66F1B3961D85E21C5FF590</Data> 
    <Data Name="Signed">true</Data> 
    <Data Name="Signature">Sysinternals</Data> 
    <Data Name="SignatureStatus">Valid</Data> 
  </EventData>
</Event>

```




