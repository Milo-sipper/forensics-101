SSPI - windows security support provider interface 
Main role is to perform authentication for windows products 
- It is currently the first level of defence and there has not been previous comprehensive 

security packages have been used in DLLs (dynamically linked libraries)

LSASS 
- security support providers are loaded by this 
- important data structures - credentiatls which contains certificates and logon data used by  SSP; security context which contains 



SSPI bugs bugs bugs bzzzzz
1. normal
	1. fuzzing and auditing can find. 
	2. (integer overflow and OOB write )
2. race condition 
	1. SSPI user called into LSASS via RPC 
	2. possibility to trigger race condition in lsas.exe 
	3. credentials / security context 
3. API misuse