I followed readme.md to try out.

since i don't want to install older visual studio, I used the following command to generate the project files for visual studio 2022:
```powershell
cmake -G "Visual Studio 17 2022" -A x64 .
# create a folder for build might be better
```

run `PIME.sln` in PIME folder.

build the solution (ctrl+shift+b).

grab file from `C:\Users\lifep\Devs\Public\kunchai\PIME\PIMETextService\Debug\PIMETextService.dll`

and 
*   Copy `PIMETextService.dll` to `C:\Program Files (X86)\PIME\x86\` and `C:\Program Files (X86)\PIME\x64\`
*   Copy the folder `python` `node`  from PIME to `C:\Program Files (X86)\PIME\`
*   
*   Use `regsvr32` to register `PIMETextService.dll`. 64-bit system need to register both 32-bit and 64-bit `PIMETextService.dll` run as administrator
```powershell
echo "please run as administrator"
regsvr32 "C:\Program Files (X86)\PIME\x86\PIMETextService.dll"
regsvr32 "C:\Program Files (X86)\PIME\x64\PIMETextService.dll"
```

then restart due to find no PIME option in input language.
![no pime](<./__files__/no pime.png>)

after restart, not a hint of PIME in input language.
- checked in all my PC language, English and Thai are not there.

I uninstalled. 

```powershell
regsvr32 /u "C:\Program Files (X86)\PIME\x86\PIMETextService.dll"
regsvr32 /u "C:\Program Files (X86)\PIME\x64\PIMETextService.dll"
```

## summary
I failed to install PIME.

