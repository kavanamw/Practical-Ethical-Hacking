GPP/cPassword Attack

* Group Policies Attack
	* allows admins to create poolicies using embedded creds
	* these creds were encrypted 
	* the key was accidentlly relesased 
	* patched in MS14-025 but works before that 

# Metasploit
	* use the smb_enum_cpp to find if this attack would be possible 