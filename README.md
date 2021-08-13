# .gitignore file for TwinCAT3 and TwinCAT3 HMI

As the development in the TwinCAT environment continues, even if no new code is written, content of some files changes, and these changes raises a need to commit.
To avoid this situation, a proper .gitginore file should be used. That's why .gitignore file plays a significant role when it comes to using git with TwinCAT3 and TwinCAT3 HMI. 

# TwinCAT3 ignored files and folders
- *.library
- *.compiled-library
- *.compileinfo
- *.bootinfo
- *.bootinfo_guids
- *.tpy
- ***.tmc**
- *.tmcRefac
- *.project.~u
- *.tclrs
- *.tclrq
- *.tnzip
- *.tpzip
- *.tszip
- *.tsproj.bk?
- *.xti.bak
- *.xti.bk?
- LineIDs.dbg
- LineIDs.dbg.bak
- _Boot/
- _CompileInfo/
- _Libraries/
- _ModuleInstall/
- _Deployment/
- _Repository/

# TwinCAT3 HMI ignored files and folders
- Packages
- blob_storage/
- .engineering_servers/
- tsconfig.json
- liveview*.html

## Important note
As it can be seen above, .tmc file is untracked; however, in some cases .tmc file should be tracked. Here are two possible cases.

1. If the project includes TwinCAT C++ project
2. If "Standalone" project are being used
