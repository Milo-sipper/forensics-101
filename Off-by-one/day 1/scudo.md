### UAFs
without quarantine and MTE, scudo doesent mitigate UADs, uses type confusions exploits the new tag 

### Scudo exploitation
u both need to guess chunk addresses and u need for forge checksums 

Zygote wused to speed up app start time by loading framework code / resources which poses a security risk due to storing metadata on the heap. Problem is scudo is initiated by zygote. 

### 1: Forged commitbase
- forge a fake secondary header
- Few constraints 
	- Write 0x28 bytes and free victim chunk + have a already occupied secondary chunk
Steps:
1. BOF
2. Forge fake secondary header 
3. Modify primary header 
4. target is placed in secondary cache 
5. allocate new secondary chunk and profit  